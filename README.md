## Exercice : Création de la version Responsive du site

### Objectif

Votre mission est de proposer une **version responsive** du site web que vous avez réalisé précédemment.  
Le site doit pouvoir **s’adapter correctement aux différents types d’écrans** : ordinateur, tablette et smartphone.

### Consignes

1. Analysez la version actuelle du site.
2. Identifiez les éléments qui doivent être adaptés pour les petits écrans :
   - navigation
   - disposition des sections
   - images
   - textes
3. Mettez en place une **version responsive** en utilisant les techniques CSS appropriées :
   - **Media Queries**
   - **Flexbox et/ou Grid**
   - unités flexibles (`%`, `rem`, `vh`, `vw`, etc.).

### Livrables attendus

Vous devez fournir dans votre dépôt Git :

- Le **code mis à jour** du site avec la version responsive.
- Une **description dans ce README** expliquant :
  - les choix réalisés pour adapter le site
  - les breakpoints utilisés (mobile, tablette, desktop)
  - les principales modifications apportées au layout.

### Critères d’évaluation

- Bonne adaptation du site aux différents écrans
- Utilisation correcte de **Flexbox / Grid**
- Organisation et lisibilité du code
- Qualité de la documentation dans le README

## Version Responsive du site

Une version responsive a été mise en place à l’aide de CSS Grid, Flexbox et de Media Queries.

### Choix réalisés
- Utilisation de CSS Grid pour la structure principale
- Adaptation de la navigation selon la taille de l’écran
- Réorganisation des sections pour améliorer la lisibilité sur mobile

### Breakpoints utilisés
- Mobile : max-width 600px
- Tablette : max-width 900px
- Desktop : au-delà de 900px

### Modifications principales
- Navigation verticale sur desktop et tablette, horizontale sur mobile
- Services en 3 colonnes (desktop), 2 colonnes (tablette), 1 colonne (mobile)
- Sections empilées verticalement sur mobile