---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/generators/quilt-stitch.html"
breadcrumb-title: ''
description: Utilisez le générateur de points de couture dans Substance 3D Sampler pour créer des motifs de tissu matelassé et des textures de couture pour les matériaux.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Quilt Stitch
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Point de surface composée
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---


# Point de surface composée

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-quiltstitch-18-n-d.png)

Générateurs De **Entrée :**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Émulez un motif de surface composée dans vos matériaux avec ce filtre.

*Avant et après l’application du **filtre Point de surface composée**.*

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0005-quilt-stitch-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0004-quilt-stitch-out.jpg){width="200px"}

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
* **Sélection de motif** :\
  Sélectionnez le style de motif pour la couture/surface composée à suivre
* **Quantité** : 1-5\
  Contrôle de la répétition du motif
* **Rotation** :\
  Faire pivoter le motif
* **Topstitch** : activer/désactiver\
  Activez cette option pour ajouter un point de coupe et voir la section de paramètre pertinente
* **Seam** : activer/désactiver\
  Activez cette option pour ajouter un seam et voir la section des paramètres pertinents
* **Surface composée** : basculer\
  Activez cette option pour ajouter une surface composée et voir la section de paramètre pertinente
* **Peinture Edge** : basculer\
  Activez cette option pour peindre le bord entre les sections matelassées et voir la section de paramètre pertinente
* **Avancé** : activer/désactiver\
  Activer pour afficher les paramètres **avancés**

**Topstitch**

* **Couleur du point de suture** : sélection de la couleur\
  Définir la couleur du fil utilisé pour le point de tête
* **Décalage du point de suture** : 0-1\
  Décalage du point de sommet par rapport aux bords de la zone matelassée
* **Rotation Topstitch** : 0-1\
  Modification de l’orientation des points qui composent le point supérieur
* **Échelle Topstitch** : 0-1\
  Ajustez la taille du point de dessus dans chaque dimension (largeur, longueur et height)
* **Intensité de la ponction** : 0-1\
  Ajuster le retrait dans la surface composée causé par la couture du dessus
* **Rugosité Topstitch** : 0-1\
  Ajuster la rugosité du lien
* **Topstitch Métallique** : 0-1\
  Ajuster la valeur métallique du lien

**Seam**

* **Sélection** **Seam** :\
  Sélectionner le style de seam à utiliser
* **Intensité du Seam** : 0-1\
  Modifier les intensités normale et height du seam
* **Intensité du Étire** : 0-1\
  Ajustez l’impact de la étire du tissu sur le seam. Cet effet est assez subtil.

**Surface composée**

* **Type de surface composée** :\
  Sélectionner le style de surface composée à utiliser
* **Intensité de la surface composée** :\
  Régler l’intensité normale et l’intensité height de l’effet de matelassage

**Peinture Edge**

* **Sélection des contours** :\
  Indiquez si la douleur doit supplanter les détails heights et normaux du matériau sous-jacent ou non
* **Couleur des contours** : sélection de la couleur\
  Sélectionner la couleur de peinture
* **rugosité Edge** : 0-1
* **Edge Métallique** : 0-1

**Avancé**

* **Height du Matériau de base** : 0-1\
  Ajuster la force de la map height à partir du matériau sous-jacent
* **Intensité normale** : 0-1\
  Ajustez la force des modifications de map normal en fonction du filtre **Point de surface composée**. Cela n’a aucune incidence sur la normalité du matériau sous-jacent.
