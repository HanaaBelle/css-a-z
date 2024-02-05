## CSS : Les piliers de ce langage 

    Le "CSS" est si spécial et présent partout sur le web car c'est le seul langage de style qu'on utilise pour styliser nos pages web (ce n'est pas un langage de programmation mais un langage de style) et ses concepts qu'il faut bien 
    métriser : 

    - La cascade : c'est appliquer du style aux éléments en fonction de l'apparition dans notre fichier "CSS" et s'il y a deux (2) sélécteurs de même force et de la même spécificité et bien celui qui est à la fin et qui est en bas de la cascade l'emporte sur l'autre donc on gardera son style
    
    - L'héritage: ça va être certaines propriétés notamment celles liées au texte comme (color, font size... etc) et bien elles vont être héritées de parents à enfants et donc ça a été créé pour faciliter le style et pour éviter certaines répétitions sans si ce sont des liens ou tout autre éléments qui ont déjà du style de base donné par le navigateur avec le "user agent stylesheet"
    
    - L'empilement des couches : c'est un concept qu'il faut absolument métriser car les éléments vont être empilés suivant plusieurs caractéristiques, des propriétés de positions, un z-index... etc et donc on va avoir un certains empilement qu'il faudra savoir gérer si on a envie de faire  des dispositions complexes ou moins complexes et du coup c'est important de bien comprendre ça 
    
    - La spécificité : c'est la force des sélecteurs qui peut aller au dessus de la force de cascade (c'est les sélecteurs de même sélection et c'est le dernier qui est fait qui va l'emporter sur l'autre mais seulement s'il est de la même spécificité) et donc les sélecteurs peuvent avoir une spécificité différente en fonction de quel sélecteur ils utilisent par exemple un "id", une "class", "pseudo élément", "pseudo class"... etc 
     
    - Le "CSSOM" : c'est plus de la théorie et plus du fonctionnement du navigateur qui va analyser notre code et va créer le "DOM" qui est le "document object model" c-à-d qu'il va transformer chaque élément de notre site en "objet" et même le DOM va au-delà de ça mais en gros chaque élément du site va être transformer en objet et pour le "CSSOM" ça veut dire qu'ici on va avoir un "objet" également par série de "style" si on a par exemple un "objet" pour un "titre" en JS on aura un "objet" pour tout le "style" qui lui est lié et c'est comme ça que le navigateur fonctionne en créant comme ça des object pour chaque élément 
    
    - Box Model (le modèle de boite) : chaque élément va être une boite avec du "contenu", du "padding", des "bordures" et des "marges", ces boites vont se comporter différement selon le type de "display" (block ou inline) donc soit le type de "display" par défaut, soit celui qu'on a rajouté nous-même car on peut bien sûr changer le type de "display" des éléments 
    
    - Flexbox / CSS Grid : sont deux (2) modules de positionnement où chaque module représente une série de propriétés et de concepts mises ensemble et donc tout ce qui est lié à "Flexbox" (dans la docummentation officiel c'est "module Flexbox" pareil pour "module CSS Grid" aussi aux "module animations"... etc) ça permet de bien positionner des éléments comme on veut et de faire des dispositions complexes et responsives et c'est très intéressant

## Bonnes pratiques : 

    - Code facile à comprendre : en évitant des sélecteurs trop compliqués et des propriétés pas très judicieuses
    Et aussi faire en sorte de bien regrouper les différents sélecteurs et les différentes régles du "CSS" en fonction des sections 
    qu'on a... etc   

    - Maintenable, lisible, réutilisable : c'est important de pouvoir modifier facilement certaines choses sans que ça explose

    - Nommage, architecture : il y a différents types de nommage le "kebab case" suivant les projets et les équipes suivant les différents environnement de travail on peut avoit plusieurs types de nommage et donc il faut respecter tout ça et c'est pareil pour l'architecture des fichiers il faut que ça soit judicieux

    - Réactivité : ça concerne le "responsive" qui est la façon dont les sites vont s'adapter à tous les écrans et pour celà on a les

    - Media queries : suivant la largeur de l'écran on peut faire certaines choses comme on applique certaines régles "CSS" 

    - Unités de mesure (%, rem, vh, vw...) : qui sont relatives le plus souvent qui vont permettre de s'adapter plus facilement

    - Medias : gérer les images et les vdéos et les adapter à tous les écrans

    - Texte : gérer le texte et l'adapter aux différents écrans aussi (rendre le texte plus petits pour les petits écrans qu'en grand écran)

    - Performances : en évitant la répétition et d'avoir un code assez concis de manière général et de bien faire les animations (c'est là où on peut se tromper) et là on a 
    
    - Animations optimisées : en utilisant les bonnes propriétés et bien les animées aussi faire des calculs et des audits des performances pour voir si ça se passe bien ou pas

    - Compresser son code : dès qu'on finit notre code on le compresse afin d'enlever tous les espaces qu'il y a entre les différents 
    morceaux de codes et ça permet d'avoir des fichiers plus légers tout simplement

    - Eviter les surcharges d'appels bloquants : lorsque notre navigateur va télécharger les fichiers pour faire fonctionner notre site comme un fichier CSS, on peut mettre des attribut qui vont précharger (comme la police d'écriture avec google font on a des link préconnect) et bien ça évite la surcharge 
    
    - Utiliser de bons attribus

    - Utiliser un préprocesseurs "CSS" pour coder plus facilement et rapidement : ce sont des fonctionnalités rajoutées en utilisant un préprocesseur et puis ça se fait compiler en CSS classique