### Exercice 1 — Analyser une structure faite de `div`

- **Objectif :** repérer où des éléments sémantiques seraient plus appropriés.
- **Durée indicative :** 25 min.



```html
<body>
  <div id="en-tete"> <!-- 1 Il faudrait utiliser la balise <header> car il s'agit d'un en-tête -->
    <div class="logo">Bibliothèque municipale</div>
    <div class="menu"> <!-- 2 Il faudrait utiliser la balise <nav> car il s'agit d'un bloc de navigation -->
      <a href="index.html">Accueil</a>
      <a href="catalogue.html">Catalogue</a>
      <a href="horaires.html">Horaires</a>
    </div>
  </div>
  <div id="contenu"> <!-- 3 Il faudrait utiliser la balise <main> car il d'agit du contenu principal de la page -->
    <div class="titre-page">Nos dernières critiques</div>
    <div class="critique"> <!-- 4 Il faudrait utiliser la balise <article> car il s'agit d'un élément indépendant à la page -->
      <h2>Le Petit Prince</h2>
      <p>Un conte poétique accessible à tous les âges.</p>
    </div>
    <div class="critique"> <!-- 5 Il faudrait utiliser la balise <article> car il s'agit d'un élément indépendant à la page -->
      <h2>Dune</h2>
      <p>Une épopée de science-fiction.</p>
    </div>
    <div class="info"> <!-- 6 Il faudrait utiliser la balise <section> car il s'agit d'un élément non diffusable seul -->
      <h2>Horaires d'ouverture</h2>
      <p>Du mardi au samedi, de 10 h à 18 h.</p>
    </div>
  </div>
  <div id="pied"> <!-- 7 Il faudrait utiliser la balise <footer> car il s'agit d'un pied de page -->
    <p>Contact : 12 rue des Lilas — 01 23 45 67 89</p>
  </div>
</body>
```

