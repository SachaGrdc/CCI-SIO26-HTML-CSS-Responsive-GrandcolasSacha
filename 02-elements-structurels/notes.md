# Séance 2 — Organiser une page avec les éléments structurels HTML5

*Fiche étudiant — 3 h — méthode : [annexe A](../12.%20-%20Annexes/A-consignes-etudiants.md)*

**Objectif général :** comprendre et utiliser les éléments sémantiques qui organisent les grandes parties d'une page web.



## Recherche autonome assistée par l'IA (35 min)

- Quelle différence existe-t-il entre `section` et `article` ?
- Quel est le rôle de `main` ?
- Pourquoi utiliser `nav` pour une navigation principale ?
- Peut-on avoir plusieurs éléments `header` dans une page ?
- Dans quels cas faut-il préférer `div` à un élément sémantique ?



1) La balise <article> sert à créer un contenu autonome, il peut facilement être sorti de la page. La balise <section> elle sert  à regrouper du contenu thématiquement lié, elle est le choix par défaut lorsque aucun élément plus précis n'existe.
2) La balise <main> contient le contenu principal de la page, ça veut dire qu'elle ne se répète pas d'une page à une autre (pas de menu ni de pied de page), elle doit être unique
3) La balise <nav> dit au navigateur que c'est un bloc de liens de navigation, ce qui permet par exemple aux lecteurs d’écran d’y accéder directement.
4) Oui il peut en avoir plusieurs, chaque balise <section> ou <article> peut contenir un <header>
5) Il faut utiliser la balise <div> quand aucun élément sémantique ne convient et qu’il faut uniquement un conteneur, c'est souvent utilisé pour le CSS

