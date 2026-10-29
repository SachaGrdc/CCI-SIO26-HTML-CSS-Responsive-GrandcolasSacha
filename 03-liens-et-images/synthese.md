## Formalisation (20 min)

Synthèse : syntaxe de `a` et `img`, règles des chemins (`./`, `../`, dossier, racine), fragments, règles pour `alt`, liste de vérification d'un lien/image cassé.



Au niveau de la syntaxe, il faut écrire la balise <a> de cette manière, on peut remplacer Destination par une image

```html
<a href="destination.html">Destination</a>
```

 et pour la balise <img> ça s'écrit comme ça, src signifie source, et alt sert à mettre un texte de remplacement en cas d'un problème de chargement, les lecteurs d'écran s'en servent aussi pour lire la page.

```html
<img src="strasbourg.png" alt="image de Strasbourg">
```

 

Pour les chemins, il existe deux types de chemins, le chemin relatif et le l'URL absolue.

L'URL absolue donne l'adresse complète, elle sert donc généralement à pointer vers un autre site internet mais elle fonctionne n'importe où, y compris dans un même site interne, une URL absolue peut ressembler à ça : https://exemple.com/fichier

Le chemin relatif lui indique l'emplacement d'un fichier par rapport à la page actuelle, c'est-à-dire que si on met le nom d'un fichier qui est dans le même dossier (par exemple : fichier.html), le même dossier parent (par exemple : ../fichier.html) ou alors dans un sous dossier (par exemple : dossier/fichier.html) ça va marcher mais si on déplace le fichier et qu'on ne met pas à jour le chemin, le lien ne fonctionnera plus comparé à l'URL absolue. Le chemin relatif sert uniquement à pointer vers une page d'un même site internet.

Les fragments servent à donner un id unique à un élément (section, article etc...) puis à pointer vers celui-ci depuis un menu par exemple, voici à quoi peut ressembler un id dans un élément : 

```html
<h2 id="conclusion">
```



L'attribut alt à plusieurs règles, il est obligatoire sur chaque balise <img> et il décrit de façon simple une image.



Il faut tout d'abord vérifier que le chemin de l'image est bon, que l'image existe toujours, qu'il n'y a pas d'erreur dans la balise  <img>. Si le le texte contenu dans la balise l'attribut alt d'affiche c'est qu'il y a un problème avec le chargement de l'image, si le chemin est bon et que le fichier existe toujours, il faudra donc vérifier que l'image n'est pas corrompu

