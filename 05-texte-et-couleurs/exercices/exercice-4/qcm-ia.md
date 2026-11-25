### Exercice 4 — Vérifier la compréhension

**Objectif** : tester sa compréhension des propriétés utilisées, sans regarder la feuille CSS.
**Durée indicative** : 20 min



Prompt : 

Tu es mon tuteur CSS. Pose-moi une question à la fois sur : color, background-color,
font-family, font-size, font-weight, font-style, text-align, px/em/rem, contraste.
Attends ma réponse avant de corriger. Ne me donne pas la réponse avant que j'aie essayé.
Après 10 questions, fais un bilan de mes points faibles.



Question n° : 1
Réponse (avant correction) : Cette règle met les paragraphes de la page en rouge et le fond en noir
Correction de l'IA : Correct. `color` s'applique au **texte** (ici `#ff0000`, rouge pur) et `background-color` au **fond** (ici `#000000`, noir). C'est la règle `p` qui cible tous les paragraphes de la page.
Réponse initiale : juste
À retenir : color change la couleur du texte et background-color celle du fond



Question n° : 2
Réponse (avant correction) : La valeur "Poppins" est le nom de la police tandis que "sans sérif" permet de ne pas ajouter de sérifs dans la police, si la police "Poppins" n'est pas disponible sur l'ordinateur du visiteur le service de google, Google Fonts s'en charge
Correction de l'IA : Tu as bien compris la moitié.
Ce qui est juste : `"Poppins"` est le nom de la police, et `sans-serif` désigne une famille de polices sans empattements (sans "serifs").
Ce qui est faux : Google Fonts n'intervient pas tout seul. Il faut d'abord charger la police dans ta page, avec une balise `<link>` dans le `<head>` ou avec `@import` dans le CSS. Sans ça, le navigateur cherche "Poppins" sur l'ordinateur du visiteur. S'il ne la trouve pas, il passe à la valeur suivante de la liste, ici `sans-serif`. Cette deuxième valeur est donc une **police de secours** (*fallback*). Le navigateur prend alors la police sans empattements par défaut de l'appareil, par exemple Arial ou Helvetica.Réponse initiale : partiellement juste
À retenir : Il faut charger une police dans la page sinon le navigateur utilise la police de secours indiquée après



Question n° : 3
Réponse (avant correction) : Rem signifie que la taille est copiée sur la taille de <html>, par exemple si la taille par défaut est de 16px, la taille sera 1.5 x 16
Correction de l'IA : Bonne réponse sur le principe. `rem` (*root em*) est relatif à la taille de police de l'élément racine `<html>`. Le calcul est juste : 1,5 × 16 = **24px**. Ta formulation « copiée sur la taille de `<html>` » est un peu approximative. La taille est **multipliée** par le coefficient, pas copiée.
Tu n'as pas donné le résultat final en px, mais le calcul montre que tu l'as. Pense à toujours conclure par la valeur.Réponse initiale : Juste
À retenir : em multiplie la taille de police de html par le coefficient (1,5rem = 1,5 x 16px = 24px)



Question n° : 4
Réponse (avant correction) : La taille du paragraphe sera de la taille de .carte * 1.5, em se base sur les balises parents contrairement à rem
Correction de l'IA : Bonne réponse. `em` se base sur la taille de police de l'**élément parent**, alors que `rem` se base toujours sur la racine `<html>`. C'est la bonne différence.
Réponse initiale : juste
À retenir : Pour font-size, em se base sur la taille du parent alors que rem se base toujours sur html.



Question n° : 5
Réponse (avant correction) : Les titres h2 passent en gras et en italique, dans font-weight on peut aussi mettre une valeur comme 400 ou 100 par exemple
Correction de l'IA : Correct. `font-weight: bold` met le texte en gras et `font-style: italic` en italique. Pour `font-weight`, les valeurs numériques vont de 100 à 900 (par centaines). `400` correspond à `normal` et `700` à `bold`. `100` donne un texte très fin, si la police propose cette graisse. Sinon le navigateur utilise la graisse la plus proche. Tu peux aussi citer `normal`, `lighter` ou `bolder`.
Réponse initiale : juste
À retenir : Font-weight accepte bold ou des valeurs de 100 à 900 avec 400 = normal et 700 = bold



Question n° : 6
Réponse (avant correction) : Les autres valeurs possibles pour text-align sont left ainsi que right, text-align: center sur un élément div qui contient une image ne centre pas l'image car cette balise ne concerne que le texte
Correction de l'IA : Réponse à moitié juste.
**Les valeurs :** `left` et `right` sont bonnes. Il manque `justify`, qui étire le texte pour qu'il remplisse toute la largeur de la ligne. Tu peux aussi rencontrer `start` et `end`.
**L'image :** ici tu te trompes. `text-align` ne concerne pas que le texte. Il aligne tout le **contenu en ligne** (*inline*) d'un bloc, et une balise `<img>` est en ligne par défaut. Dans une `<div>` avec `text-align: center`, l'image **est donc centrée**. Ça ne marche plus si l'image est passée en `display: block`. Il faut alors `margin: 0 auto;` pour la centrer.
Réponse initiale : partiellement juste
À retenir : text-align aligne tout le contenu en ligne donc aussi les images et justify existe en plus de left, right et center



