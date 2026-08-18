---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/wear-and-finish/scratch.html"
breadcrumb-title: ''
description: Utilisez le filtre de rayure de Substance 3D Sampler pour ajouter des rayures réalistes et des effets d’endommagement de la surface à vos matériaux.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Wear and Finish > Scratch
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gratter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---


# Gratter

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-scratches-18-n-d.png)

**Entrée :** usure et finition

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Ajoutez des rayures et de l&#39;usure à votre matériau.

*Avant et après l’application du **filtre de travail**.*

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0001-scratch-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0000-scratch-out.jpg){width="200px"}

</td>
</tr>
</table>

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Générateur aléatoire** :\
  La valeur de départ aléatoire détermine les valeurs aléatoires des autres paramètres qui utilisent le caractère aléatoire dans ce filtre.
* **Gratter** : activer/désactiver\
  Activez ou désactivez les rayures. Si cette option est activée, la section **Gratter** s&#39;affiche.
* **Puce** : basculer\
  Ajoutez un effet d&#39;écaillage à la surface. Si cette option est activée, la section **Puce** s&#39;affiche.
* **Micro-rayure** : basculer\
  Ajoutez des micro-rayures à la surface. Si cette option est activée, la section **Micro-rayure** s&#39;affiche.

**Gratter**

**Paramètres de base > Rayure** doit être activé pour que cette section apparaisse.

* **Quantité** : 0-1\
  Contrôlez le nombre de rayures qui apparaissent.
* **Intensité** : 0-1\
  Réglez la profondeur et l’intensité des rayures.
* **Échelle** : 1-4\
  Modifiez la taille des rayures. Augmentez cette valeur pour réduire la taille de la zone de travail.

**Puce**

**Paramètres de base > Rayure** doit être activé pour que cette section apparaisse.

* **Quantité** : 0-1\
  Contrôlez le nombre de puces qui apparaissent.
* **Intensité** : 0-1\
  Réglez la profondeur et la force des puces.
* **Échelle** : 1-4\
  Modifiez la taille des puces. Augmentez cette valeur pour réduire la taille de la puce.

**Micro-rayure**

* **Quantité** : 0-1\
  Contrôlez le nombre de micro-rayures qui apparaissent.
* **Intensité** : 0-1\
  Réglez la profondeur et l’intensité des micro-rayures.
* **Rotation** : 0-1\
  Faites pivoter les micro-rayures.
* **Rotation Aléatoire** : 0-1\
  Faites varier la rotation des micro-rayures de manière aléatoire.
* **Échelle** : 0-2\
  Réglez la taille des micro-rayures. Augmentez la valeur de ce curseur pour augmenter la taille des micro-rayures.
* **Échelle aléatoire** : 0-1\
  Faites varier l’échelle des micro-rayures de manière aléatoire.
* **Largeur** : 0-1\
  Contrôle de la largeur des rayures
* **Width Random** : 0-1\
  Faites varier la largeur des micro-rayures de manière aléatoire.
* **Distorsion** : 0-1\
  Ajoutez de la distorsion aux rayures pour rompre l’uniformité.
* **Distorsion aléatoire** : 0-1\
  Contrôlez le caractère aléatoire de l’effet de distorsion.
* **Fréquence de Distorsion** : 0-1\
  Contrôlez l’échelle de fréquence de l’effet distorsion.

**Masquer**

* **Masque personnalisé** : activer/désactiver\
  Activez ou désactivez l’utilisation d’un masque personnalisé. Si cette option est activée, les paramètres suivants apparaissent :
  * **Masque** : image/pinceau\
    Sélectionnez une image à utiliser comme masque ou utilisez le pinceau pour peindre un masque personnalisé directement dans la vue 2D.
  * **Masque personnalisé - Flou** : 0-1\
    Floutez le masque.
  * **Masque personnalisé - Inverser** : activer/désactiver\
    Inversez le masque.

**Paramètres avancés**

* **Opacité Globale** : 0-1\
  Réglez l&#39;opacité de l&#39;effet **Filtre de travail**.
* **Couleur de base** : activer/désactiver\
  Indique si la couche de couleur de base est affectée par le filtre. Si cette option est activée, une commande supplémentaire apparaît :
  * **Couleur de base - Couleur** : sélection de la couleur\
    Sélectionnez la couleur de base des rayures et des copeaux.
* **Métallique** : activer/désactiver\
  Indiquez si le canal métallique est affecté par le filtre. Si cette option est activée, une commande supplémentaire apparaît :
  * **Valeur Métallique** : 0-1\
    Réglez la valeur métallique des zones rayées.
* **Rugosité** : activer/désactiver\
  Définissez si la couche de rugosité est affectée par le filtre. Si cette option est activée, une commande supplémentaire apparaît :
  * **Rugosité - Valeur** : 0-1\
    Réglez la valeur de rugosité des zones rayées.
* **Normal** : activer/désactiver\
  Indique si le canal normal est affecté par le filtre. Si cette option est activée, des commandes supplémentaires s’affichent :
  * **Normal - Intensité** : -1 à 1\
    Réglez l’intensité des normales.
  * **Normal -** **Aplatir** :\
    Diminuez cette valeur pour aplatir les normales.
* **Height** : activer/désactiver\
  Définissez si le canal d’height est affecté par le filtre. Si cette option est activée, une commande supplémentaire apparaît :
  * **Height - Intensité** : 0-1\
    Réglez le contraste de la courbe d’height.
* **Émissif** : activer/désactiver\
  Définissez si le canal émissif est affecté par le filtre. Si cette option est activée, une commande supplémentaire apparaît :
  * **Émissif - Couleur** : sélection de couleur\
    Définissez la couleur du canal émissif.
* **Specular level** : activer/désactiver\
  Détermine si la couche de specular level est affectée par le filtre. Si cette option est activée, une commande supplémentaire apparaît :
  * **Specular level** **- Valeur** : 0-1\
    Réglez la valeur de la couche de specular.
* **Occlusion ambiante** : activer/désactiver\
  Définissez si le canal d’occlusion ambiante est affecté par le filtre. Si cette option est activée, les commandes supplémentaires suivantes apparaissent :
  * **Occlusion ambiante - Intensité** : 0-1\
    Réglez l’intensité de l’AO généré.
  * **Occlusion ambiante** **- Rayon** : 0-1\
    Réglez le rayon de l’effet AOP.
* **Opacité** : activer/désactiver\
  Définissez si la couche d’opacité est affectée par le filtre. Si cette option est activée, une commande supplémentaire apparaît :
  * **Opacité - Valeur** : 0-1\
    Modifiez l’opacité du matériau.
