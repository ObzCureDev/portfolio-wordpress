# Portfolio WordPress

Par Dan Nutu, fondateur de Bizleen, Product Engineer & Systems Engineer et créateur de MindVision Studio.

Ce dépôt présente deux sites WordPress montés entre 2020 et 2022 :

1. **All Patrimoine & Finance** (projet principal) : le site d'un cabinet de conseil en gestion de patrimoine, avec prise de rendez-vous en ligne, espace membres et réseau social interne.
2. **All Université** : une plateforme de formation en ligne (e-learning) pour les métiers de l'assurance, du crédit, de l'immobilier et du conseil financier.

Les deux sites ne sont plus en ligne. Les captures ont été faites en novembre 2026 sur une copie locale, restaurée à partir des fichiers et des bases sauvegardés (voir [Méthode](#méthode-des-captures)).

Le dépôt ne contient que ce fichier et des images. Ces sites sont construits par assemblage et configuration d'outils existants (thème, constructeur de pages, extensions), sans code sur mesure : le dépôt montre donc le résultat en images.

## Sommaire

- [All Patrimoine & Finance](#all-patrimoine--finance)
  - [Le site](#le-site)
  - [Pages publiques](#pages-publiques)
  - [Prise de rendez-vous en ligne](#prise-de-rendez-vous-en-ligne)
  - [Version mobile](#version-mobile)
  - [Administration](#administration)
  - [Espace membres](#espace-membres)
- [All Université](#all-université)
- [Méthode des captures](#méthode-des-captures)

---

## All Patrimoine & Finance

### Le site

**Mon rôle :** j'ai cofondé le cabinet et j'ai conçu et construit le site de bout en bout : le choix des modules, la façon de les combiner (rendez-vous, espace membres, contenus), toute la partie technique et l'hébergement sur mon propre serveur. Mes associés ont importé les textes et vérifié leur mise en page.

- **Adresse d'origine :** `all-patrimoine.finance` (hors ligne).
- **Ce que c'est :** le site vitrine et l'outil de travail d'un cabinet de conseil en gestion de patrimoine (CGP) : présentation des services, blog, glossaire, prise de rendez-vous avec un conseiller, et un espace réservé aux membres de l'équipe (profils, groupes, messagerie).

**Dates d'activité** (relevées dans la base de données et dans le dossier `uploads`) :

| Repère | Période |
|---|---|
| Premières pages et premiers médias | août 2020 |
| Articles du blog (75 publiés) | février à août 2021 |
| Rendez-vous enregistrés dans LatePoint (32) | juillet à novembre 2021 |
| Glossaire (273 définitions publiées) | octobre et novembre 2021 |
| Derniers médias envoyés | octobre 2021 |
| Dernières modifications de contenu | mars à juillet 2022 |
| Dernière connexion d'un membre | octobre 2022 |

**Outils :**

- **WordPress 6.0.2**, thème **BuddyBoss Theme 1.7.2** avec son thème enfant d'origine.
- **Mise en page :** Elementor 3.0.16 et Elementor Pro 3.0.9, complétés par Essential Addons, Happy Addons et Element Pack.
- **Rendez-vous :** LatePoint 4.3.3 et ses modules (champs personnalisés, emplacements, synchronisation Google Agenda, rappels, SMS par Twilio, QR code, fuseaux horaires) : 27 services, 3 conseillers, 11 départements ou modes de rendez-vous.
- **Communauté :** BuddyBoss Platform 1.7.4 et sa version Pro : profils, types de membres, groupes, messagerie privée, fil d'actualités, forums, médias et documents, invitations, modération.
- **Formulaires :** Super Forms (contact, candidature).
- **Contenus :** CM Tooltip Glossary pour le glossaire, TablePress, Yoast SEO Premium, Loco Translate.
- **Performance et sécurité :** WP Rocket, Redis Object Cache, Nginx Cache, Imagify, Wordfence, UpdraftPlus, Freesoul Deactivate Plugins (chargement des extensions page par page).
- Au moment de la dernière sauvegarde : 74 extensions installées, dont 60 actives.

**Hébergement :** sur un serveur personnel (machine virtuelle Linux) administré soi-même : nginx avec HTTPS (certificats Let's Encrypt), PHP 8.0 en FPM, MariaDB pour la base de données et Redis pour le cache d'objets.

### Pages publiques

Captures en 1440 px de large, en visiteur non connecté.

**Accueil**

![Accueil](all-patrimoine-finance/accueil.webp)

**Nos services**

![Nos services](all-patrimoine-finance/nos-services.webp)

**Une page de service : la gestion privée**

![Gestion privée](all-patrimoine-finance/gestion-privee.webp)

**Notre équipe**

![Notre équipe](all-patrimoine-finance/notre-equipe.webp)

**Rendez-vous sur mesure**

![Rendez-vous](all-patrimoine-finance/rendez-vous.webp)

**Contact** (haut de page)

![Contact](all-patrimoine-finance/contact.webp)

**Blog** (haut de page)

![Blog](all-patrimoine-finance/blog.webp)

**Glossaire** (haut de page)

![Glossaire](all-patrimoine-finance/glossaire.webp)

### Prise de rendez-vous en ligne

Le parcours du client, de bout en bout, dans la fenêtre de réservation LatePoint : choix du département, du service, du conseiller, de l'adresse, puis de la date et de l'heure, et enfin les coordonnées.

![Parcours de prise de rendez-vous](all-patrimoine-finance/reservation-parcours.gif)

| Étape | Capture |
|---|---|
| 1. Département | ![Choix du département](all-patrimoine-finance/reservation-1-departement.webp) |
| 2. Service | ![Choix du service](all-patrimoine-finance/reservation-2-service.webp) |
| 3. Conseiller | ![Choix du conseiller](all-patrimoine-finance/reservation-3-conseiller.webp) |
| 4. Date et heure | ![Choix de la date et de l'heure](all-patrimoine-finance/reservation-4-date-et-heure.webp) |
| 5. Coordonnées | ![Coordonnées du client](all-patrimoine-finance/reservation-5-coordonnees.webp) |

### Version mobile

Captures en 390 px de large (haut de page).

| Accueil | Nos services | Rendez-vous |
|---|---|---|
| ![Accueil sur mobile](all-patrimoine-finance/mobile-accueil.webp) | ![Nos services sur mobile](all-patrimoine-finance/mobile-nos-services.webp) | ![Rendez-vous sur mobile](all-patrimoine-finance/mobile-rendez-vous.webp) |

### Administration

**Tableau de bord WordPress** : le menu d'administration donne une idée de l'étendue de ce qui était monté.

![Tableau de bord](all-patrimoine-finance/admin-tableau-de-bord.webp)

**BuddyBoss : les composants activés**

![Composants BuddyBoss](all-patrimoine-finance/admin-buddyboss-composants.webp)

**LatePoint : agenda des conseillers, vue du jour**

![Agenda LatePoint, vue du jour](all-patrimoine-finance/admin-latepoint-jour.webp)

**LatePoint : agenda d'un conseiller, vue de la semaine**

![Agenda LatePoint, vue de la semaine](all-patrimoine-finance/admin-latepoint-semaine.webp)

**LatePoint : liste des rendez-vous**

![Rendez-vous LatePoint](all-patrimoine-finance/admin-latepoint-rendez-vous.webp)

**LatePoint : catalogue des services, classés par catégorie** (haut de page)

![Services LatePoint](all-patrimoine-finance/admin-latepoint-services.webp)

**LatePoint : les conseillers et leurs horaires**

![Conseillers LatePoint](all-patrimoine-finance/admin-latepoint-conseillers.webp)

**LatePoint : fichier clients**

![Clients LatePoint](all-patrimoine-finance/admin-latepoint-clients.webp)

**Elementor : l'éditeur sur la page d'accueil**

![Éditeur Elementor](all-patrimoine-finance/admin-elementor-editeur.webp)

**Super Forms : le constructeur du formulaire de contact**

![Constructeur Super Forms](all-patrimoine-finance/admin-super-forms-editeur.webp)

### Espace membres

Vu par un membre connecté.

**Annuaire des conseillers**

![Annuaire des membres](all-patrimoine-finance/membres-annuaire.webp)

**Groupes**

![Groupes](all-patrimoine-finance/membres-groupes.webp)

**Profil d'un membre**, avec sa carte de visite digitale (QR code flouté)

![Profil d'un membre](all-patrimoine-finance/membres-profil.webp)

**Messagerie privée**

![Messagerie](all-patrimoine-finance/membres-messagerie.webp)

---

## All Université

### Le site

- **Adresse d'origine :** `all-univer.site` (hors ligne).
- **Ce que c'est :** une plateforme de formation en ligne. Elle proposait des parcours de certification et de formation continue pour les intermédiaires en assurance (IAS), en opérations de banque (IOBSP), les conseillers en investissements financiers (CIF), la directive sur la distribution d'assurance (DDA) et la loi ALUR, avec inscription, catalogue de cours, leçons, quiz et une page sur le financement des formations (CPF, OPCO).

**Dates d'activité** (relevées dans la base de données et dans le dossier `uploads`) :

| Repère | Période |
|---|---|
| Premières pages et premiers médias | août 2020 |
| Dernières modifications des cours et des leçons | mai 2021 |
| Derniers médias envoyés | septembre 2021 |
| Dernière activité enregistrée dans BuddyBoss | octobre 2021 |

**Contenus pédagogiques publiés :** 23 formations, 75 leçons, 139 sujets, 87 quiz et 831 questions.

**Outils :**

- **WordPress 5.8.1**, thème **BuddyBoss Theme 1.6.5** avec son thème enfant d'origine.
- **Formation en ligne :** LearnDash 3.4.0.2, avec Course Grid, ProPanel, Notifications, le paiement par Stripe et Uncanny LearnDash Toolkit (et sa version Pro).
- **Ludification :** GamiPress 2.1.2, relié à LearnDash et à BuddyBoss.
- **Communauté :** BuddyBoss Platform 1.5.8 et sa version Pro.
- **Mise en page :** Elementor 3.0.16 et Elementor Pro, Essential Addons, Element Pack.
- **Performance et sécurité :** WP Rocket, Redis Object Cache, Wordfence, UpdraftPlus, Yoast SEO Premium.

**Hébergement :** sur le même serveur personnel : nginx avec HTTPS (Let's Encrypt), PHP 7.4 en FPM, MariaDB et Redis.

### Pages publiques

Captures en 1440 px de large, en visiteur non connecté.

**Accueil**

![Accueil](all-universite/accueil.webp)

**Les formations**

![Formations](all-universite/formations.webp)

**Les certifications IAS**

![Certifications IAS](all-universite/certifications-ias.webp)

**Le catalogue des cours** (LearnDash)

![Catalogue des cours](all-universite/catalogue-des-cours.webp)

**Une fiche de cours : la certification CIF**

![Fiche de cours CIF](all-universite/cours-certification-cif.webp)

**Le financement des formations**

![Financement](all-universite/financement.webp)

**Contact** (haut de page)

![Contact](all-universite/contact.webp)

### Version mobile

Captures en 390 px de large (haut de page).

| Accueil | Catalogue des cours | Fiche de cours |
|---|---|---|
| ![Accueil sur mobile](all-universite/mobile-accueil.webp) | ![Catalogue sur mobile](all-universite/mobile-catalogue-des-cours.webp) | ![Fiche de cours sur mobile](all-universite/mobile-cours-certification-cif.webp) |

---

## Méthode des captures

- **Restauration :** les fichiers d'origine des deux sites, montés en lecture seule, et leurs bases restaurées depuis la sauvegarde du 30 octobre 2026, dans des conteneurs Docker temporaires (PHP 7.4, MariaDB 10.11). Les adresses ont été remplacées par celles de la copie locale avec wp-cli. Les conteneurs ont été supprimés après les captures.
- **Extensions coupées sur la copie locale :** cache (WP Rocket, Redis, Nginx Cache), sécurité et redirections de connexion (Wordfence, LoginWP), mode maintenance, statistiques et suivi marketing, envoi de courriels et de SMS, application web progressive, protection contre la copie. Aucun courriel ni SMS n'est parti de la copie.
- **Différences avec les sites d'origine :**
  - l'année du pied de page est calculée à l'affichage, d'où « 2026 » ;
  - le reCAPTCHA du formulaire de contact est masqué : sa clé n'est valable que sur le domaine d'origine ;
  - les messages d'avertissement de l'administration, liés à la copie locale, sont masqués ;
  - les pages connectées le sont avec un compte administrateur temporaire, « Portfolio », créé pour l'occasion et retiré de l'annuaire des membres et du fichier clients.
- **Données personnelles :** les adresses e-mail, numéros de téléphone et adresses postales sont floutés sur toutes les captures, tout comme les noms des clients de LatePoint extérieurs à l'équipe et le QR code de la carte de visite. Aucune page affichant une clé d'API ou un identifiant de service tiers n'a été capturée.
- **Anciens associés :** leurs noms et leurs photos sont floutés sur toutes les captures, comme les coordonnées.
