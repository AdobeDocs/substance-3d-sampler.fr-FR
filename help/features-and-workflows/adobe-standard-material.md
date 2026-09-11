---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/features-and-workflows/adobe-standard-material.html"
breadcrumb-title: ''
description: Apprenez à utiliser Adobe Standard Material dans Substance 3D Sampler pour créer des matériaux compatibles avec la norme matériau d’Adobe.
helpx_creative_field: ""
helpx_description: Sampler > Features and workflows > Adobe Standard Material
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Adobe Standard Material
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0f989901713dd30f8f936de2445caf5dc70a9225
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 1%

---


# Adobe Standard Material

>[!NOTE]
>
> Substance 3D Sampler utilise désormais par défaut le modèle de matériau [OpenPBR](openpbr.md) plutôt que l&#39;Adobe Standard Material.


## Propriétés de matériau standard

## Propriétés de la surface de base

**Base color**

Couleur de la surface.

**Rugosité**

Lissage ou cache de la surface.

![](../assets/surface-roughness.jpg)

**Métallique**

Degré d&#39;éclat métallique de la surface.

![](../assets/surface-metallic.jpg)

**Opacité**

La visibilité de la surface.

![](../assets/surface-opacity.jpg)

**Ambient occlusion**

Ombres des cavités et plis empêchant la lumière de frapper la surface.

**Specular level**

Force des reflets de lumière sur la surface.

![](../assets/surface-specularlevel.jpg)

**Specular edge color**

Couleur des reflets de lumière. Affecte les angles de visée des matériaux métalliques.

![](../assets/surface-specularedgecolor.jpg)

**Normal**

Simule les détails d’une surface tels que les bosses et les fissures.

**Échelle normale**

Force de l&#39;effet normal.

**Combiner normal et height**

Applique la texture normale au-dessus de la texture d’height.

**Height**

Crée des détails de surface à l&#39;aide d&#39;un displacement de relief ou de géométrie.

**Échelle d&#39;Height**

Echelle d&#39;height en unités de scène. S’applique à la bosse et au displacement.

**Niveau d&#39;Height**

Valeur de la texture d&#39;height représentant le displacement zéro.

**Anisotropy level**

Quantité que les reflets étirent dans une direction le long de la surface.

![](../assets/surface-anisotropy.jpg)

**Anisotropy angle**

Rotation antihoraire de l’effet anisotrope.

**Intensité des émissions**

Intensité de la lumière émise par la surface.

![](../assets/surface-emission.jpg)

**Couleur d&#39;émission**

Couleur de la lumière émise.

![](../assets/surface-emissioncolor.jpg)

**Opacité de l&#39;Éclat**

Simule l&#39;effet des fibres microscopiques ou du flou sur la surface.

![](../assets/surface-sheen.jpg)

**Couleur de l&#39;éclat**

Couleur de l’effet éclat.

![](../assets/surface-sheencolor.jpg)

**rugosité d&#39;Éclat**

Lissage de l’effet éclat.

![](../assets/surface-sheenroughness.jpg)

## Propriétés intérieures

**Translucency**

Quantité de lumière pouvant passer à travers la surface.

![](../assets/interior-translucency.jpg)

**Couleur d&#39;absorption**

La lumière de couleur convergera à mesure qu’elle sera absorbée.

**Distance d&#39;Absorption**

Distance approximative en unités de scène que la lumière parcourra avant d’atteindre la couleur d&#39;absorption. Si cette option est définie sur zéro, le thickness n’affectera pas la couleur d&#39;absorption.

![](../assets/interior-absorptiondistance.jpg)

**Index de réfraction**

La quantité de lumière qui passe à travers l’objet.

![](../assets/interior-indexofrefraction.jpg)

**Dispersion**

Étendue du spectre de couleurs lorsque réfracté.

**Subsurface scattering**

Dispersion la lumière sous la surface, plutôt que de passer directement à travers.

**Scattering**

Couleur sous la surface à laquelle la lumière diffuse se transforme.

![](../assets/interior-scattercolor.jpg)

**Distance de diffusion**

La lumière de distance approximative doit parcourir avant d&#39;atteindre la diffusion complète.

![](../assets/interior-scatterdistance.jpg)

**Échelle de distance de diffusion**

Multiplicateur de la distance de dispersion. Peut être différent pour chaque couche de couleur.

![](../assets/interior-scatterdistancescale.jpg)

**Décalage rouge**

Définit la lumière rouge pour voyager plus loin que les autres couleurs claires. Utile pour la peau.

![](../assets/interior-scatterredshift.jpg)

**Diffusion Rayleigh**

Définit la lumière orange pour qu’elle passe plus loin sous la surface et la lumière bleue pour qu’elle voyage moins.

![](../assets/interior-scatterraleigh.jpg)

**thickness de volume**

Thickness de la surface par rapport au cadre de sélection de l’objet. Utilisé pour les effets d&#39;intérieur lorsque le thickness réel n&#39;est pas connu.

**Échelle de thickness du volume**

Multiplicateur du thickness de volume.

## Propriétés du pelage

**Coat opacity**

Simule un calque au-dessus du matériau. Permet de créer des couches, des laques et des vernis clairs.

![](../assets/coat-coatopacity.jpg)

**Coat color**

La couleur du pelage.

![](../assets/coat-coatcolor.jpg)

**Coat roughness**

Degré de lissage ou de mat de la surface du pelage.

![](../assets/coat-coatroughness.jpg)

**Indice de réfraction de la couche**

La quantité de lumière se courbe lorsqu’elle passe à travers le pelage.

![](../assets/cooat-coatior.jpg)

**Coat specular level**

La force des reflets lumineux sur le pelage à des angles de regard.

![](../assets/coat-coatspecular.jpg)

**Coat normal**

Simule les détails de la surface comme les bosses et les fissures sur la surface du pelage.

![](../assets/coat-coatnormal.jpg)

**Échelle de Coat normal**

Force de l’effet de coat normal.
