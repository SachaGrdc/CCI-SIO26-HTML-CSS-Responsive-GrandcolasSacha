# Séance 6 — Le modèle de boîte CSS

*Fiche étudiant — 3 h — méthode : [annexe A](../12.%20-%20Annexes/A-consignes-etudiants.md)*

**Objectif général :** comprendre le calcul des dimensions et la gestion des espacements en CSS.





## Recherche autonome assistée par l'IA (35 min)

- Comment fonctionne le modèle de boîte ?
- Quelle différence existe-t-il entre `margin` et `padding` ?
- Comment calculer la largeur totale d'un élément avec `content-box` ?
- Quel est l'effet de `box-sizing: border-box` ?
- Comment utiliser l'inspecteur du navigateur pour analyser les espacements ?



1) Le navigateur traite chaque élément HTML comme une boîte rectangulaire, cette boîte a quatre couches qui va du centre vers l'extérieur, tout d'abord le content, c'est le contenu (texte, image) dont la taille est fixée par `width` et `height`, ensuite le padding, c'est l'espace entre le contenu et la bordure à l'intérieur de la boîte, de plus il y a la border, c'est la bordure qui entoure le padding et enfin le margin qui est l'espace transparent autour de la bordure, ça se trouve entre cette boite et les autres.

   Par exemple : 

   ```css
   .carte {
     width: 300px;
     padding: 20px;
     border: 2px solid #333;
     margin: 30px;
   }
   ```



2) Le paddig se trouve dans la boite, il est colorié par le fond de l'élément, les valeurs négatives, la valeur auto ainsi que l'effet de fusion y sont interdites alors que le margin se trouve à l'extérieur de la boite, il est toujours transparent, les valeurs négatives, la valeur auto ainsi que l'effet de fusion y sont autorisés.



3) Pour calculer la largeur totale d'un élément avec content box il faut utiliser cette formule : 

   ```
   Largeur totale = width + padding gauche + padding droit + border gauche + border droite
   ```

   Si on reprend cet exemple : 

   ```css
   .carte {
     width: 300px;
     padding: 20px;
     border: 2px solid #333;
     margin: 30px;
   }
   ```

   

​	cela fait ça : 300 + 20 + 20 + 2 + 2 = 344 px 



4) Par défaut, quand on écrit width: 300px, le navigateur applique ces 300 px au contenu seul. Le padding et la bordure s'ajoutent ensuite, donc la boîte finit plus large que prévu, avec box-sizing: border-box les 300 px comprennent tout : contenu, padding et bordure. La boîte fait donc bien 300 px quoi que vous ajoutiez à l'intérieur.



5) Il faut faire un clic droit sur l'élément puis « Inspecter », ensuite il faut regarder le schéma de la boîte dans l'onglet « Calculé » ou « Mise en page » qui affiche les valeurs de margin, border et padding. Enfin, on peut modifier ces valeurs en direct pour tester sans rien modifier