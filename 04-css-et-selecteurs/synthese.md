## Formalisation (20 min)

Synthèse : anatomie d'une règle (sélecteur, propriété, valeur), trois façons d'appliquer du CSS, types de sélecteurs, ordre de priorité (spécificité, ordre, héritage).



Une règle CSS se compose d'un sélecteur qui désigne les éléments à mettre en forme, il est  suivi d'un bloc entre accolades qui contient des déclarations. Chaque déclaration associe une propriété (l'aspect à modifier par exemple `color`) à une valeur (par exemple `blue`), séparées par `:` et terminées par `;`.

```css
h1 {
  color: blue;
}
```

Pour appliquer du CSS il faut relier le fichier CSS avec la balise `<link rel="stylesheet" href="style.css">` dans le `<head>`,  `rel="stylesheet"` sert à montrer au navigateur que le fichier relié est un fichier CSS et `href="style.css` sert à donner le chemin du fichier, il peut être relatif ou absolu.

Plusieurs types de sélecteurs permettent de cibler les éléments. Le sélecteur de balise `p` cible tous les éléments avec la balise `<p>`. Le sélecteur de classe `.important` cible les éléments qui ont l'attribut `class="important"` et peut être réutilisé. Le sélecteur d'id `#titre` cible l'élément qui a `id="titre"` et un id n'est là qu'une seule fois dans la page donc il est unique.

Quand plusieurs règles se contredisent la spécificité décide en premier : plus le sélecteur est précis plus il est prioritaire (style en ligne, puis id, puis classe, puis balise), si tout est à égalité c’est la dernière règle écrite qui l’emporte.

Enfin l'héritage fait que si aucune règle ne cible directement un élément certaines propriétés comme `color` ou `font-family` sont transmises par son parent mais il y a des exceptions comme  `margin` ou `border`

