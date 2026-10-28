## Exercice 1 — Reconnaître et corriger des documents HTML

###### Document A

1. Il n'y a aucun problème de visible

2. Il y a plusieurs problèmes, tout d'abord la balise <head> se trouve à l'intérieur de la balise <body> alors que celle-ci doit se trouver au dessus de la balise <body>, le second problème est se trouve à la ligne 10, la balise <!DOCTYPE html> se trouve à la fin du code alors qu'elle devrait normalement se trouver tout en haut du code à la ligne 1, la balise <p> n'est pas fermé, il faut donc mettre </p> et enfin il manque la balise <html lang="fr"> pour définir la langue de la page

3. <!DOCTYPE html>
    <html>
      <head>
        <meta charset="UTF-8">
        <title>Réseau du BTS SIO</title>
      </head>
      <body>
          <h1>Bienvenue sur ma page</h1>
          <p>Je prépare un BTS SIO option SISR.</p>
      </body>
    </html>



###### Document B

1. Sur le page web nous pouvons voir que le titre qui se trouve dans l'onglet du navigateur n'est pas bon et que les caractères spéciaux de la page ne s'affichent pas correctement
2. Il y a plusieurs tout d'abord la balise de fermeture </body> se trouve en dehors de la balise <html>, il manque la balise <title> à l'intérieur de la balise <head>.

3. 

<!DOCTYPE html>
<html lang="fr">
    <head>
        <meta charset="UTF-8">
        <title>Page</title>
    </head>
    <body>
        <h1>Ma page</h1>
        <p>Élève de première année</p>
    </body>
</html>

