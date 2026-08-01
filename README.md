# Site N'KO-FINITION

## ⚠️ APERÇU EN LOCAL — À LIRE EN PREMIER

Si vous **double-cliquez** sur `index.html`, le navigateur passe en mode
`file://`. Dans ce mode, Chrome et Firefox **bloquent la lecture des fichiers
du site** pour des raisons de sécurité. Conséquence : la vidéo, la galerie et
l'avant/après ne peuvent pas se charger — ce n'est PAS un bug du site.

Le site le détecte et garde les encadrés visibles pour que vous puissiez juger
la mise en page, mais le contenu ne s'affichera vraiment qu'une fois en ligne.

**Pour un aperçu fidèle sur votre ordinateur**, ouvrez un terminal dans le
dossier du site et lancez :

    python -m http.server 8000

puis allez sur http://localhost:8000 dans votre navigateur.
Tout fonctionnera exactement comme sur le site en ligne.

---


Site vitrine 4 pages, 100 % statique (HTML/CSS/JS). Design clair premium, animation peinture, vraie carte interactive, emplacement vidéo. Aucun serveur.

## Fichiers
- `index.html` — accueil (hero animé, prestations, vidéo du patron, avant/après, carte 100 km, avis)
- `realisations.html` — galerie filtrable
- `a-propos.html` — présentation, valeurs, méthode
- `contact.html` — formulaire de devis détaillé + coordonnées
- `style.css` — charte commune
- `photos/` — vos images et vidéos

## Ce qui change dans cette version
- **Fonds clairs partout** : blanc chaud + sable, plus aucune section noire. Seul le pied de page est en brun chaud pour ancrer.
- **Nouvelles couleurs 2026** : terracotta (l'accent du peintre) + vert sauge naturel, palette chaude et élégante.
- **Animation peinture** dans le hero : le mot « couleur » se peint via un coup de pinceau au chargement, et un nuancier de pastilles apparaît en cascade (survolez-les).
- **Hero réagencé** : titre à gauche, visuel chantier à droite, chiffres alignés dessous. Plus clair et mieux hiérarchisé.
- **Vraie carte interactive** (OpenStreetMap) centrée sur Dax avec le cercle des 100 km.
- Adresse intégrée : **44 route de Montfort, 40100 Dax** (à vérifier).

## Ajouter la VIDÉO DU PATRON
Dans `index.html`, section « Le mot du fondateur », remplacez le bloc `.ph` + `.video-play` par :
```html
<video id="bossVideo" controls poster="photos/patron-poster.jpg">
  <source src="photos/patron.mp4" type="video/mp4">
</video>
```
Déposez `patron.mp4` (+ image `patron-poster.jpg`) dans `photos/`. Format 16/9, 1 à 2 min.

## Photos
Déposez les images dans `photos/`, puis remplacez chaque cadre `.ph` par :
```html
<img src="photos/mon-chantier.jpg" alt="Description" style="width:100%;height:100%;object-fit:cover">
```
- Accueil : image hero (portrait) + paire avant/après.
- Réalisations : 8 à 12 photos paysage (4/3).
- À propos : portrait de l'artisan (format 4/5).

## Infos à compléter (repères « à compléter » visibles)
Téléphone · horaires · Facebook/Instagram · texte « À propos » · avis supplémentaires · prénom/fonction du fondateur. Vérifiez l'adresse et la liste des communes.

## Activer le formulaire (gratuit, 5 min)
1. Compte sur https://formspree.io → New form, relié à `nkofinition@gmail.com`.
2. Copiez l'ID du formulaire.
3. Dans `contact.html`, remplacez `VOTRE_ID_FORMSPREE` par cet ID.

## Mettre en ligne (gratuit)
Glissez le dossier sur https://app.netlify.com/drop → en ligne en quelques secondes. Vous pourrez ensuite brancher un nom de domaine (ex. `nko-finition.fr`).

## Référencement local
Créez une fiche **Google Business Profile** pour N'KO-FINITION : c'est le levier n°1 pour apparaître sur « peintre Dax ».

---

---

## COORDONNÉES INTÉGRÉES

- Téléphone : **06 05 80 24 16** (cliquable sur mobile, sur les 4 pages)
- Email : nkofinition@gmail.com
- Adresse : **44 route de Montfort, 40100 Dax** — adresse actuelle confirmée.
  Le logo porte encore l'ancienne adresse (avenue du Sablar) : **le logo est à
  refaire**, sinon les deux adresses circuleront en parallèle (devis, cartes de
  visite, site) et brouilleront la fiche Google Business.
- Facebook, Instagram, TikTok : liés dans les pieds de page et la page Contact
- Mentions légales : E.I. SOUARE Ousmane · SIREN 934 590 761

⚠️ La page Facebook s'appelle « N'ko-services » et non N'KO-FINITION, et n'a
qu'une dizaine d'abonnés quand TikTok en compte plus de 250. Renommer la page
Facebook pour qu'elle corresponde à la marque.

## IDENTITÉ VISUELLE

Le **logo** reprend la charte de l'entreprise : « N'KO-FINITION » en bleu nuit
sur une plaque blanche bordée, comme sur le fichier d'origine — sans l'adresse,
sans le téléphone, sans le slogan. Uniquement le nom.

Le **site** garde sa charte chaude (terracotta et sable), plus juste pour un
métier de la couleur. Le logo y ressort d'autant mieux qu'il tranche.

## SECTION AVIS — À LIRE

L'ancienne section « Témoignages » contenait un avis **copié depuis la fiche
PagesJaunes d'une autre entreprise de peinture de Dax**, présenté comme un avis
de N'KO-FINITION. Il a été retiré : publier l'avis d'un tiers constitue une
pratique commerciale trompeuse (jusqu'à 300 000 € d'amende).

Aucun avis de N'KO-FINITION n'est aujourd'hui trouvable en ligne, hormis une
note 5/5 sur l'annuaire Obat (un seul avis, sans texte).

La section a donc été remplacée par **« Nos engagements »** — trois principes
concrets qui rassurent sans avoir besoin d'avis — et un bouton invitant les
clients à en déposer un sur Facebook.

**Dès que 3 vrais avis existent, remettez une section témoignages.** Le plus
simple : après chaque chantier terminé, Ousmane envoie un SMS avec le lien
direct vers sa fiche Google Business.

## ESPACE DE GESTION — Ousmane met ses photos à jour lui-même

Adresse : **votre-site.fr/admin**

⚠️ **Cette adresse ne fonctionne PAS en local ni sur un simple glisser-déposer.**
Elle n'existe qu'une fois le site déployé sur Netlify **depuis un dépôt GitHub**,
et après les 5 réglages ci-dessous. Avant ça, /admin affichera une page vide.

Il s'y connecte avec son email, ajoute un chantier (photo, titre, commune,
catégorie), et la page Réalisations se met à jour toute seule. Aucun code.

