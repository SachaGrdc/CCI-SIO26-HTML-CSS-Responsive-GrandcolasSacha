Dans un document HTML5, le code commence par <!DOCTYPE html> afin de définir le document comme de l'HTML pour le navigateur puis on utilise la balise <html lang="fr"> pour définir que le document est en langue française, c'est utile pour le navigateur, le moteur de recherche ainsi que les outils de traductions.

Après cela nous devons mettre la balise <head> qui regroupe toutes les métadonnées de la page tel que le nom de la page (dans l'onglet) , <meta charset="UTF-8"> pour définir l'encodage de la page , <link> afin de lier des pages CSS ou encore <script> pour lier des pages JavaScript.

Pour finir la balise <body> sert à contenir tout le contenu visible dans la page avec des balises tel que <p> pour faire un paragraphe ou encore <h1> pour pouvoir faire des titres. Elle inclue aussi des balises tel que <sections> ou encore <div> pour structurer son code.

HTML sert à structurer la page et à mettre du contenu. CCS sert à mettre en forme l'apparence de la page et JavaScript sert à apporter de l'interactivité via des animations par exemple.

Le navigateur lit le code pour construire le DOM, cela signifie que ça transforme le code en arborescence d'objets et les balises en noeud, il charge les fichiers liés tel que le CSS, les images ou encore le JavaScript puis pour finir il l'affiche à l'écran.

Voici un le code de base d'une page HTML : 

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
</body>
</html>

