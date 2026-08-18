---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/generators/decal.html"
breadcrumb-title: ''
description: Utilisez le générateur de décalcomanies de Substance 3D Sampler pour créer des motifs de décalcomanie et des textures d’incrustation pour les surfaces de matériau.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Decal
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Décalque
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 1%

---


# Décalque

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-decal-18-n-d.png)

Générateurs De **Entrée :**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Le filtre Décalcomanie vous permet d’ajouter des instances d’une autre matière à un emplacement spécifique. Ceci est utile pour ajouter des éléments tels que des autocollants ou des détails spécifiques qui pourraient ne pas être faciles à générer d’un point de vue procédural.

Les images ci-dessous montrent le **filtre Décalcomanie** utilisé pour endommager le béton.

![](../../assets/3d-2d-filters-cropped-0045-decal-in.jpg)

Avant l’ajout de la décalcomanie, la couche de base en béton est propre et intacte.

![](../../assets/3d-2d-filters-cropped-0044-decal-out.jpg)

Une fois le **filtre Décalcomanie** appliqué, des fissures et des dommages réalistes sont ajoutés au matériau.

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Mode mosaïque** :\
  Détermine s&#39;il faut afficher en mosaïque au-delà des poignées dans la **vue 2D**.\
  H représente Horizontal, tandis que V représente Vertical.
* **Correspondance des couleurs du matériau inférieur** : 0-1\
  Réglez les couleurs de la décalcomanie pour qu’elles correspondent à la valeur chromatique des calques situés en dessous.
* **Mode de fusion normal** :\
  Réglage de la fusion des normales entre le matériau de la décalcomanie et les calques sous-jacents
* **Fusion d&#39;opacité normale** : 0-1\
  Modification de l’opacité des normales de la matière de décalcomanie
* **Position De L&#39;Height De Décalcomanie** : 0-1\
  Régler l’height de la décalcomanie par rapport à l’height des calques sous-jacents
* **Échelle D&#39;Height De Décalcomanie** : 0-1\
  Modification du contraste de la courbe d’height de la matière de la décalcomanie

**Paramètres avancés**

* **Transformation de décalcomanie** :\
  Ajustez les valeurs de transformation de la matrice pour la décalcomanie. En général, il est plus facile d&#39;utiliser simplement les poignées de la **vue 2D** pour ajuster la transformation de la décalcomanie.
* **Décalage** **Décalage** : -1 à 1\
  Réglez le décalage de la décalcomanie.

## Guide d’utilisation

Pour utiliser le filtre Décalcomanie :

1. Ajout du filtre Décalcomanie à la pile de calques
1. Sous le calque Décalcomanie, un emplacement d’entrée apparaît
1. Faites glisser le matériau de votre décalcomanie dans l’emplacement d’entrée du calque de décalcomanie

Vous pouvez ajuster les paramètres du filtre dans le **panneau Propriétés** en sélectionnant le calque Décalcomanie.

Vous pouvez ajuster les paramètres du matériau d&#39;entrée de la décalcomanie dans le **panneau Propriétés** en sélectionnant le matériau dans l&#39;emplacement d&#39;entrée.
