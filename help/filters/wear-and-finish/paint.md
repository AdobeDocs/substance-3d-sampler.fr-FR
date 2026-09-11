---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/wear-and-finish/paint.html"
breadcrumb-title: ''
description: Utilisez le filtre Peinture de Substance 3D Sampler pour ajouter des calques de peinture, des revêtements et des effets de surface peints à vos matériaux.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Wear and Finish > Paint
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Peinture
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---


# Peinture

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-paint-18-n-d.png)

**Entrée :** usure et finition

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Le **filtre de Peinture** vous permet de couvrir votre matériau d&#39;un calque de peinture de thickness variable.

*Un matériau métallique recouvert d’une peinture usée a été ajouté.*

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0017-paint-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0016-paint-out.jpg){width="200px"}

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
* **Couleur** : sélection de couleur\
  Définissez la couleur de la peinture.
* **Rugosité** : 0-1\
  Définissez la rugosité des zones couvertes par la peinture.
* **Thickness** : 0-1\
  Régler la viscosité et le thickness de la peinture. Cela a un impact sur la part de l’height sous-jacent et des informations normales qui est visible à travers la peinture.
* **Peel** : 0-1\
  Ajoutez les dispositifs à l’endroit où la peinture s’est détachée du matériau sous-jacent.
* **Grain** : 0-1\
  Modifiez le grain de la surface de la peinture.
* **Taille de grain** : 1-5\
  Réglez l’échelle de la texture utilisée pour créer les grains.

**Masquer**

* **Masque de cavité** : activer/désactiver\
  Créez un masque en fonction des cavités présentes dans la map height. Si cette option est activée, les paramètres suivants apparaissent :
  * **Taille de la cavité** : 0-1\
    Ajustez la plage d’heights utilisée pour créer le masque de cavité.
  * **Intensité de la cavité** : 0-1\
    Réglez l’opacité du masque en fonction de la profondeur de la cavité.
  * **Masque d&#39;inversion de cavité** : activer/désactiver\
    Inversez le masque de cavité pour modifier s’il affecte les points haut ou bas.
* **Utiliser un masque personnalisé** : activer/désactiver\
  Activez ou désactivez l’utilisation d’un masque personnalisé. Si cette option est activée, les paramètres suivants apparaissent :
  * **Masque** : image/pinceau\
    Sélectionnez une image à utiliser comme masque ou utilisez le pinceau pour appliquer un peinture personnalisé directement dans la Vue 2D.
  * **Masque personnalisé - Flou** : 0-1\
    Floutez le masque.
  * **Masque personnalisé - Inverser** : activer/désactiver\
    Inversez le masque.

**Paramètres avancés**

* **Base color** : activer/désactiver\
  Définissez si le canal de base color est affecté par le filtre.
* **Métallique** : activer/désactiver\
  Définissez si la couche métallique est affectée par le filtre.
  * **Valeur Métallique** : 0-1\
    Ajustez la valeur métallique des zones peintes.
* **Rugosité** : activer/désactiver\
  Définissez si le canal de rugosité est affecté par le filtre.
* **Normal** : activer/désactiver\
  Indique si le canal normal est affecté par le filtre. Si cette option est activée, une commande supplémentaire apparaît :
  * **Normal - Intensité** : -1 à 1\
    Réglez l’intensité des normales.
* **Height** : activer/désactiver\
  Définissez si le canal d’height est affecté par le filtre. Si cette option est activée, une commande supplémentaire apparaît :
  * **Height - Intensité** : 0-1\
    Réglez le contraste de la map height.
* **Opacité** : activer/désactiver\
  Définissez si la couche d’opacité est affectée par le filtre. Si cette option est activée, une commande supplémentaire apparaît :
  * **Opacité - Valeur** : 0-1\
    Modifiez l’opacité du matériau.
* **Emissive** : activer/désactiver\
  Définissez si le canal d’emissive est affecté par le filtre. Si cette option est activée, une commande supplémentaire apparaît :
  * **Emissive - Couleur** : sélection de la couleur\
    Définissez la couleur de la couche emissive.
* **Ambient occlusion** : activer/désactiver\
  Définissez si le canal d’ambient occlusion est affecté par le filtre. Si cette option est activée, les commandes supplémentaires suivantes apparaissent :
  * **Ambient occlusion - Intensité** : 0-1\
    Réglez la force de l’AO généré.
  * **Ambient occlusion** **- Rayon** : 0-1\
    Réglez le rayon de l’effet AOP.
