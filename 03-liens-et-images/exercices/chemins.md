### Exercice 2 — Corriger des chemins

**Objectif** : lire une arborescence et retrouver les chemins corrects.
**Durée indicative** : 30 min



```html
<link rel="stylesheet" href="../css/style.css"> <!-- il ne faut pas mettre deux ../ devant le dossier css car cela signifie que qu'on remonte d'un dossier, le bon chemin est "css/style.css" -->
<img src="img/Logo.png" alt="Logo du club"> <!-- Le chemin est bon mais le L de Logo.png est en majuscule alors que dans l'arborescence il est en minuscule, le bon chemin est "img/logo.png" -->
<a href="pages\contact.html">Contact</a> <!-- Le chemin n'est pas bon car il utilise un \ alors qu'il faut utiliser un / -->
<a href="doc/plaquette.pdf">Plaquette</a> <!-- Il y a un erreur dans le chemin, le dossier est nommé doc dans le chemin alors que dans l'arborescence il est nommé docs, le bon chemin est "docs/plaquette.pdf" -->
```



```html
<link rel="stylesheet" href="css/style.css"> <!-- Le chemin n'est pas bon, la page contact.html se trouve dans le dossier pages, or le fichier cible se trouve dans le dossier css donc il faut revenir en arrière, voici le bon chemin : "../css/style.css" -->
<a href="index.html">Accueil</a> <!-- Même chose sauf que cette fois le fichier index.html se trouve à la racine, le bon chemin est donc "../index.html" -->
<img src="../img/photos/equipe.jpeg" alt="L'équipe du club"> <!-- Il y a un erreur dans l'image equipe, le bon format de l'image est le .jpg, le bon chemin est donc "../img/photos/equipe.jpg -->
```



```html
<a href="contact.html">Nous contacter</a> <!-- Le chemin n'est pas bon, la page reseau.html se trouve dans le dossier pages puis dans le dossier services, or le fichier cible se trouve dans le dossier pages donc il faut revenir en arrière, voici le bon chemin : "../contact.html" -->
<img src="../img/icones/mail.svg" alt=""> <!-- Le chemin n'est pas bon, la page reseau.html se trouve dans le dossier pages puis dans le dossier services, or le fichier cible se trouve dans le dossier img puis icones donc il faut revenir en arrière, voici le bon chemin : "../../img/icones/mail.svg" -->
```



| Fichier                         | Ligne fautive                                                | Ligne corrigée                                               | Explication                                                  |
| ------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| site/index.html                 | `<link rel="stylesheet" href="../css/style.css">`            | `<link rel="stylesheet" href="css/style.css">`               | `index.html` est à la racine, donc `css/` est dans son propre dossier et le `../` sort du site. |
| site/index.html                 | `<img src="img/Logo.png" alt="Logo du club">`                | `<img src="img/logo.png" alt="Logo du club">`                | Le fichier s'appelle `logo.png` en minuscule, et la casse compte. |
| site/index.html                 | `<a href="pages\contact.html">Contact</a>`                   | `<a href="pages/contact.html">Contact</a>`                   | Dans une URL, le séparateur est `/` et non `\`.              |
| site/index.html                 | `<a href="doc/plaquette.pdf">Plaquette</a>`                  | `<a href="docs/plaquette.pdf">Plaquette</a>`                 | Le dossier s'appelle `docs`, avec un « s ».                  |
| site/pages/contact.html         | `<link rel="stylesheet" href="css/style.css">`               | `<link rel="stylesheet" href="../css/style.css">`            | `contact.html` est dans `pages/`, il faut remonter d'un dossier pour atteindre `css/`. |
| site/pages/contact.html         | `<a href="index.html">Accueil</a>`                           | `<a href="../index.html">Accueil</a>`                        | `index.html` est à la racine, un niveau au-dessus de `pages/`. |
| site/pages/contact.html         | `<img src="../img/photos/equipe.jpeg" alt="L'équipe du club">` | `<img src="../img/photos/equipe.jpg" alt="L'équipe du club">` | Le chemin est bon, mais l'extension du fichier est `.jpg` et non `.jpeg`. |
| site/pages/services/reseau.html | `<a href="contact.html">Nous contacter</a>`                  | `<a href="../contact.html">Nous contacter</a>`               | `contact.html` est dans `pages/`, un niveau au-dessus de `services/`. |
| site/pages/services/reseau.html | `<img src="../img/icones/mail.svg" alt="">`                  | `<img src="../../img/icones/mail.svg" alt="">`               | `reseau.html` est à deux niveaux de la racine, il faut donc remonter deux fois pour atteindre `img/`. |
