1. # Partie A - Calcul de spécificité

   p : (0, 0, 1)

   .carte : (0, 1, 0)

   #entete : (1, 0, 0)

   header nav a : (0, 0, 3)

   ul.menu li : (0, 1, 2)

   #menu a.actif : (1, 1, 1)

   a:hover : (0, 1, 1)

   input[type="text"] : (0, 1, 1)

   .carte .titre : (0, 2, 0)

   body #page .contenu p : (1, 1, 2)

   ## Comparaison des paires

   .titre (0, 1, 0) vs h1.titre (0, 1, 1) = h1.titre gagne (une balise en plus)

   #menu a (1, 0, 1) vs .menu .lien.actif (0, 3, 0) = #menu a gagne (1 identifiant bat 3 classes).

   p (0, 0, 1) vs * (0, 0, 0) = p gagne (* vaut 0).

   ## Règles des spécificités

   Quand deux règles ont la même spécificité c'est la dernière écrite dans le fichier CSS qui gagne
   Pour <p class="titre carte"> la couleur sera rouge parce que .titre est déclaré après .carte parce que en HTML l'ordre ne compte pas 

   ## L'ordre de priorité

   Du plus fort au plus faible :
   1. !important
   2. Style en ligne (style="")
   3. #id
   4. Classe
   5. Balise

   Pour <p id="menu"> la couleur sera bleu parce que !important est plus importante même devant un #id