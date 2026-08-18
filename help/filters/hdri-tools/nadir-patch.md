---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/hdri-tools/nadir-patch.html"
breadcrumb-title: ''
description: Utilisez l’outil Nadir patch de Substance 3D Sampler pour corriger la zone nadir des images HDRI afin de créer des cartes d’environnement homogènes.
helpx_creative_field: ""
helpx_description: Sampler > Filters > HDRI Tools > Nadir Patch
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Nadir patch
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---


# Nadir patch

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-nadirpatch-18-n-d.png)

**Entrées :** Outils HDRI

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Appliquez un correctif au nadir de la lumière de votre environnement pour masquer les artefacts ou les coutures.

Dans les images ci-dessous, vous pouvez voir comment **Nadir patch** est utilisé pour retirer le support de l&#39;appareil photo de cette image panoramique.

![](../../assets/3d-2d-filters-cropped-0011-nadir-patch-in.jpg)![](../../assets/3d-2d-filters-cropped-0010-nadir-patch-out.jpg)

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Activer** : activer/désactiver\
  Activer ou désactiver le patch : cette option peut être utile pour voir rapidement l’impact du patch sans avoir à modifier la visibilité du calque.
* **Afficher l&#39;assistant d&#39;images** : activer/désactiver\
  Activez ou désactivez l’option Images.
* **Thickness d&#39;images** : 0-1\
  Ajustez le thickness de l&#39;image. Cela peut être utile lorsque la source du patch est loin du nadir.
* **Échelle de correctif** : 0-1\
  Ajustez la limite de la zone à corriger.
* **Taille du correctif** :\
  Ajustez les dimensions du patch.
* **Rotation du correctif** : 0-1\
  Faites pivoter les limites du patch. La source et l&#39;emplacement du correctif pivotent, de sorte que le correctif ait toujours la même orientation. Pour faire pivoter le correctif en place, utilisez **Décalage de rotation source**.
* **Alpha du correctif** :\
  Sélectionnez la forme utilisée pour masquer le patch. Si **Entrée de masque** est sélectionné, un paramètre supplémentaire s&#39;affiche :
  * **Entrée de masque** : image/pinceau\
    Importez une image à utiliser comme masque ou peignez un masque directement dans la **vue 2D**.
* **Dureté du correctif** : 0-1\
  Ajustez le flou sur les bords du masque de correction.
* **Décalage de rotation source** : 0-1\
  Décaler la rotation de la source : cette opération a pour effet de faire pivoter le patch.

## Guide d’utilisation

Un problème courant pouvant se produire lors de la création d’une luminosité de l’environnement à partir de photos est celui des artefacts se produisant autour des nadirs supérieur et inférieur de la texture. Le **filtre** **Nadir patch** permet de réduire ces problèmes.

1. Ajoutez le **filtre de Nadir patch** en haut de la pile de calques.
1. Utilisez la poignée de la **vue 2D** pour modifier l&#39;emplacement source du correctif.
   1. Le nadir corrigé change selon l’emplacement de la source. Si la source se trouve dans la moitié inférieure de l’espace de texture, le nadir inférieur est corrigé ; si la source se trouve dans la moitié supérieure, le nadir supérieur est corrigé.
1. Modifiez les paramètres pour affiner la transformation du patch afin de mieux masquer les coutures et les artefacts.
