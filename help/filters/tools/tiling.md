---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/tools/tiling.html"
breadcrumb-title: ''
description: Utilisez l’outil Répétition de Substance 3D Sampler pour créer des motifs de répétition homogènes à partir de textures de surfaces de matériau répétables.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Tiling
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Répétition
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 0%

---


# Répétition

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-tiling-18-n-d.png)

Outils **In:**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Utilisez le **filtre de Répétition** pour rendre votre matériau assemblable. Le filtre **Juxtaposer** rend également votre matériau juxtaposable, mais chaque filtre fonctionne différemment. Si le **filtre Répétition** ne fonctionne pas pour vous, essayez le **filtre Juxtaposer**.

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Afficher le Seam** : activer/désactiver\
  Choisir d’afficher ou non le seam
* **Utiliser le masque** : activer/désactiver\
  Si cette option est activée, vous pouvez créer un masque personnalisé pour contrôler l’emplacement du seam
  * **Masque** : image/pinceau\
    Importez une image à utiliser comme masque ou utilisez le pinceau pour appliquer une peinture directement dans la **Vue 2D**

**Edge**

* **Détecter les contours** : activer/désactiver\
  Indiquez si les contours doivent être détectés en fonction des couches de matériau pour créer une transition plus organique entre les calques de matériau. Si cette option est activée, les paramètres supplémentaires suivants apparaissent :
  * **Utiliser le seuil par canal** : activer/désactiver\
    Si cette option est activée, des paramètres supplémentaires apparaissent pour ajuster le seuil de chaque couche individuellement.
    * **Base color du seuil** : 0-1
    * **Seuil normal** : 0-1
    * **Height du seuil** : 0-1
  * **Seuil** : 0-1\
    Ajustez la valeur de seuil utilisée pour rechercher le seam.
  * **Flou** : 0-1\
    Flouter la zone autour du seam
  * **Smoothness** : 0-2\
    Ajustez le smoothness du seam. Cela permet d’éviter les artefacts
  * **Résolution de Grille** : 1-11\
    Réglez la résolution de la grille sur laquelle le seam est dessiné. Une résolution inférieure peut améliorer les performances, mais diminuer la qualité du seam
  * **Utiliser la Base color** : activer/désactiver\
    Indiquer si les informations de base color sont prises en compte dans la génération du seam
  * **Utiliser la normale** : activer/désactiver\
    Indiquer si les informations normales sont prises en compte dans la génération du seam
  * **Utiliser l&#39;Height** : activer/désactiver\
    Indiquer si les informations sur l’height sont prises en compte dans la génération du seam
  * **Décalage de coupe** : 0-0,5\
    Réglage du décalage du seam sur les axes X et Y

**Paramètres avancés**

* **Transformer** : 0-2\
  Ajustez les valeurs de transforme de la matrice. Augmentez les valeurs X et W pour définir le degré de chevauchement entre le matériau sous-jacent et le sous-jacent.
* **Décalage** : 0-1\
  décaler le matériau sur les axes X et Y
* **Filtrage** :\
  Sélectionnez la méthode de filtrage à utiliser sur les pixels redimensionnés. Le filtrage bilinéaire applique un flou aux pixels, tandis que le filtrage le plus proche opère un lissage entre les pixels.
* **Taille d&#39;entrée** : 0-8192\
  Ajustez la taille de l’entrée en pixels sur les axes X et Y.

## Guide d’utilisation

Le **filtre de Répétition** fonctionne en deux étapes :

1. Il adapte et décale votre matériau pour générer un chevauchement.
1. Ensuite, il fait varier le bord qui se chevauche pour masquer le seam.

Ainsi, pour utiliser le **filtre de Répétition**, ces deux étapes du processus peuvent vous donner les meilleurs résultats.

1. Ajoutez le **filtre de Répétition** en haut de la pile de calques
1. Utilisez les poignées pour transformer le matériau afin qu’il y ait suffisamment de chevauchement pour masquer le seam.
   1. Il peut être utile de redimensionner le matériau pour créer un chevauchement, mais cela peut également entraîner une perte de détails.
1. Ajustez les paramètres dans la section **Edge** pour ajuster le seam.

Pour certains matériaux, l&#39;utilisation du **filtre de Répétition** seul entraînera toujours des artefacts ou des problèmes le long du seam. Dans ce cas, il est conseillé d&#39;utiliser d&#39;autres filtres tels que **Tampon de Clone** pour résoudre les problèmes de seam et de répétition.

Il est recommandé de travailler sur la répétition du matériau dès le début du processus de création du matériau. Dès qu&#39;un élément sans répétition est ajouté au matériau, assurez-vous qu&#39;il comporte des vignettes avant de continuer. Les filtres de Sampler sont conçus de manière à ne pas rompre les matériaux de répétition. Cela signifie qu’une fois les mosaïques de matériau sous-jacentes créées, vous pouvez continuer à travailler avec les filtres et les matériaux Sampler inclus, et votre matériau continuera à fonctionner avec ces mosaïques.
