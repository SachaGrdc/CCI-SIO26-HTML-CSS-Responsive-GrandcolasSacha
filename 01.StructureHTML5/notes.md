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
3) Tout d'abord le navigateur analyse le code notamment avec la balise <DOCTYPE html>, ensuite il construit le DOM (qui transforme le code en arborescence d'objets et les balises en noeud)
4) La balise <head> contient les métadonnées de la page alors que la balise <body> sert à contenir le code visible de la page web.
5) Cette déclaration sert à définir la page comme une page HTML5, elle s'adresse au navigateur, si celle-ci n'est pas présente le navigateur passe en "Quirks mode" 
6) Le titre du document se trouve dans la balise <head> alors que le titre affiché dans la page si trouve dans la balise <body> puis dans <h1>
