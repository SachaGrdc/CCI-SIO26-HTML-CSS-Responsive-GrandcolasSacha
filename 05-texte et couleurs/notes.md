# Séance 5 — Les propriétés CSS de texte, de couleurs et de présentation





## Recherche autonome assistée par l'IA (35 min)

- Comment définir une couleur en CSS ?
- Quelle différence existe-t-il entre `px`, `em` et `rem` ?
- Comment choisir une police de caractères ?
- Quelle différence existe-t-il entre `font-weight` et `font-style` ?
- Pourquoi le contraste est-il important pour l'accessibilité ?





1) Pour définir une couleur en CSS il faut sélectionner une balise HTML puis on ouvre des accolades, dedans on met mettre différentes propriétés : 

   -`color` : pour définir la couleur du texte

   -`background-color` : pour définir la couleur du fond

   -`border` : pour définir la couleur des bordures

   ```css
   h1 {
     color: #2c3e50;
     background-color: hsl(210, 20%, 95%);
   }
   ```

   

2) `px` : unité absolue fixe. 16px reste 16px quel que soit le contexte

   `em` : relative à la taille de police de l'élément parent . Elle se cumule dans les éléments imbriqués : un `1.5em` dans un `1.5em` donne 2,25 fois la taille de base

   `rem` : relative à la taille de police de la racine (`<html>`, 16px par défaut). Elle ne se cumule pas donc elle est plus prévisible

   

3) Lisibilité d'abord : une police claire, avec des lettres bien distinctes (par exemple `l`, `I` et `1`).

   Adaptée au contenu : sans-serif (Arial, Roboto, Open Sans) pour les écrans et les interfaces, serif (Georgia, Merriweather) pour les textes longs ou un ton plus classique.

   Pas plus de 2 polices : une pour les titres et une pour le corps de texte

   Cohérente avec l'identité du site ou du projet

   

4) La propriété `font-weight` gère l'épaisseur du trait, par exemple normal (400) ou bold (700) tandis que `font-style` gère l'inclinaison par exemple normal ou italic

   ```css
   strong { font-weight: 700; }
   em     { font-style: italic; }
   ```



5) Le contraste est important pour que tout le monde puisse lire notre site web, c'est notamment utile pour les personnes malvoyantes, les daltoniens, les personnes âgées ainsi que l'ensemble des visiteurs quand il y a du soleil sur l'écran ou de la fatigue par exemple.