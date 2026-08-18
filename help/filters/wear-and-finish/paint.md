---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/wear-and-finish/paint.html"
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

Le **filtre Peinture** vous permet de recouvrir votre matériau d&#39;une couche de peinture de thickness variable.

*Un matériau métallique recouvert d’une peinture usée.*

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
  Définissez la couleur de peinture.
* **Rugosité** : 0-1\
  Définissez la rugosité des zones couvertes par la peinture.
* **Thickness** : 0-1\
  Réglez la viscosité et le thickness de la peinture. Cela a un impact sur la proportion de l’height sous-jacent et des informations normales visibles à travers la peinture.
* **Peel** : 0-1\
  Ajoutez des patchs à l’endroit où la peinture s’est détachée de la matière sous-jacente.
* **Grain** : 0-1\
  Modifiez le grain de la surface de la peinture.
* **Taille de grain** : 1-5\
  Réglez l’échelle de la texture utilisée pour créer les grains.

**Masquer**

* **Masque de cavité** : activer/désactiver\
  Créez un masque en fonction des cavités présentes dans la carte des heights. Si cette option est activée, les paramètres suivants apparaissent :
  * **Taille de la cavité** : 0-1\
    Ajustez la plage d’heights utilisée pour créer le masque de cavité.
  * **Intensité de la cavité** : 0-1\
    Réglez l’opacité du masque en fonction de la profondeur de la cavité.
  * **Masque d&#39;inversion de cavité** : activer/désactiver\
    Inversez le masque de cavité pour modifier s’il affecte les points haut ou bas.
* **Utiliser un masque personnalisé** : activer/désactiver\
  Activez ou désactivez l’utilisation d’un masque personnalisé. Si cette option est activée, les paramètres suivants apparaissent :
  * **Masque** : image/pinceau\
    Sélectionnez une image à utiliser comme masque ou utilisez le pinceau pour peindre un masque personnalisé directement dans la vue 2D.
  * **Masque personnalisé - Flou** : 0-1\
    Floutez le masque.
  * **Masque personnalisé - Inverser** : activer/désactiver\
    Inversez le masque.

**Paramètres avancés**

* **Couleur de base** : activer/désactiver\
  Indique si la couche de couleur de base est affectée par le filtre.
* **Métallique** : activer/désactiver\
  Indiquez si le canal métallique est affecté par le filtre.
  * **Valeur Métallique** : 0-1\
    Ajustez la valeur métallique des zones peintes.
* **Rugosité** : activer/désactiver\
  Définissez si la couche de rugosité est affectée par le filtre.
* **Normal** : activer/désactiver\
  Indique si le canal normal est affecté par le filtre. Si cette option est activée, une commande supplémentaire apparaît :
  * **Normal - Intensité** : -1 à 1\
    Réglez l’intensité des normales.
* **Height** : activer/désactiver\
  Définissez si le canal d’height est affecté par le filtre. Si cette option est activée, une commande supplémentaire apparaît :
  * **Height - Intensité** : 0-1\
    Réglez le contraste de la courbe d’height.
* **Opacité** : activer/désactiver\
  Définissez si la couche d’opacité est affectée par le filtre. Si cette option est activée, une commande supplémentaire apparaît :
  * **Opacité - Valeur** : 0-1\
    Modifiez l’opacité du matériau.
* **Émissif** : activer/désactiver\
  Définissez si le canal émissif est affecté par le filtre. Si cette option est activée, une commande supplémentaire apparaît :
  * **Émissif - Couleur** : sélection de couleur\
    Définissez la couleur du canal émissif.
* **Occlusion ambiante** : activer/désactiver\
  Définissez si le canal d’occlusion ambiante est affecté par le filtre. Si cette option est activée, les commandes supplémentaires suivantes apparaissent :
  * **Occlusion ambiante - Intensité** : 0-1\
    Réglez l’intensité de l’AO généré.
  * **Occlusion ambiante** **- Rayon** : 0-1\
    Réglez le rayon de l’effet AOP.
