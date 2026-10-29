# Séance 3 — Les liens, les images et les chemins d'accès

*Fiche étudiant — 3 h — méthode : [annexe A](../12.%20-%20Annexes/A-consignes-etudiants.md)*

**Objectif général :** comprendre comment intégrer des ressources dans un document HTML et assurer leur accessibilité.



## Recherche autonome assistée par l'IA (35 min)

- Comment fonctionne un lien hypertexte ?
- Quelle différence existe-t-il entre un chemin relatif et une URL absolue ?
- Comment fonctionne un lien vers une ancre ?
- À quoi sert l'attribut `alt` ?
- Comment diagnostiquer une image qui ne s'affiche pas ?



1) Un lien hypertexte fonctionne avec la balise <a>, il utilise ensuite l'attribut href pour contenir la destination puis le navigateur lit le lien qui est contenu dans href et redirige vers la page indiqué.

2) L'URL absolue donne l'adresse complète, elle sert donc généralement à pointer vers un autre site internet mais elle fonctionne n'importe où, y compris dans un même site interne.

   Le chemin relatif lui indique l'emplacement d'un fichier par rapport à la page actuelle, c'est-à-dire que si on met le nom d'un fichier qui est dans le même dossier, ou alors le même dossier parent ça va marcher mais si on déplace le fichier et qu'on ne met pas à jour le chemin, le lien ne fonctionnera plus comparé à l'URL absolue. Le chemin relatif sert uniquement à pointer vers une page d'un même site internet.

3. Pour faire fonctionner un lien vers une ancre il faut tout d'abord donner un id unique à un élément (section, article etc....), dans l'attribut href on met aussi un # suivi de l'id qu'on a donné à notre élément puis lorsqu'on clic dessus la page défile automatiquement jusqu'à l'élément.
4. L'attribut alt sert à donner une description d'une image, il va être lu par les lecteurs d'écran et s'afficher lorsque l'image ne charge pas
5. Il faut tout d'abord vérifier que le chemin de l'image est bon, que l'image existe toujours, qu'il n'y a pas d'erreur dans la balise  <img>. Si le le texte contenu dans la balise l'attribut alt d'affiche c'est qu'il y a un problème avec le chargement de l'image, si le chemin est bon et que le fichier existe toujours, il faudra donc vérifier que l'image n'est pas corrompu