---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/hdri-tools/plane-light.html"
breadcrumb-title: ''
description: Utilisez l’outil Lumière plane de Substance 3D Sampler pour ajouter des sources lumineuses planaires aux environnements HDRI afin de créer des effets d’éclairage de zone.
helpx_creative_field: ""
helpx_description: Sampler > Filters > HDRI Tools > Plane Light
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Éclairage plan
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---


# Éclairage plan

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-planelight-18-n-d.png)

**Entrées :** Outils HDRI

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Ajoutez une lumière en forme de plan plat à votre environnement.

![](../../assets/3d-2d-filters-cropped-0002-plane-light-out.jpg)

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
      Importez une image à utiliser comme couleur. Vous pouvez utiliser l&#39;outil Pinceau pour effectuer une peinture directement dans la **Vue 2D**, mais les résultats peuvent être imprévisibles avec ce filtre.
  * **Exemple D&#39;Arrière-Plan**
    * L’exemple d’arrière-plan ne rend pas les nouveaux paramètres disponibles. Il base plutôt la couleur de la lumière sur les valeurs d’arrière-plan.
* **Mode de position** :\
  Modifiez la méthode utilisée pour déterminer la position des éclairages. Les paramètres de la section **Coordonnées de position** changeront en fonction de la sélection. Lorsque **Position mondiale** est sélectionnée, les poignées disparaissent de la **Vue 2D**. Utilisez plutôt les paramètres de **Coordonnées de position** pour modifier la position de la lumière.

**Forme**

* **Échelle de plan**; 0-1\
  Réglez l’échelle de la lumière.
* **Taille du plan** : 0-1\
  Ajustez les dimensions de la lumière dans les axes X et Y.
* **Rotation du plan** : 0-1\
  Réglez la rotation de la lumière le long des axes X, Y et Z.
* **Motif** :\
  Sélectionnez la forme de la lumière.
* **Dureté de motif** : 0-1\
  Adoucissez ou floutez les bords de la lumière
* **Mode d&#39;UV de motif** :\
  Choisissez si les transformes doivent étirer la forme entière ou uniquement le milieu de la forme pour conserver les détails des bords et des angles.

**Coordonnées De Position**

Les paramètres disponibles dépendent de la sélection effectuée pour **Paramètres de base > Mode de position**. Si **Sol/plafond** ou **Distance avec l&#39;origine** sont sélectionnés, les paramètres suivants sont disponibles :

* **Height absolu de ligne** : 0-1\
  Modifiez la distance de la lumière par rapport à la caméra.
* **Position De La Caméra** : 0-1\
  Ajustez la position relative de la caméra par rapport à la lumière dans les axes X, Y et Z.

Si **Position universelle** est choisie dans **Paramètres de base > Mode de position**, les paramètres suivants sont disponibles :

* **Up Vector** :\
  Modifiez la direction vers le haut.
* **Position mondiale du point 1** : -2 à 2\
  Ajustez la position du premier point de la ligne dans les axes X, Y et Z.
* **Position mondiale au point 2** : -2 à 2\
  Ajustez la position du deuxième point de la ligne dans les axes X, Y et Z.
* **Position De La Caméra** : 0-1\
  Ajustez la position relative de la caméra par rapport à la lumière dans les axes X, Y et Z.

**Arrière-plan**

* **Afficher la Grille du Sol** : activer/désactiver\
  Affichez ou masquez la grille du sol.
* **Activer l&#39;écrêtage du Sol** : activer/désactiver\
  Indiquez si la lumière peut se couper à travers le sol ou non. Si cette option est activée, le contrôle suivant s’affiche :
  * **Height du Sol** : -2 à 2\
    Réglez l’height du sol pour écrêter la lumière.
* **Gamma d&#39;arrière-plan** :\
  Sélectionnez le système de couleurs utilisé pour déterminer le gamma de l’arrière-plan.
