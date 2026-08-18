---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/adjustments/colorize.html"
breadcrumb-title: ''
description: Utilisez le filtre Coloriser de Substance 3D Sampler pour appliquer des teintes de couleur et des effets de coloration monochrome aux textures et aux matières.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Adjustments > Colorize
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Coloriser
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 1%

---


# Coloriser

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/S_ColorFill_18_N_D.png)

**Entrée :** Réglages

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

L’option Coloriser vous permet d’ajouter de la couleur à une sélection de couches sans perdre de détails.

>[!NOTE]
>
> Le filtre Coloriser vous permet de modifier la couche normale, mais ce n’est pas une bonne idée de le faire à moins de bien comprendre le fonctionnement de la couche normale et son impact sur votre matériau. Il s’agit d’une fonction avancée qui ne devrait généralement être nécessaire que dans des circonstances spécifiques.

Dans ces images, le **filtre Coloriser** a été utilisé pour ajuster la couleur de base afin de produire un matériau en bois beaucoup plus riche.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0045-colorize-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0044-colorize-out.jpg){width="200px"}

</td>
</tr>
</table>

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

Les paramètres disponibles dans cette section changent en fonction de la **sélection de canal**.

* **Sélection de canal** :\
  Sélectionnez le canal que le filtre affectera. Il est conseillé d’afficher le canal sélectionné dans la vue 2D pour voir directement les résultats du filtre.
  * ***Options de couleur de base/d’émission***
    * ***Nom du canal*** **- Couleur** : sélection de la couleur\
      Sélection de la couleur utilisée pour coloriser la couche
    * ***Nom du canal*** **- Conserver la luminosité** : activer/désactiver\
      Si cette option est activée, les valeurs de luminosité et de luminosité des couleurs d’origine sont conservées
    * ***Nom Du Canal*** **- Intensité** : 0-1\
      Réglez l’intensité de l’effet Coloriser.
  * ***Options de canal normal***
    * **Normal - Angle De Pente** : 0-90\
      Modifier le dégradé de la normale
    * **Normal - Direction** : 0-360\
      Réglage de la direction des faces normales
    * **Normal - Conserver la luminosité** : activer/désactiver\
      Si cette option est activée, la luminosité des normales d&#39;origine est conservée
    * **Normal - Intensité** : 0-1\
      Réglez l’intensité de l’effet Coloriser.
* **Masque personnalisé** : activer/désactiver\
  Activez ou désactivez l’utilisation d’un masque personnalisé. Si cette option est activée, les paramètres suivants apparaissent :
  * **Masque** : image/pinceau\
    Sélectionnez une image à utiliser comme masque ou utilisez le pinceau pour peindre un masque personnalisé directement dans la vue 2D
  * **Masque personnalisé - Flou** : 0-1\
    Flouter le masque
  * **Masque personnalisé - Inverser** : activer/désactiver\
    Inverser le masque
