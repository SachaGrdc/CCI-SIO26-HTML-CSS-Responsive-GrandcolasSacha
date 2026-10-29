### Exercice 4 — Diagnostiquer une erreur

**Objectif** : trouver la cause réelle de liens ou d'images qui ne fonctionnent pas.
**Durée indicative** : 25 min



Si la page ne remonte pas c'est parce que il y a une majuscule à services dans la balise <a>, j'ai pu vérifier que ça marche en faisant la correction car la page page défile correctement, voici le code corrigé : 

```html
<a href="#services">Services</a>
```



Le schéma ne s'affiche pas car dans le code, le nom de l'image n'est pas correct, il y a un tiret du bas au lieu d'un tiret, voici le code corrigé : 

```html
<img src="img/schema-reseau.png" alt="Schéma du réseau du lycée">
```



L'image ne s'affiche pas en ligne car linux fait la différence entre les majuscules et les minuscules contrairement à Windows et Mac os, en effet le nom du fichier dans l'arborescence comporte des majuscules alors que dans le code tout est en minuscule, voici le code corrigé : 

```html
<img src="img/Photo-Salle.jpg" alt="Salle informatique">
```



La page est cassée car il manque un guillemet pour fermer l'attribut href, voici le code corrigé : 

```html
<a href="docs/guide.pdf">Télécharger</a>
```



Le site ne charge pas correctement car le lien n'a pas de protocole, le navigateur pense donc qu'il s'agit d'un chemin relatif du même site, voici le code corrigé : 

```html
<a href="https://www.education.gouv.fr">education.gouv.fr</a>
```

