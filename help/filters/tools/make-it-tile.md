---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/tools/make-it-tile.html"
breadcrumb-title: ''
description: Utilisez l’outil Juxtaposer dans Substance 3D Sampler pour créer automatiquement des motifs de répétition homogènes à partir de textures autres que de répétition.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Make it Tile
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Création d’une mosaïque
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---


# Création d’une mosaïque

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-tiling-18-n-d.png)

Générateurs De **Entrée :**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Utilisez le filtre **Création de mosaïque** pour rendre votre matériau assemblable. Le **filtre de Répétition** rend également votre matériau regroupable, mais chaque filtre fonctionne différemment. Si vous constatez que le **filtre Juxtaposer** ne fonctionne pas, essayez le **filtre Répétition**.

Dans les images ci-dessous, vous pouvez voir comment le filtre **Création d&#39;un matériau** peut convertir un matériau sans répétition en mosaïque. Ce matériau fonctionne bien car il suit un motif de type grille et il n’y a pas de points spécifiques qui attirent l’attention.

![](../../assets/3d-2d-filters-cropped-0015-make-it-tile-in.jpg)

Dans l’image ci-dessus, la ligne rouge indique la limite du matériau. Il est très clair qu&#39;il y a un seam fort, et que ce matériau ne fait pas de carreaux.

![](../../assets/3d-2d-filters-cropped-0014-make-it-tile-out.jpg)

Après **Création de mosaïque**, ce matériau présente une bonne mosaïque et sans la ligne rouge, il serait impossible de voir les seams aux limites du matériau.

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Seuil** : 0-1\
  Ajustez la taille et la correspondance du calque supérieur.
* **Smoothness** : 0-1\
  Lissez le seam du calque supérieur.
* **Contraste** : 0-1\
  Réglez le contraste du seam. Réduire le contraste a le même effet que flouter le seam.
* **Suppression des défauts** : activer/désactiver\
  Si cette option est activée, le filtre tente de supprimer les artefacts près du seam entre les calques supérieur et inférieur.
* **Color Equalizer** : 0-50\
  Égalisez les valeurs chromatiques pour diminuer la visibilité du seam.
* **Correspondance d&#39;Height** :\
  Modifiez la manière dont les maps height sont fusionnées pour les calques supérieur et inférieur. Pour voir les résultats plus clairement, affichez le canal height dans la **Vue 2D**. Notez que la correspondance d’height n’a aucune incidence sur les couches autres que la couche d’height. Les normales et l’AOP ne seront donc pas affectées par les modifications apportées à la correspondance d’height.

**Paramètres avancés**

* **Influence de la chrominance** : 0-1\
  Réglez l’impact des valeurs chromatiques sur le seam.
* **Inversion de masque** : activer/désactiver\
  Inversez les masques des calques supérieur et inférieur.
* **Smoothness de correspondance Height** : 0-16\
  Ajustez le flou de la correspondance des heights entre les calques supérieur et inférieur.
* **Source de correctif gauche/droit** : -1 à 1\
  Ajustez l’emplacement de la source pour les correctifs gauche et droit.
* **Source de correctif supérieur/inférieur** : -1 à 1\
  Ajustez l’emplacement de la source pour les patchs supérieur et inférieur.

## Guide d’utilisation

Le **filtre** Placer dans la mosaïque **&#x200B;**&#x200B;fonctionne en superposant plusieurs copies du matériau les unes sur les autres.

L’image ci-dessous montre la disposition des calques :

* Le périmètre vert montre les contours du matériau résultant du filtre **Mosaïque**
* Les lignes rouges indiquent les bordures du calque inférieur. Le calque inférieur est décalé de 50 % de l’espace UV sur les axes X et Y. Les lignes rouges correspondent donc aux seams de répétition à recouvrir.
* Le carré bleu et les demi-cercles couvrent les seams rouges. Les paramètres du filtre vous permettent d’ajuster les bordures des formes bleues pour vous assurer que le seam rouge n’est pas visible tout en conservant un seam bleu aussi lisse que possible.

![](../../assets/makeittilediagram.png){width="512px"}

Les demi-cercles gauche et droit correspondent pour assurer les mosaïques de matériau horizontalement, et les demi-cercles supérieur et inférieur assurent les mosaïques de matériau verticalement. Le carré bleu au centre supprime tous les seams restants pour créer un matériau entièrement carrelé sans seams.
