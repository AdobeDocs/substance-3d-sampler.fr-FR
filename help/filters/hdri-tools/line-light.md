---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/hdri-tools/line-light.html"
breadcrumb-title: ''
description: Utilisez l’outil Lumière linéaire de Substance 3D Sampler pour ajouter des sources lumineuses linéaires aux environnements HDRI afin de contrôler avec précision l’éclairage.
helpx_creative_field: ""
helpx_description: Sampler > Filters > HDRI Tools > Line Light
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lumière de ligne
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---


# Lumière de ligne

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-linelight-18-n-d.png)

**Entrées :** Outils HDRI

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Ajoutez une **Lumière de ligne** à l&#39;éclairage de votre environnement.

Les images ci-dessous montrent comment utiliser une **lumière de ligne** pour régler l&#39;éclairage de votre environnement.![](../../assets/3d-2d-filters-cropped-0017-line-light-in.jpg)

L’image ci-dessus montre une sphère sans modification de la luminosité de l’environnement.

![](../../assets/3d-2d-filters-cropped-0016-line-light-out.jpg)

Après avoir ajouté une **Lumière de ligne**, l&#39;apparence de la sphère a sensiblement changé.

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Exposition (EV)** : 0-10\
  Réglez l’exposition ou la luminosité de la lumière.
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
* **Mode de position** :\
  Modifiez la méthode utilisée pour déterminer la position des éclairages. Les paramètres de la section **Coordonnées de position** changeront en fonction de la sélection. Lorsque **Position mondiale** est sélectionnée, les poignées disparaissent de la **vue 2D**. Utilisez plutôt les paramètres de **Coordonnées de position** pour modifier la position de la lumière.

**Forme**

* **Rotation de ligne** : 0-1\
  Faire pivoter la lumière
* **Thickness de ligne** : 0-1\
  Ajustez le thickness de la ligne qui constitue la lumière.
* **Motif** :\
  Modification de la forme de la ligne
* **Dureté du motif** : 0-1\
  Adoucissez les bords de la lumière
* **Mode UV du motif** :\
  Modifiez le motif sur lequel la lumière est basée. **Étirer** étire toute la forme pour qu&#39;elle corresponde aux extrémités de la ligne. **L’option Étirer le milieu uniquement** étire le milieu de la forme en conservant les extrémités de la ligne non déformées. **Répéter + Espacement** crée des tampons de la forme le long des lignes et ajoute un paramètre supplémentaire pour gérer l&#39;espacement :
  * **Espacement de répétition de motif** : 0-1\
    Ajustement de la largeur de l’espacement entre les instances de forme

**Coordonnées De Position**

Les paramètres disponibles dépendent de la sélection effectuée pour **Paramètres de base > Mode de position**. Si **Sol/Plafond** ou **Distance avec l&#39;origine** sont sélectionnés, les paramètres suivants sont disponibles :

* **Height absolu de ligne** : 0-1\
  Modifiez la distance de la lumière par rapport à l’appareil photo.
* **Position de l&#39;appareil photo** : 0-1\
  Réglez la position relative de la caméra par rapport à la lumière sur les axes X, Y et Z.

Si **Position universelle** est choisie dans **Paramètres de base > Mode de position**, les paramètres suivants sont disponibles :

* **Up Vector** :\
  Modifiez la direction vers le haut.
* **Position mondiale du point 1** : -2 à 2\
  Ajustez la position du premier point de la ligne sur les axes X, Y et Z.
* **Position mondiale au point 2** : -2 à 2\
  Ajustez la position du deuxième point de la ligne sur les axes X, Y et Z.
* **Position de l&#39;appareil photo** : 0-1\
  Réglez la position relative de la caméra par rapport à la lumière sur les axes X, Y et Z.

**Arrière-plan**

* **Afficher la grille au sol** : activer/désactiver\
  Affichez ou masquez la grille de sol.
* **Activer l&#39;écrêtage au sol** : activer/désactiver\
  Indiquez si la lumière peut se couper à travers le sol ou non. Si cette option est activée, le contrôle suivant s’affiche :
  * **Height au sol** : -2 à 2\
    Réglez l’height du sol afin d’écrêter la lumière.
* **Gamma d&#39;arrière-plan** :\
  Sélectionnez le système de couleurs utilisé pour déterminer le gamma de l’arrière-plan.
