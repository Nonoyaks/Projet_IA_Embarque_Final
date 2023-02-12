# Projet_IA_Embarque_Final
IA embarqué détection cancer de la peau


## Données ;

Choix du dataset : le dataset utilisé est celui obtenu sur le site : https://www.kaggle.com/datasets/fanconic/skin-cancer-malignant-vs-benign
Le dataset est disponible sur ce Repository. Ce choix fut fait car le nombre d'images est intéressant sans être trop élevé. De plus, le nombre d'avis positif pour ce dataset est suffisament élevé pour qu'il puisse être jugé pertinent.

## Appareil :

Nous pensions utiliser la caméra fournie avec le kit TinyML Arduino 33 BLE Sense. Cependant, nous n'avons pas réussi à modifier la distance focale de la caméra, les couleurs ne reflètent pas la réalité et les images ne sont clairement pas d'une qualité semblable à celle utilisée par le dataset.

Nous avons donc choisi d'utiliser les photos de notre téléphone portable pour tester notre modèle.

## Design :

Le Design du modèle s'est fait en considérant le peu de mémoire RAM de la carte Arduino Nano 33 BLE Sense (256kB). Nous avons donc fait le choix de prendre de petites images pour réduire au maximum la taille du modèle à charger sur la carte. Soit des images 32x32.

## Deployment :

Concernant le déploiment du modèle, nous l'avons réalisé suivant 3 types différents :

1. Flash.bat à transférer sur la carte Arduino ;
2. Programme.ino à transférer sur la carte Arduino ;
3. Programme.py à utiliser sur OpenMV IDE.
