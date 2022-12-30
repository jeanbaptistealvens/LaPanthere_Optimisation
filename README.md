# LaPanthere
 Optimisez un site web existant

Pour information
    - L’outil d’audit utilisé pour améliorer les performances techniques, l’accessibilité, les meilleurs démarches et le CEO  du site La Panthère, agence webdesign est LightHouse. 
    - Etant donné que les parts de marché des moteurs de recherche en France sont très largement dominées par Google avec ses 92%. Il est donc avantageux d’utiliser cet outil crée par Google afin d’obtenir des meilleurs suggestions pour plaire aux robots Google et d’atteindre une meilleure positionnement lors d’une recherche.
    - Les diagnostics et les actions méthodologiques réalisées regroupent les pages d’accueil et contact. 
    - Des captures d’écrans des actions méthodologiques réalisées après chaque  modifications est prise afin de mieux cibler son amélioration.
    - Le site est hébergé sur Github.com.

Pour réduire la consommation de la bande passante et améliorer le temps de chargement de la page afin d'atteindre 100% de performance dans les pages d’accueil et contact :
    
    Les fichiers scripts (JS) et les images se chargent de façon différer et asynchroniser
        Pour cela, j’ai ajouté des attributs "defer" et "async" pour les fichiers javascripts et les images des attributs "lazy" et "async"
        pour optimiser leurs chargements
    
    Les images (jpg, png ou bmp) sont dans des formats nouvelle génération (webp)
        Pour cela, j’ai lié des images webp pour optimiser leurs chargements

    Les fichiers scripts, styles (CSS) et les images (les images webp) sont plus légères
        Pour cela, j’ai lié des fichiers JS, CSS et photos minifiés, après leurs compressions en ligne pour optimiser leurs chargements

    Les textes utilisant la police s’affichent immédiatement
        Pour cela, j’ai inserer dans la partie @font-face l'attribut font-display: swap dans les feuilles de style bootstrap-min.css, et-line-min.css, font-awesome-min.css afin de spécifier que le texte utilisant la police doit être affiché immédiatement en utilisant une police système pour optimiser leurs chargements

Pour augmenter à 100% l'expérience des utilisateurs de technologies d'assistance :

    Les couleurs d'arrière-plan et de premier plan ont un rapport de contraste suffisant 
        Pour cela, j’ai rectifié les éléments de texte dans leurs feuilles de styles par un contraste de couleur suffisant à l’aide d’un outil d’analyseur de contraste des couleurs en ligne

    Les balises sémantiques sont suffisant et les liens ont un nom discernable 
        Pour cela, j’ai structuré les codes html en ajoutant la balise sémantique header/main et j’ai remplacé toutes les balises div incluant des titre par des balises sémantiques section et, j’ai discerné les liens grâce à l’attribut aria-label permettant une alternative textuelle à ces liens qui n'a pas de texte visible à l'écrans 

    Les éléments d'en-tête apparaissent dans un ordre séquentiel décroissant 
        Pour cela, j’ai fais en sorte que les  textes doivent être organisés par thème et titrés de manière logique en suivant la chronologie des balises h1, h2, h3. C'est à dire dans la partie du <!-bloc-1-presentation-> fait office de h1, dans le <!-bloc-2-services-> fait office de h2, dans la partie <!-bloc-2-services-> jusqu’à <!-- bloc-4-portfolio END --> fait office de h3 

Pour atteindre 92% des meilleurs pratiques dans les pages d’accueil et contact afin de réduire la pénalité de blacklist par les moteurs de recherches à cause de son contenu non conforme:
        
     Les images  de la page accueil  sont adaptées pour une utilisation optimales pour des appareils mobiles
        Pour  cela, j’ai ajouté la balise Picture et proposer des images peu gourmandes en ressources

    Les attributs width et height pour des dimensionnements optimales des images de la page accueil sont présents
        Pour cela, j’ai ajouté des attributs width et heigh pour avoir des dimensionnements optimales concernant les images

    La page contact présente des textes visibles qui sont orienter au centre sur l’image
        Pour cela, j’ai modifié cet éléments par un changement de la couleur dans la feuille de style style-min.css et aligner au centre  dans la feuille de style bootstrap-min.css 

Pour optimiser à 100% le positionnement du site web dans la page de résultats sur les moteur de recherche:

    Les liens cliquables dans les SERP (c-a-d les liens présentent dans les resulats de recherches) des moteurs de recherche ne sont pas référenciés, ne disposent pas des mots clés pertinents et aucune interprétation linguistique française
        Pour cela, j’ai spécifié que la page web doit être interpréter en langue française, j’ai ajouté des contenus descriptifs et j'ai modifié les mots clés pour qu'ils soient + pertinents en relation à l’activité du site web

    Les liens URL de footer obsolètes et certains qui ne correspondent pas à la nature de l’activité du site web sont supprimés
        Pour cela, j’ai supprimé les liens URL qui  apparaissent en effet comme des techniques trompeuses (cloaking), causant  des pénalités de blacklist par les moteurs de recherches

    La dissimulation de 3"keywords" dans les divs de la page d’accueil sont également supprimés 
        Pour cela, j’ai également  supprimés tous les "keywords" dissimulés dans les divs dans cette page, causant des pénalités de blacklist par les moteurs de recherches

    La balise p est augmenté à au moins 12px  présentant ainsi une taille de police de caractères conforme
        Pour cela, j’ai augmenté la taille de la balise p dans la feuille de style style-min.css à au moins 12px présentant ainsi une taille police de caractères conforme
