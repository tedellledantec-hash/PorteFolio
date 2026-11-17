# DESIGN.md — Portfolio BTS SIO SISR

## 1. Direction artistique

Le portfolio adopte une identité visuelle moderne, sobre et professionnelle, orientée informatique, systèmes et réseaux.

L'univers graphique repose sur :
- un fond bleu nuit pour les zones immersives et les sections importantes ;
- des accents turquoise pour mettre en évidence les éléments interactifs et les mots-clés ;
- des surfaces claires pour faciliter la lecture des contenus ;
- une typographie sans-serif contemporaine ;
- des cartes, encadrés et séparateurs discrets pour organiser l'information.

L'objectif est de présenter un profil technique de manière claire, structurée et actuelle, sans surcharge décorative.

## 2. Palette de couleurs

| Rôle | Couleur | Code |
|---|---|---|
| Fond principal sombre | Bleu nuit | `#0B1724` |
| Fond sombre secondaire | Bleu ardoise | `#112638` |
| Fond sombre profond | Bleu très foncé | `#081522` |
| Accent principal | Turquoise | `#40D6C3` |
| Accent secondaire | Turquoise foncé | `#0B9D91` |
| Fond clair | Gris très clair | `#F5F7F8` |
| Fond de section clair | Gris bleuté | `#EAF1F2` |
| Surface / carte | Blanc | `#FFFFFF` |
| Texte principal clair | Blanc cassé | `#EAF1F4` |
| Texte secondaire clair | Gris bleuté | `#A9B8C5` |
| Texte principal sombre | Bleu gris | `#253545` |
| Bordures claires | Gris pâle | `#DFE7EB` |

Le bleu nuit est utilisé pour l'en-tête, le hero, les sections Compétences techniques, Parcours et Tableau E5, ainsi que le pied de page. Le turquoise sert aux mots mis en valeur, aux boutons, aux tags, aux icônes et aux indicateurs. Les sections de contenu utilisent un fond clair.

## 3. Typographie

Polices chargées depuis Google Fonts :
- **Manrope** : titres, grands textes d'accroche et éléments de marque.
- **DM Sans** : paragraphes, navigation, boutons, tableaux et textes courants.
- **ui-monospace** : contenu de la fenêtre de terminal dans la section d'accueil.

Les titres utilisent généralement une graisse 700 ou 800. Les paragraphes utilisent une graisse 400 à 600. Les petites légendes sont en capitales, en graisse 800 et avec un espacement des lettres augmenté.

## 4. Structure de la page

Le site est conçu comme une page unique avec navigation par ancres.

| Ordre | Section | Ancre | Contenu |
|---:|---|---|---|
| 1 | Accueil | `#accueil` | Présentation principale, spécialité SISR et liens d'action |
| 2 | Profil | `#profil` | Présentation, formation et approche personnelle |
| 3 | Compétences techniques | `#competences` | Virtualisation, systèmes, réseaux, cybersécurité, compétences transversales, développement et langues |
| 4 | Compétences acquises en stage | `#competences-stage` | Compétences effectivement mobilisées en milieu professionnel, avec niveaux à personnaliser |
| 5 | Parcours | `#parcours` | Chronologie de formation et lien vers le CV |
| 6 | Stages | `#experiences` | Expériences professionnelles et réalisations de stage |
| 7 | Réalisations | `#realisations` | Projets et travaux pratiques |
| 8 | Développement professionnel | `#developpement` | Environnement d'apprentissage, veille, identité et projet professionnel |
| 9 | Tableau de compétences E5 | `#tableau-e5` | Tableau de correspondance des réalisations avec les six compétences |
| 10 | Contact | `#contact` | E-mail, GitHub et LinkedIn |

La navigation reste visible en haut de l'écran lors du défilement. Le menu mobile se replie derrière un bouton hamburger.

## 5. Composants et styles

### En-tête et navigation
- Barre bleu nuit, positionnée en haut et sticky.
- Marque textuelle « PORTFOLIO. » avec un carré turquoise « P. ».
- Liens de navigation compacts.
- Lien Contact présenté comme un bouton contour turquoise.
- Sur mobile, navigation remplacée par un menu déroulant contrôlé par un bouton hamburger.

### Section d'accueil — Hero
- Fond bleu nuit avec dégradé bleu-vert et grille discrète.
- Mise en page en deux colonnes sur grand écran.
- Titre principal très visible, avec les mots importants en turquoise.
- Texte d'introduction et deux boutons d'action.
- Informations de contexte en petites lignes.
- Illustration décorative composée d'orbites, d'une fenêtre de terminal et de petits badges flottants.
- Sur mobile, les éléments sont empilés verticalement.

### Profil
- Trois cartes : présentation, formation et approche personnelle.
- Une carte accentuée en bleu ardoise.
- Encadré informatif sous les cartes.

