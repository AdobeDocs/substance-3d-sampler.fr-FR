---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/wear-and-finish/rust.html"
breadcrumb-title: ''
description: Utilisez le filtre Rouille de Substance 3D Sampler pour ajouter des effets de rouille et de corrosion réalistes aux matériaux et surfaces métalliques.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Wear and Finish > Rust
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Rouille
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 1%

---


# Rouille

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-rust-18-n-d.png)

**Entrée :** usure et finition

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Utilisez le **filtre Rouille** pour ajouter une couche de métal oxydé à votre matériau.

Dans les images ci-dessous, vous pouvez voir un matériau métallique avant et après l&#39;ajout du **filtre de Rouille**.

![](../../assets/3d-filters-cropped-0002-rust-out.jpg){width="200px"}

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Générateur aléatoire** :\
  La valeur de départ aléatoire détermine les valeurs aléatoires des autres paramètres qui utilisent le caractère aléatoire dans ce filtre.
* **Répartition des Rouilles** : 0-1\
  Contrôlez la planche ou la quantité de rouille.
* **Influence des contours** : 0-1\
  Ajustez la façon dont la rouille interagit avec les arêtes en fonction de la courbe de courbure.
* **Smoothness de planche** : 0-1\
  Augmentez cette valeur pour accentuer le lobby des zones rouillées ou diminuez-la pour les rendre plus détaillées.
* **Affecter Metal uniquement** : activer/désactiver\
  Lorsque cette option est activée, le **filtre de Rouille** n&#39;a d&#39;impact que sur les zones dont la valeur métallique est supérieure à 0.

**Rouille**

* **Forme de Rouille** :\
  Modifiez le motif sur lequel la rouille est basée.
* **Intensité de la Rouille** : 0-1\
  Modifiez l’intensité de l’effet rouille. Si vous augmentez cette valeur, la rouille semble plus ancienne et plus résistante.

**Peel**

* **Échelle de pelage** : 0-1\
  Modifiez l’échelle de la rouille de pelage.
* **Intensité normale du pelage** : 0-1\
  Ajustez la visibilité des normales de la peau.
* **Intensité de l&#39;Height de pelage** : 0-1\
  Ajustez l&#39;impact des pelages sur la carte des heights.

**Gouttes**

* **Intensité des gouttes** : 0-1\
  Modifiez l’intensité de l’effet de goutte à goutte.
* **Orientation des gouttes** : 0-1\
  Orientez les gouttes pour qu&#39;elles correspondent à la gravité ou au vent.
* **Longueur des gouttes** : 0-1\
  Ajustez la distance sur laquelle les gouttes s’étendent depuis la source.

**Masquer**

* **Utiliser le masque** : activer/désactiver\
  Activez ou désactivez l’utilisation d’un masque personnalisé. Si cette option est activée, les paramètres suivants apparaissent :
  * **Masque** : image/pinceau\
    Sélectionnez une image à utiliser comme masque ou utilisez le pinceau pour peindre un masque personnalisé directement dans la vue 2D.
  * **Masque personnalisé - Flou** : 0-1\
    Floutez le masque.
  * **Masque personnalisé - Inverser** : activer/désactiver\
    Inversez le masque.
