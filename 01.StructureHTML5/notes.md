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



## Formalisation

Dans un document HTML5, le code commence par <!DOCTYPE html> afin de définir le document comme de l'HTML pour le navigateur puis on utilise la balise <html lang="fr"> pour définir que le document est en langue française, c'est utile pour le navigateur, le moteur de recherche ainsi que les outils de traductions.

Après cela nous devons mettre la balise <head> qui regroupe toutes les métadonnées de la page tel que le nom de la page (dans l'onglet) , <meta charset="UTF-8"> pour définir l'encodage de la page , <link> afin de lier des pages CSS ou encore <script> pour lier des pages JavaScript.

Pour finir la balise <body> sert à contenir tout le contenu visible dans la page avec des balises tel que <p> pour faire un paragraphe ou encore <h1> pour pouvoir faire des titres. Elle inclue aussi des balises tel que <sections> ou encore <div> pour structurer son code.

HTML sert à structurer le code, CSS à le mettre en forme et Javascript à mettre de l’interactivité. 

Le navigateur lit le code pour construire le DOM, cela signifie que ça transforme le code en arborescence d'objets et les balises en noeud, il charge les fichiers liés tel que le CSS, les images ou encore le JavaScript puis pour finir il l'affiche à l'écran.



