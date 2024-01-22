# The Artbox project

## Étape 1 : Préparez votre travail

Avant de commencer le développement, il est important de commencer par comprendre le fonctionnement du site actuel, disponible sur ce repository envoyé par votre cliente.

### Recommandations

- Commencez par installer votre environnement de développement comme vu dans le cours, avec VSCode et MAMP, ou XAMP.
- Puis téléchargez le site envoyé par la cliente, ouvrez-le dans votre navigateur et dans votre IDE. Prenez bien le temps de regarder les différents fichiers. Vous verrez que du code est dupliqué entre les fichiers (le contenu et la structure) ainsi qu’au sein du fichier de la page d’accueil.

## Étape 2 : Factorisez le header et le footer

Maintenant que vous avez pris le temps de découvrir le code actuel, il est temps de l’améliorer ! Vous avez probablement remarqué que le code du header et du footer étaient présents sur chacune des pages.

Imaginez que vous souhaitiez modifier le contenu de ces éléments… Il faudrait alors effectuer cette modification pour chaque page, soit 16 fois !

### Recommandations

Vous savez maintenant utiliser la fonction include ? Utilisez-la sur le projet ! Deux étapes pour cela :

1. Créez les fichiers header.php et footer.php en y mettant respectivement le code HTML du header et du footer.
2. Remplacez le code du header et du footer par deux include, vers les fichiers fraîchement créés. Pensez à remplacer l’extension de tous les fichiers HTML par “.php” afin qu’ils soient lus par PHP.

Une fois ces changements effectués, vous serez capable de modifier le header ou le footer en une seule fois, et vos changements apparaîtront sur toutes les pages.

Vous y êtes arrivé ? Bravo ! Améliorons maintenant la gestion des œuvres !

#### changements effectués uniquement sur oeuvre-1.php : la suite du projet nous amenera à réduire le nombre de fichier oeuvre à un seul.
