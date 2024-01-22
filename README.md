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

## Étape 3 : Créez le tableau des œuvres

Le site a maintenant un header et un footer “factorisés”. Il est temps de passer au code des œuvres.

Vous avez probablement remarqué que chaque œuvre était décrite deux fois dans le code : une fois dans la page d’accueil, une fois dans la page de détail de l’œuvre. Changer une œuvre implique donc de faire la modification deux fois. L’objectif va donc être de centraliser les œuvres dans un tableau PHP, qui sera beaucoup plus simple à maintenir.

### Recommandations

Une fois la notion de tableau bien comprise, vous pouvez mettre en place le tableau des œuvres. Pour cela :

- créez un fichier oeuvres.php ;
- dans ce fichier, créez un tableau PHP qui contiendra les 15 œuvres de la galerie. Vous vous servirez de ce tableau dans les étapes suivantes.

Pour vous aider :

- identifiez bien les informations de chaque œuvre sur le site ;
- vous aurez également besoin d’un identifiant d’œuvre (numéro de 1 à 15) pour pouvoir générer le lien vers les différentes œuvres par la suite ;
- l’idée est de regrouper toutes les œuvres dans un tableau. Chaque œuvre sera elle-même représentée par un tableau associatif qui regroupera les informations importantes de l'œuvre (titre, description, image...). Vous aurez donc une variable du type tableau contenant des tableaux.

Une fois cette étape terminée, vous devriez avoir un tableau avec toutes les œuvres pleinement utilisable pour les prochaines étapes !

## Étape 4 : Factorisez la page d’accueil

Maintenant que votre tableau est prêt, vous allez pouvoir l’utiliser sur la page d’accueil. En effet, vous avez peut-être remarqué que le code de la vignette représentant une œuvre est écrit 15 fois. Seuls l’image et le texte varient d’une vignette à une autre.

Ceci est problématique : si vous devez faire une modification sur le format de la vignette, vous devrez faire ce changement 15 fois !

### Recommandations

Comme vous l’avez peut-être compris, pour factoriser l’affichage des vignettes, vous allez devoir mettre en place une boucle dans votre page d’accueil afin de :

- parcourir votre tableau d’œuvres créé à l’étape précédente ;
- répéter automatiquement le code d’une vignette pour chacune de ces œuvres.

Pour vous aider dans votre tâche :

1. Identifiez bien le code répété pour chaque vignette.
2. Insérez, dans votre boucle, le code HTML répété.
3. Remplacez le contenu qui doit changer d’une œuvre à l’autre par les variables correspondantes, que vous afficherez en utilisant la fonction “echo”.

Votre boucle est mise en place ? Félicitations, votre page d’accueil est maintenant complètement factorisée et terminée ! Si vous avez besoin de modifier le format des vignettes, vous n’aurez à faire le changement qu’une seule fois au lieu de 15. Félicitations !
