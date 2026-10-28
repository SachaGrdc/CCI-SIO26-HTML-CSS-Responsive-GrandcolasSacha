# Exercice 3 — Corriger une hiérarchie de titres et choisir les bonnes balises



1. Extrait A : On passe d'une balise <h1> à une balise <h3> sans passer par une balise <h2>

   Correction proposée : 

   ```
   <h1>Les réseaux</h1>
   <h2>Le modèle OSI</h2>
   <h2>Le modèle TCP/IP</h2>
   ```

​	

​	Extrait B : Il y a 3 balises <h1> alors qu'il est recommandé de ne pas avoir plusieurs balises <h1> dans une même page

​	Correction proposée :
```html
<h1>Guide du technicien</h1>
<h2>Installation</h2>
<h2>Configuration</h2>
```

​	

​	Extrait C : La page commence avec un <h2> alors qu'il faut utiliser une <h1>, on passe aussi de <h2> à <h4> sans passer par 	<h3>, de plus les balises sont dans le mauvais ordre

​	Correction proposée : 

```html
<h1>Sauvegardes</h1>
<h2>Sauvegarde complète</h2>
<h2>Sauvegarde incrémentale</h2>
<h2>Conclusion</h2>
```



​	Extrait D : La balise <h2> se trouve dans une balise <p> ce qui n'est pas possible

​	Correction proposée : 

```
<h1>Serveur DNS</h1>
<h2>Rôle du serveur</h2>
<p>Il traduit les noms de domaine en adresses IP.</p>
```



​	Extrait E : La balise <h2> n'est pas un titre, il vaut mieux la remplacer par une balise <p>, de plus cette phrase est importante c'est pourquoi il vaut mieux la mettre en gras

​	Correction proposée : 

```
<h1>Procédure de mise à jour</h1>
<p><strong>Attention : ne pas éteindre le serveur pendant la mise à jour</strong></p>
<ol>
  <li>Lancer la mise à jour.</li>
  <li>Attendre la fin du traitement.</li>
</ol>
```



2.  S1 : On peut utiliser la balise <ol> pour numéroter les étapes de la configuration

   S2 : On peut utiliser la balise <ul> pour énumérer sans ordre particulier

   S3 : On peut utiliser la balise <strong> pour mettre en évidence la phrase

   S4 : On peut utiliser la balise <em> pour insister sur ce mot
