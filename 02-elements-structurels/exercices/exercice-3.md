### Exercice 3 — Diagnostiquer une structure incorrecte

- **Objectif :** repérer les erreurs de structuration d'une page et justifier les corrections.
- **Durée indicative :** 25 min.



```html
<body>
  <main>
    <header> <!-- La balise <header> se trouve dans la balise <main> alors qu'elle doit se trouver dans la balise <body> -->
      <h1>Hôtel du Lac</h1>
      <nav>
        <ul>
          <li><a href="index.html">Accueil</a></li>
          <li><a href="chambres.html">Chambres</a></li>
          <li><a href="contact.html">Contact</a></li>
        </ul>
      </nav>
    </header>
    <section class="fond-bleu"> <!-- La balise <section doit normalement avoir un titre, or ici elle n'en a pas. De plus une section n'est pas utile pour un simple paragraphe -->
      <p>Bienvenue dans notre hôtel au bord du lac d'Annecy.</p>
    </section>
  </main>
  <footer> <!-- La balise <footer> se trouve normalement en fin de page or, ici elle se trouve en plein milieu -->
    <nav>
      <p>© 2026 Hôtel du Lac — Tous droits réservés</p>
    </nav>
  </footer>
  <main> <!-- Il y a deux fois la balise <main> -->
    <section>
      <h2>Actualités</h2>
      <section> <!-- Ici il vaut mieux utiliser la balise <article> car il s'agit d'un contenu autonome -->
        <h3>Ouverture de la terrasse</h3>
        <p>La terrasse rouvre le 1er mai.</p>
      </section>
    </section>
  </main>
</body>
```

