---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/adjustments/color-replace.html"
breadcrumb-title: ''
description: Utilisez le filtre Remplacement de couleur de Substance 3D Sampler pour remplacer des couleurs spécifiques dans des textures par de nouvelles valeurs chromatiques.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Adjustments > Color Replace
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Remplacement de couleur
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---


# Remplacement de couleur

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-replacecolor-18-n-d.png)

**Entrée :** Réglages

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Remplacer une couleur ou une valeur choisie dans une couche.

Les images ci-dessous montrent **Remplacement de couleur** en action. Notez que les zones entre les carreaux restent de la même couleur, seuls les carreaux sont modifiés.

![](../../assets/3d-2d-filters-cropped-0051-color-replace-in.jpg)![](../../assets/3d-2d-filters-cropped-0050-color-replace-out.jpg)

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Segmentation avancée** : basculer\
  Lorsque cette option est activée, le filtre peut utiliser une couche distincte pour générer des informations de masque à partir de la couche affectée par le remplacement de couleur.
  * **Masquer** **De** :\
    Sélectionnez un canal qui servira de source pour la génération du masque. Par exemple, le masque de la valeur métallique remplace la couleur de base des zones métalliques du matériau
* **Remplacer dans** :\
  Sélectionnez la couche affectée par le remplacement de couleur.
* **Couleur cible** : sélection de couleur\
  Sélectionnez la couleur qui remplacera les couleurs de la couche actuelle.
* **Variation de luminosité** : 0-1\
  Réglez le degré d&#39;incidence de la luminosité des valeurs de luminosité d&#39;origine sur la luminosité de la nouvelle couleur.
* **Plage de masques**\
  Le masque est créé en fonction de la combinaison des valeurs suivantes :
  * **&#x200B;**&#x200B;**&#x200B; De Luminosité&#x200B;**: 0-1\
    Plage de luminosité utilisée pour créer le masque **&#x200B;**
  * **De la couleur** : 0-1\
    Plage de couleurs utilisée pour créer le masque
* **Smoothness de masque** : 0-1\
  Réglage de la granularité du masque
* **Flou de masque** : 0-1\
  Flouter le masque

**Masquer**

Ce masque est distinct du masque créé sous **Paramètres de base**. Vous pouvez utiliser un masque personnalisé pour peindre ou utiliser une image pour spécifier les zones à affecter par le filtre **Remplacement de couleur** dans son ensemble.

* **Utiliser un masque personnalisé** : activer/désactiver\
  Activez ou désactivez l’utilisation d’un masque personnalisé. Si cette option est activée, les paramètres suivants apparaissent :
  * **Masque** : image/pinceau\
    Sélectionnez une image à utiliser comme masque ou utilisez le pinceau pour peindre un masque personnalisé directement dans la vue 2D
  * **Masque personnalisé - Flou** : 0-1\
    Flouter le masque
  * **Masque personnalisé - Inverser** : activer/désactiver\
    Inverser le masque

## Guide d’utilisation

Le filtre **Remplacement de couleur** est un excellent moyen de modifier l&#39;apparence de vos matériaux. Par exemple, utilisez-le pour transformer une rouille de fer en cuivre oxydé

Le filtre fonctionne en créant d’abord un masque basé sur les valeurs de luminosité et de couleur d’un point choisi, puis en remplaçant la couleur de la zone définie par ce masque. Pour utiliser le filtre :

1. Ajoutez le filtre **Remplacement de couleur** à la pile de calques
1. Déterminez la couche à utiliser pour créer le masque et la couche dont vous souhaitez remplacer la couleur
   1. Si vous souhaitez baser le masque sur une couche mais remplacer la couleur d&#39;une autre, activez la **Segmentation avancée** et sélectionnez les couches respectives.
   1. Si vous souhaitez baser le masque sur une couche et remplacer la couleur de la même couche, laissez **Segmentation avancée** désactivé.
1. Déplacez le contrôle dans la **vue 2D** sur la couleur que vous souhaitez remplacer.
1. Ajustez les zones couvertes par le masque à l&#39;aide des commandes **Plage de masque**, **Smoothness du masque** et **Flou du masque**.
1. Sélectionnez une **couleur cible** et réglez la **variation de luminosité** jusqu&#39;à ce que vous soyez satisfait de l&#39;effet.
1. Ajoutez éventuellement un masque personnalisé pour appliquer uniquement les effets du filtre dans les zones choisies. Le masque personnalisé n’a aucune incidence sur le masque créé à l’étape 1. Il s’agit plutôt d’un masque supplémentaire que vous pouvez utiliser pour ajuster davantage l’endroit où l’effet est appliqué.

Parfois, il peut être utile d&#39;utiliser plusieurs **filtres de remplacement de couleur** les uns sur les autres pour créer des effets plus avancés.
