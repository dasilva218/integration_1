# Exercice : Création de la version Responsive du site

## ADAPTATION RESPONSIVE (HTML & CSS)

1. Choix réalisés pour adapter le site

   L’adaptation du site a été réalisée selon une approche mobile-first améliorée, en combinant :

   - Flexbox pour organiser les éléments principaux (navigation, contenu, sections)
   - Media queries pour ajuster le layout selon la taille d’écran
   - Une séparation des styles par contexte :
      - styles.css → version desktop (base)
      - mobile.css → adaptation mobile
      - tablette.css → adaptation tablette
      - watch.css → adaptation montre connectée

   Le layout repose principalement sur une structure flexible (display: flex) permettant de passer facilement d’un affichage en ligne (desktop) à un affichage en colonne (mobile/tablette).

2. Breakpoints utilisés

   Quatre formats principaux ont été définis :
   - Watch [@medi (max-width: 240px)] :
      - Taille de la police réduite à 10px
      - Navigation en pleine largeur
      - Contenu empilé verticalement
      - Services affichés en colonne

   - Mobile [@media (min-width: 240px) and (max-width: 768px)] :
      - Navigation en pleine largeur
      - Contenu empilé verticalement
      - Services affichés en colonne

   - Tablette [@media (min-width: 768px) and (max-width: 1024px)] :
      - Layout en colonne comme mobile et watch
      - Largeur du contenu centrée (≈ 80%)
      - Meilleure lisibilité avec marges automatiques

   - Desktop [Supérieur à 1024px (par défaut dans styles.css)] :
      Layout horizontal :
      - nav à gauche (20%)
      - hero à droite (80%)

3. Modifications principales du layout

   ### Structure globale

   Passage d’un layout fixe à un layout flexible avec Flexbox et utilisation de "flex-direction" pour gérer les changements :
   - row (desktop)
   - column (watch, mobile et tablette)

   ### Header et Footer

   Largeur de 100% sur tous les écrans et hauteur de 5em pour un ajustement en fontion du contenu.

   ### Navigation

   - Desktop : barre latérale (20%)
   - Watch / Mobile / Tablette : barre horizontale (100%)

   ### Section Hero

   - Adaptation automatique de la largeur
   - Alignement vertical
   - Bouton stylisé avec une marge intérieure (paddind) de 0.5em haut-bas et 1.5em gauche-droite

   ### Liste des services

   - Desktop : affichage horizontal
   - Watch / Mobile / Tablette : affichage vertical (flex-direction: column)
   - Chaque service concerve un aspect-ratio de 6/3 et prend toute la largeur sur petits écrans

   ### Centrage et lisibilité

   Réduction des largeurs sur tablette et ajout de marges automatiques (margin: auto) pour améliorer le confort visuel