### Activation, une seule fois, après la mise en ligne sur Netlify
1. Netlify → votre site → **Site configuration → Identity → Enable Identity**
2. **Identity → Registration** → passer sur **Invite only**
   (sinon n'importe qui peut créer un compte et modifier le site)
3. **Identity → Services → Git Gateway → Enable**
4. **Identity → Invite users** → inviter nkofinition@gmail.com
5. Ousmane reçoit un email, choisit son mot de passe, et accède à /admin

Le site doit être relié à un dépôt Git (GitHub) pour que Git Gateway
fonctionne. Un simple glisser-déposer Netlify Drop ne suffit pas pour le CMS.

### Galerie Réalisations
**Aucun exemple n'est affiché** : la page ne montre que les vrais chantiers
ajoutés depuis /admin. Tant qu'il n'y en a aucun, un encart soigné annonce que
les photos arrivent et renvoie vers le devis — le site peut donc être mis en
ligne sans photos sans jamais paraître inachevé.
### Comparateur avant / après — piloté depuis /admin
Rubrique **② Avant / après** dans l'espace de gestion. Ousmane dépose deux
photos par comparaison (AVANT / APRÈS), avec un titre et une commune. Aucun
nom de fichier à respecter, aucun code à toucher.

**La première paire de la liste est celle qui s'affiche sur le site**, sur
l'accueil comme sur la page Réalisations. Pour changer de vitrine, il fait
glisser une autre paire tout en haut de la liste.

Tant qu'aucune paire n'existe, la section reste masquée et les fonds des
sections voisines se réorganisent seuls — la page n'a jamais de trou.

⚠️ Les deux photos doivent être prises **exactement du même endroit** : même
position, même hauteur, même cadrage. Sinon le glissement montre deux images
décalées au lieu d'une transformation. Astuce de chantier : poser un repère au
sol (un bout de scotch) avant de commencer, et se remettre dessus à la fin.

### Récapitulatif pour Ousmane
Dans /admin, deux rubriques et rien d'autre :
- **① Galerie — mes chantiers** : une photo = un chantier. Il en met autant
  qu'il veut, elles apparaissent sur la page Réalisations avec les filtres.
- **② Avant / après** : deux photos qui vont ensemble. La première de la liste
  s'affiche sur le site.

Aucun fichier à renommer, aucun dossier à gérer : le CMS s'en occupe.


## LA VIDÉO DU FONDATEUR

**Où la mettre : dans `photos/`, à la racine — PAS dans `photos/realisations/`**
(ce sous-dossier est réservé au CMS pour les photos de chantiers).

Nommez le fichier de l'une de ces façons, le site prend le premier qu'il trouve :

    photos/patron.mp4
    photos/fondateur.mp4
    photos/video.mp4
    photos/presentation.mp4

Rien d'autre à faire : la section « Le mot du fondateur » apparaît toute seule.
Tant qu'aucune vidéo n'est présente, elle reste masquée et les fonds des
sections voisines se réorganisent — la page n'a jamais de trou.

**Image d'attente (optionnelle mais recommandée)** : déposez
`photos/patron-poster.jpg`. C'est l'image figée affichée avant la lecture.
Sans elle, le navigateur montre la toute première image de la vidéo, qui est
souvent floue ou mal cadrée.

### Poids du fichier — important
Le format doit être **.mp4 (H.264)**, c'est le seul lu partout.
Visez **20 Mo maximum**, idéalement moins de 15 Mo.

Une vidéo de téléphone non compressée pèse facilement 150 Mo : elle serait
refusée par GitHub (limite 100 Mo par fichier), et surtout un visiteur en 4G
sur un chantier ne l'attendrait jamais. Pour compresser gratuitement, exportez
en 1080p à un débit d'environ 3 Mbit/s, ou passez le fichier dans HandBrake
(preset « Fast 1080p30 »).

Durée conseillée : **1 à 2 minutes**, format horizontal 16/9.
