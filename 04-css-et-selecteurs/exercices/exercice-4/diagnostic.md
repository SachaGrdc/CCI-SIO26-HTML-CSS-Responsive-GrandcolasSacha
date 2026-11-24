1. Rien ne s'affiche avec du style
  Symptome : La page est toute blanche et noire sans aucun style CSS.
  Cause : Dans index.html le lien vers le CSS est href="styles.css" alors que le fichier s'appelle style.css sans s et qu'il est dans le dossier css
  Correction : J'ai mis href="css/style.css" dans index.html
  Verification : En rechargeant la page, style.css charge bien maintenant

  

2. Le titre n'est pas en grand
  Symptome : Le titre h1 Tableau de bord reste à sa taille de base
  Cause : Dans le CSS il y a .titre-page avec un point alors que dans le HTML c'est un id (id="titre-page")
  Correction : J'ai changé .titre-page en #titre-page dans style.css
  Verification : Dans l'inspecteur sur le h1 on voit bien font-size 2.5rem qui s'applique

  

3. L'alerte n'est pas rouge ni en gras
  Symptome : Le texte Serveur indisponible reste noir et pas gras
  Cause : Il manque un point-virgule après color: red donc ça casse la ligne d'après
  Correction : J'ai rajouté le point-virgule après color: red;.
  Verification : Dans l'inspecteur sur p.alerte les deux lignes sont bien actives et il n'y a plus d'erreur

  

4. Le message info n'est pas vert
  Symptome : Le texte Sauvegarde terminée reste noir
  Cause : Dans le CSS c'est écrit colour avec un u au lieu de color
  Correction : J'ai remplacé colour par color
  Verification : Dans l'inspecteur la propriété n'est plus barrée et le texte est bien vert

  

5. Le service DHCP est gris au lieu de vert
  Symptome : Tous les services de la liste sont gris même celui qui a la classe actif
  Cause : Le sélecteur .liste-services li est plus fort que .actif tout seul donc il passe par dessus
  Correction : J'ai mis .liste-services .actif dans le CSS pour qu'il soit plus précis
  Verification : Dans l'inspecteur sur le li actif le vert s'applique bien et le gris est barré

  

6. Le lien aide n'est pas agrandi
  Symptome : Le lien reste petit
  Cause : Il y a un espace entre 1.2 et rem dans font-size: 1.2 rem; donc le navigateur comprend pas
  Correction : J'ai enlevé l'espace pour écrire font-size: 1.2rem;
  Verification : Dans l'inspecteur le lien passe bien à 1.2rem (19.2px)