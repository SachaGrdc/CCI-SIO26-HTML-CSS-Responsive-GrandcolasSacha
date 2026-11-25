## Formalisation (20 min)

Synthèse : schéma annoté du modèle de boîte (contenu, padding, bordure, marge), formules de largeur totale pour `content-box` et `border-box`.



Schéma annoté du modèle de boîte :

```
┌──────────────────────────────────────────────┐
│ MARGIN (espace transparent, extérieur)       │
│  ┌────────────────────────────────────────┐  │
│  │ BORDER (bordure)                       │  │
│  │  ┌──────────────────────────────────┐  │  │
│  │  │ PADDING (espace intérieur)       │  │  │
│  │  │  ┌────────────────────────────┐  │  │  │
│  │  │  │ CONTENT (texte, image)     │  │  │  │
│  │  │  │ width × height             │  │  │  │
│  │  │  └────────────────────────────┘  │  │  │
│  │  └──────────────────────────────────┘  │  │
│  └────────────────────────────────────────┘  │
└──────────────────────────────────────────────┘
```

Formule de la largeur totale avec `content-box` (valeur par défaut) :

```
Largeur totale = width + padding gauche + padding droit + border gauche + border droit
```

Formule de la largeur totale avec `border-box` :

```
Largeur totale = width
Largeur du contenu = width − padding gauche − padding droit − border gauche − border droit
```

Exemple avec `width: 300px`, `padding: 20px` et `border: 2px` :

```
content-box : 300 + 20 + 20 + 2 + 2 = 344 px
border-box  : 300 px (le contenu fait 300 − 20 − 20 − 2 − 2 = 256 px)
```