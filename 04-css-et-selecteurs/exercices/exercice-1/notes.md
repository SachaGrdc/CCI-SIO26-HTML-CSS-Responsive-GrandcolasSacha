### Exercice 1 — Associer HTML et CSS

**Objectif** : créer une feuille de style externe et la relier à un document HTML.
**Durée indicative** : 15 min



Dans une règle CCS il y a un sélecteur qui montre les éléments à cibler, il est suivi d'un bloc entre accolades contenant des déclarations. Chaque déclaration associe une propriété à une valeur qui est séparées par un : et terminées par un ; h1

par exemple : 

```
h1 {
    color:blue;
}
```

 Dans cet exemple  `h1` est le sélecteur, `color` la propriété et `blue` la valeur



Les trois méthodes: 

-Externe (`<link>` vers `style.css`) : un seul fichier pour toutes les pages, il est facile à maintenir mais du coup ça rajoute un fichier à charger

-Interne (balise `<style>` dans le `<head>`) : pratique pour une seule page mais on ne peut pas réutiliser le style  sur les autres pages.

-En ligne (attribut `style`) : s'applique tout de suite à un seul élément et l'emporte sur les deux autres mais il mélange HTML et mise en forme et il se maintient très mal.