### Compétences techniques
- Section bleu nuit, organisée en cartes sur deux colonnes sur grand écran.
- Catégories : Virtualisation, Systèmes, Réseaux, Cybersécurité, Compétences transversales, Développement et Langues.
- Chaque compétence est présentée sur une ligne avec un badge de niveau modifiable.
- Les badges utilisent trois classes : `beginner`, `intermediate` et `advanced`.
- Avant validation par le propriétaire du portfolio, le badge neutre `level-to-set` affiche « À définir ».
- Aucun graphique ni barre de progression n'est utilisé pour éviter de suggérer une mesure artificiellement précise.

### Compétences acquises en stage
- Section claire distincte des compétences générales.
- Cartes organisées par période de stage et organisme.
- Les éléments connus du stage ENSSAT concernent le développement Python, l'API REST HAPI, la plateforme CyberRange et la gestion de topologies réseau.
- La carte du stage de deuxième année reste à compléter avec les missions réellement effectuées.
- Les niveaux restent à définir par le propriétaire du portfolio.

### Cartes, stages et réalisations
- Fond blanc ou bleu ardoise selon la section.
- Bordure fine et rayon d'environ 8 à 10 px.
- Espacement intérieur généreux.
- Ombre légère sur les cartes claires.
- Animation de survol discrète sur les cartes de projets : légère remontée et ombre renforcée.
- Les stages utilisent un panneau latéral bleu nuit et une zone de contenu claire.

### Chronologie
- Date placée à gauche sur grand écran.
- Ligne verticale et point turquoise pour matérialiser le parcours.
- Carte de contenu à droite.
- Sur petit écran, la date et la carte sont réorganisées verticalement.

### Tableau de compétences E5
- Tableau horizontal avec en-tête bleu ardoise.
- Lignes de séparation et groupes de réalisations.
- Défilement horizontal possible sur les écrans étroits.
- Les coches sont turquoise.
- Les correspondances affichées sont indicatives et doivent être validées avec le tableau officiel E5.

### Contact et pied de page
- Bloc Contact sur fond bleu nuit avec dégradé discret.
- Coordonnées organisées en grille.
- Pied de page bleu très foncé, avec marque, contexte de formation et lien de retour en haut.

## 6. Boutons et interactions

- Bouton principal : fond turquoise, texte bleu nuit.
- Bouton secondaire : fond transparent et bordure claire.
- Bouton contour : fond transparent, bordure turquoise et texte turquoise.
- Les boutons remontent légèrement au survol.
- Les liens de navigation font défiler la page vers leur ancre.
- Le menu mobile s'ouvre et se ferme avec le bouton hamburger et se referme après sélection d'un lien.

## 7. Responsive design

Le design s'adapte aux ordinateurs, tablettes et téléphones.

### Grand écran
- Hero en deux colonnes.
- Cartes de profil et projets en trois colonnes.
- Cartes de compétences techniques en deux colonnes.
- Cartes de compétences de stage en deux colonnes.
- Développement professionnel en quatre colonnes.

### Écran intermédiaire
- Réduction des espacements et de la taille des titres.
- Grilles réorganisées pour conserver une lecture confortable.

### Mobile (700 px et moins)
- Menu de navigation déroulant.
- Hero en une seule colonne.
- Cartes empilées verticalement.
- Stages en une seule colonne.
- Chronologie réorganisée.
- Compétences techniques et compétences de stage en une seule colonne.
- Tableau conservant sa largeur minimale avec défilement horizontal.

## 8. Accessibilité et lisibilité

- Langue du document déclarée en français (`lang="fr"`).
- Balises HTML sémantiques : `header`, `nav`, `main`, `section`, `article` et `footer`.
- Bouton de menu doté d'un libellé accessible et de l'état `aria-expanded`.
- Contraste renforcé entre fonds sombres et textes clairs.
- Liens et boutons avec états de survol.
- Mise en page fluide sur petits écrans.

## 9. Arborescence prévue

```text
portfolio-one-page/
├── index.html
├── style.css
├── DESIGN.md
├── README.txt
├── images/
└── documents/
    ├── CV.pdf
    ├── tableau-de-synthese-E5.pdf
    ├── veille.pdf
    ├── stage1-cyberrange-dossier.pdf
    ├── stage1-cyberrange-code.zip
    └── ...
```

Les fichiers du dossier `documents/` doivent être ajoutés par le propriétaire du portfolio. Les liens vers des documents absents ne fonctionneront pas tant que les fichiers correspondants ne seront pas déposés.

## 10. Règles de cohérence

1. Conserver la palette bleu nuit / turquoise / gris clair.
2. Utiliser Manrope pour les titres et DM Sans pour le texte courant.
3. Privilégier des cartes simples et des espacements généreux.
4. Éviter les animations excessives et les effets visuels trop chargés.
5. Garder une navigation à ancres puisque le portfolio est une page unique.
6. Garder distinctes les compétences générales et celles réellement acquises en stage.
7. Laisser les niveaux à la validation du propriétaire : ne pas attribuer automatiquement un niveau.
8. Vérifier le rendu sur mobile après chaque modification.
9. Ne publier que des informations personnelles, dates, compétences et réalisations exactes et vérifiées.
