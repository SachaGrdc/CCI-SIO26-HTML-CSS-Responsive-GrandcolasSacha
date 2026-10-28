# Séance 1 — Comprendre le Web et la structure d'un document HTML5



## Recherche autonome assistée par l'IA

Répondre aux questions suivantes :

- Qu'est-ce que HTML5 ?
- Que signifie « langage de balisage » ?
- Comment un navigateur interprète-t-il un document HTML ?
- Quelle différence existe-t-il entre `head` et `body` ?
- À quoi sert la déclaration `<!DOCTYPE html>` ?
- Quelle différence existe-t-il entre le titre du document et le titre affiché dans la page ?

1) HTML signifie HyperText Markup Language, HTML5 est la version 5 finalisé en 2014, c'est un langage qui décrit ce qu'est la structure ainsi que le contenu d'une page web notamment à l'aide des balises.
2) Le langage de balisage est un langage qui sert à annoter un texte avec des balises afin d'indiquer le rôle de chaque morceau du code mais ce n'est pas un langage de programmation car on ne calcule rien.
3) Le navigateur lit d’abord le fichier HTML et le décode en UTF-8 grâce à <meta charset>, puis il transforme les balises en un arbre d’objets appelé DOM, en même temps il télécharge les ressources externes. Il assemble ensuite le DOM et les styles dans un arbre de rendu qui ne garde que les éléments visibles puis il calcule la taille et la position de chacun selon la largeur de la fenêtre et affiche le tout à l’écran.
4) La balise <head> contient les métadonnées de la page, le titre de l'onglet, les liens vers d'autres pages tel que du CSS ou du JavaScript alors que la balise <body> sert à contenir le code visible de la page web.
5) Cette déclaration sert à définir la page comme une page HTML5, elle s'adresse au navigateur, si celle-ci n'est pas présente le navigateur passe en "Quirks mode" , c'est-à-dire le mode de compatibilité
6) Le titre du document se trouve dans la balise <head> alors que le titre affiché dans la page si trouve dans la balise <body> puis dans <h1>
7) La sémantique sert à utiliser des balises qui décrivent le sens et le rôle de leur contenu, il ne faut pas utiliser h1 pour obtenir un texte plus grand car les balises <h1> <h2> <h3> etc... servent à structurer la hiérarchie du contenu, pour obtenir un texte plus grand il faut utiliser le CSS.
8) La balise <ul> sert à faire des listes non ordonnées, c'est-à-dire regrouper les éléments où l'ordre n'a pas d'importance (sous forme de puces) alors que la balise <ol> sert à faire des listes ordonnées qui servent quand on a des éléments dont l'ordre compte (sous forme de numérotations)
   La balise <strong> sert à définir un texte comme très important, les navigateurs vont donc l'afficher en gras et les lecteurs d'écran le signalent à l'utilisateur la balise <b> sert elle à définir un texte comme peu important, elle va aussi mettre le texte  en gros mais ce n'est que visuel, c'est une balise de style et les lecteurs d'écran n'y prêtent pas d'importance.
