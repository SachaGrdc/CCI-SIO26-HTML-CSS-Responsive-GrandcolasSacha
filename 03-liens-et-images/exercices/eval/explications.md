### Évaluation — Corriger un document

**Objectif** : corriger un document contenant plusieurs erreurs de liens et d'images, puis expliquer les corrections.
**Durée** : 15 min, sans IA, sans aide de l'IA ; seuls le navigateur et les notes personnelles sont autorisés. Barème sur 20 donné au formateur.



Dans le fichier index.html,  dans ````<img src="images/logo.svg">``` il manque l'attribut alt, voici la version corrigée : 

```html
<img src="images/logo.svg" alt="Logo de l'atelier réseau">
```



Dans le fichier index.html,  dans ````<img src="images/banniere.jpeg" alt="banniere.jpeg">``` le format du fichier n'est pas le bon, dans le chemin c'est un .jpeg mais le fichier est un .jpg, de plus cette bannière est décorative donc il n'y a pas besoin de alt, voici la version corrigée : 

```html
<img src="images/banniere.jpg" alt="">
```



Toujours dans le fichier index.html, dans  ```<img src="C:\Users\eleve\Images\labo.png" alt="Photo du laboratoire réseau">``` le chemin n'est pas bon puisqu'il s'agit d'un chemin Windows personnel, il faut utiliser un chemin relatif, voici la version corrigée : 

```html
<img src="images/labo.png" alt="Photo du laboratoire réseau">
```



Pour finir dans le fichier index.html, dans `<a href="pages/stage.html#Candidature">Candidature au stage</a>` l'ancre contient une majuscule alors que l'id est en minuscule, voici la version corrigée : 

```html
<a href="pages/stage.html#candidature">Candidature au stage</a>
```



Et dans le fichier stage.html, dans ```<a href="index.html">Retour à l'accueil</a>``` le chemin n'est pas le bon car index.html est dans le dossier parent alors que stages.html est dans le dossier pages, il faut donc remonter d'un niveau, voici la version corrigée : 

```html
<a href="../index.html">Retour à l'accueil</a>
```

