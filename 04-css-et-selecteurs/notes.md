# Séance 4 — Introduction à CSS3 et aux sélecteurs



## Recherche autonome assistée par l'IA (35 min)

- Comment fonctionne une règle CSS ?
- Quelle différence existe-t-il entre `p`, `.important` et `#titre` ?
- Comment relier un fichier CSS externe à une page HTML ?
- Que signifie la cascade CSS ?
- Comment le navigateur détermine-t-il la règle applicable lorsqu'il existe plusieurs déclarations contradictoires ?



1) Une règle CSS dit au navigateur quels éléments cibler et comment les mettre en forme elle se compose de deux parties, un sélecteur et un bloc de déclarations
2) Le sélecteur p s'applique à toutes les balises <p>, tandis que le sélecteur .important s'applique dans les éléments qui ont l'attribut class="important", ça peut être un p ou un div par exemple, enfin le sélecteur #titre s'applique aux éléments qui ont l'attribut id="titre", cet attribut ne peut être présent qu'une seule fois
3) Pour relier un fichier CSS à une page HTML il faut utiliser la balise <link>, celle-ci doit se trouver dans la balise <head>. Pour montrer que le fichier relié est un fichier CSS il faut utiliser l'attribut rel="stylesheet" ainsi que l'attribut href pour donner le chemin d'accès de fichier CSS, ça peut être un chemin relatif ou bien un chemin ou un chemin absolu.
4) La cascade CSS vient du nom même de CSS, en effet le C de CSS signifie Cascading, il s'agit de l'ensemble des règles qui permettent au navigateur de combiner plusieurs sources de style et de décider qu'est ce qu'il faut appliquer quand il y en a plusieurs.
5) Pour départager des déclarations contradictoires, le navigateur applique la cascade il regarde d’abord l’origine et l’importance (!important), puis les couches (@layer), puis la spécificité du sélecteur (style en ligne > #id > .classe > balise), si tout est à égalité c’est la dernière règle écrite qui l’emporte.