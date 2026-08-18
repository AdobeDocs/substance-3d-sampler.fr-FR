---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/hdri-tools/sphere-light.html"
breadcrumb-title: ''
description: Utilisez l’outil Lumière sphérique de Substance 3D Sampler pour ajouter des sources lumineuses sphériques aux environnements HDRI afin d’obtenir des effets d’éclairage ponctuels.
helpx_creative_field: ""
helpx_description: Sampler > Filters > HDRI Tools > Sphere Light
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lumière sphérique
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---


# Lumière sphérique

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-spherelight-18-n-d.png)

**Entrées :** Outils HDRI

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Ajoutez une lumière sphère à votre environnement.

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Mode de couleur de forme** :\
  Sélectionnez la méthode à utiliser pour déterminer la couleur de la lumière. Les paramètres disponibles changeront en fonction de cette sélection.
  * **Température (Kelvin)**
    * **Température** : 1 000 - 27000\
      Réglez la température de la lumière.
  * **RGB**
    * **Couleur** : sélection de couleur\
      Sélectionnez la couleur de la lumière.
  * **Entrée d&#39;image**
    * **Entrée d&#39;image de forme** : image/pinceau\
      Importez une image à utiliser comme couleur. Vous pouvez utiliser l&#39;outil Pinceau pour peindre directement dans la **vue 2D**, mais les résultats peuvent être imprévisibles avec ce filtre.
  * **Exemple D&#39;Arrière-Plan**
    * L’exemple d’arrière-plan ne rend pas les nouveaux paramètres disponibles. Il base plutôt la couleur de la lumière sur les valeurs d’arrière-plan.
* **Exposition (EV)** : 0-10\
  Réglez l’exposition ou la luminosité de la lumière.
* **Rayon sphère** : 0-1\
  Réglez la taille de la lumière.
* **Mode de position** :\
  Modifiez la méthode utilisée pour déterminer la position des éclairages. Les paramètres de la section **Coordonnées de position** changeront en fonction de la sélection.

**Coordonnées De Position**

Les paramètres disponibles dépendent de la sélection effectuée pour **Paramètres de base > Mode de position**. Si **Distance avec l&#39;origine** est sélectionnée, les paramètres suivants sont disponibles :

* **Distance avec l&#39;origine** : 0-20\
  Réglez la distance entre la lumière et l’appareil photo.
* **Position de l&#39;appareil photo** : 0-1\
  Réglez la position relative de la caméra par rapport à la lumière sur les axes X, Y et Z.

Si **Position universelle** est sélectionnée, les paramètres suivants sont disponibles :

* **Up Vector** :\
  Modifiez la direction vers le haut.
* **Position mondiale Sphère** : -2 à 2\
  Ajustez la position de la lumière de la sphère sur les axes X, Y et Z.
* **Distance avec l&#39;origine** : 0-20\
  Réglez la distance entre la lumière et l’appareil photo.
* **Position de l&#39;appareil photo** : 0-1\
  Réglez la position relative de la caméra par rapport à la lumière sur les axes X, Y et Z.

**Forme**

* **Dureté de la sphère** : 0-1\
  Adoucissez ou durcissez les bords de la lumière de la sphère
* **Ombrage** :\
  Modifiez le dégradé de l&#39;exposition de la lumière en fonction de différents styles de lumière du monde réel. Avec l&#39;option **Lumière d&#39;Ombrage** sélectionnée, des paramètres supplémentaires apparaissent :
  * **Position mondiale Ombrage clair** : -1 à 1\
    Modifier la position de la zone ombrée sur la lumière
  * **Transparence Penumbra** : 0-1\
    Réglez le niveau d’opacité de la zone ombrée de la lumière.

**Arrière-plan**

* **Gamma d&#39;arrière-plan** :\
  Sélectionnez le système de couleurs utilisé pour déterminer le gamma de l’arrière-plan.
