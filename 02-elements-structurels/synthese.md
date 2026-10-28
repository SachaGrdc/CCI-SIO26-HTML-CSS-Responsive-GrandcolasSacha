# Séance 2 — Organiser une page avec les éléments structurels HTML5

*Fiche étudiant — 3 h — méthode : [annexe A](../12.%20-%20Annexes/A-consignes-etudiants.md)*

**Objectif général :** comprendre et utiliser les éléments sémantiques qui organisent les grandes parties d'une page web.



## Formalisation (20 min)

|  Élément  | Rôle                                                         | Exemple d'usage                               | Erreur courante                                              |
| :-------: | :----------------------------------------------------------- | --------------------------------------------- | :----------------------------------------------------------- |
| <article> | Contenu autonome qui garde son sens s'il est sorti de la page | Article de presse                             | L'utiliser pour n'importe quel bloc                          |
| <section> | Regroupement thématique de contenu                           |                                               | L'utiliser comme simple conteneur de style, ou sans titre    |
|  <main>   | Contenu principal et unique de la page sans ce qui se répète (menu, pied de page) | Faire un bouton "Retour au contenu principal" | En mettre plusieurs sur une page, ou y placer le menu et le pied de page |
|   <nav>   | Bloc principal de liens de navigation                        | Menu du site                                  | Mettre les liens du pied de page                             |
| <header>  | Contenu d'introduction d'une page ou d'une section (titre, logo, menu) | En-tête du site                               | Le mettre dans un autre <header>                             |
|   <div>   | Conteneur générique sans signification, pour le style ou la mise en page | Pour le CSS et le JavaScript                  | L'utiliser partout par réflexe alors qu'un élément sémantique existe |