Question n° : 7
Réponse (avant correction) : Oui ce choix de couleur cause un problème d'accessibilité car cela donne seulement un score de 4.48 de ratio de contraste ce qui est bas, pour le régler il faut modifier la couleur du texte du bouton, par exemple avec #000000 le ratio de contraste passe a 21 ce qui est excellent
Correction de l'IA : Excellente réponse, et tes chiffres sont exacts : `#777777` sur blanc donne environ **4,48:1**, et `#000000` sur blanc donne **21:1**.
Tu n'as pas cité le seuil, et c'est lui qui rend le problème réel. Les règles WCAG niveau AA demandent **4,5:1** pour un texte normal et **3:1** pour un grand texte. Avec 4,48 tu échoues de justesse. Le niveau AAA demande 7:1. Le noir pur marche, mais il n'est pas obligatoire : un gris un peu plus foncé comme `#767676` ou `#595959` suffit et garde un rendu plus doux.
Réponse initiale : juste
À retenir : Le contraste doit atteindre au moins 4,5:1 pour un texte normal (3:1 pour un grand texte)



Question n° : 8
Réponse (avant correction) : On ne va pas voir le texte car la valeur red et la valeur rgb(255, 0, 0) représentent la même chose, ça sera donc du rouge sur du rouge, ça s'appelle un défaut de contraste
Correction de l'IA : Correct. `red` et `rgb(255, 0, 0)` donnent exactement la même couleur (`#ff0000`), donc le texte se confond avec le fond et devient invisible. Le ratio de contraste est de **1:1**, le minimum possible, très loin des 4,5:1 demandés.
Pour être plus précis, on parle de **contraste insuffisant** (ici, nul). Le terme « défaut de contraste » est compréhensible, mais le vocabulaire des normes d'accessibilité est « contraste insuffisant ».
Réponse initiale : juste
À retenir : Un texte de la même couleur que son fond donne un contraste de 1:1 donc un texte invisible.



Question n° : 9
Réponse (avant correction) : Dans ce cas 1em vaut 16px car 1 x 16 = 16, si on met font-size a 24px le padding vaudra 24px  car 1 x 24 = 24
Correction de l'IA : Correct : 1 × 16 = **16px**, puis 1 × 24 = **24px**.
Nuance à retenir : avec `em`, la référence change selon la propriété. Pour `font-size`, `em` se base sur la taille de police du **parent**, comme on l'a vu à la question 4. Pour les autres propriétés (`padding`, `margin`, `width`...), `em` se base sur la taille de police de **l'élément lui-même**. C'est pour ça que le `padding` suit ici le `font-size` de `.exemple`.
Réponse initiale : juste
À retenir : Hors font-size, em se base sur la taille de police de l'élément lui-même



Question n° : 10
Réponse (avant correction) : Le contraste est presque nul entre les deux couleurs, on peut par exemple mettre le fond en blanc, le texte est trop petit, on peut remplacer les 12px par 1rem ou 16px cela revient au même, il n'y a pas de police de secours et le texte justifié n'est pas idéal car celui-ci crée des espaces irréguliers entre les mots ce qui gène les personnes ayant du mal a distinguer les mots
Correction de l'IA : Tu as repéré les quatre problèmes.

- **Contraste :** `#333333` sur `#1a1a1a` donne un ratio d'environ 1,5:1, très loin des 4,5:1 demandés. Passer le fond en blanc marche. Tu pouvais aussi éclaircir le texte et garder le fond sombre.
- **Taille :** 12px est trop petit pour un texte courant. `1rem` vaut bien 16px par défaut, mais `rem` a un avantage sur `px` : il respecte la taille de police que le visiteur a choisie dans son navigateur.
- **Police de secours :** il faut écrire `font-family: Arial, sans-serif;`.
- **`justify` :** tu as bien expliqué les espaces irréguliers entre les mots. `text-align: left` est le bon choix pour un texte courant.

Réponse initiale : juste
À retenir : Un texte lisible demande un bon contraste, une taille d'au moins 16px (ou 1rem), une police de secours et un alignement à gauche plutôt que justifié



## Bilan : tes points faibles

Sur les 10 questions, 8 sont solides et 2 étaient à moitié justes (les questions 2 et 6).

**À retravailler**

1. **Le rôle de `font-family` (question 2).** Une police doit être chargée dans la page (`<link>` ou `@import`). Sinon le navigateur passe à la police de secours. Tu l'as bien appliqué à la question 10, donc c'est en bonne voie.
2. **Ce que couvre `text-align` (question 6).** Il aligne tout le contenu en ligne, pas seulement le texte, donc les `<img>` aussi. Tu as aussi oublié `justify` dans la liste des valeurs.
3. **Conclure tes calculs (questions 3 et 4).** Tu posais la formule sans donner le résultat en px. Pense à écrire la valeur finale