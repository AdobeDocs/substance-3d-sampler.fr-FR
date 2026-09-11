---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/adjustments/color-variation.html"
breadcrumb-title: ''
description: Utilisez le filtre Variation de couleur de Substance 3D Sampler pour ajouter de la diversité et de la variation de couleur aux textures afin de rendre les matériaux plus naturels.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Adjustments > Color Variation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Variation de couleur
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 1%

---


# Variation de couleur

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-colorpalette-18-n-d.png)

**Entrée :** Réglages

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Le filtre Variation de couleur vous permet de remplacer simultanément plusieurs couleurs dans la base color ou la couche de diffusion. Cela est similaire au **filtre Remplacement de couleur**, mais bien que la **variation de couleur** vous permette d&#39;ajuster plusieurs couleurs dans un seul filtre, le **Remplacement de couleur** vous donne plus de contrôle sur le masque utilisé pour remplacer les couleurs et peut être utilisé sur plusieurs couches.

Dans les images ci-dessous, le **filtre Variation de couleur** a été utilisé pour ajuster non seulement la couleur blanche sous-jacente afin de lui donner l&#39;aspect d&#39;une turquoise pâle, mais également pour augmenter le contraste de nombreuses petites taches.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0047-color-variation-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0046-color-variation-out.jpg){width="200px"}

</td>
</tr>
</table>

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Nombre de couleurs** : 1-10\
  Modifier le nombre de couleurs qui remplaceront les couleurs de la couche
* **Variation de luminosité** : 0-1\
  Réglez l’impact de la couleur remplacée sur les valeurs de luminosité
* **Segmentation** :\
  Basez le masque utilisé pour appliquer des couleurs sur une autre couche.
* **Mode Choix de couleur** :\
  Choisissez de sélectionner les couleurs source manuellement ou automatiquement. Si le mode de sélection **manuelle** est choisi, utilisez les poignées de la **Vue 2D** pour sélectionner les couleurs.
  * **Afficher l&#39;Assistant du texte** : activer/désactiver\
    Cette commande n&#39;est visible que si le **mode Choix de couleur** est défini sur **manuel**. Lorsque cette option est activée, l&#39;option **Afficher l&#39;Assistant du texte** ajoute des étiquettes de texte aux poignées de la **Vue 2D** pour distinguer plus facilement les poignées de choix de couleur
* **Couleur X** : sélection de couleur\
  Le nombre de commandes de couleur disponibles dépend de la valeur sélectionnée avec **Nombre de couleurs**. Pour chaque couleur, sélectionnez la nouvelle couleur pour remplacer la couleur de matériau d’origine.

## Guide d’utilisation

Le **filtre Variation de couleur** vous permet de modifier rapidement plusieurs couleurs de la couche de base color à la fois. Pour certains matériaux, cela peut être utile pour effectuer de petits réglages, mais le **filtre Variation de couleur** est idéal pour retoucher complètement les couleurs de votre matériau avec un seul filtre.

Pour utiliser le **filtre Variation de couleur** :

1. Ajoutez le **filtre Variation de couleur** à la pile de calques
1. Ajustez le nombre de couleurs à remplacer avec **Nombre de couleurs**. Le filtre remplacera toute la couleur de la couche. La commande **Nombre de couleurs** vous permet de définir le nombre de nouvelles couleurs par lesquelles les couleurs existantes seront remplacées.
1. Sélectionnez éventuellement une **segmentation** ou un canal différent sur lequel baser les couleurs. Par exemple, vous pouvez sélectionner la couche métallique et utiliser **Mode Choix de couleur > Manuel** pour placer une poignée sur une valeur métallique noire et une autre sur une valeur métallique blanche. Avec cette configuration, vous pouvez contrôler individuellement la couleur des parties métalliques et non métalliques de votre matériau.
1. Sélectionnez un **mode de Choix de couleur**. Lorsque le mode manuel est sélectionné, des poignées apparaissent dans la **Vue 2D** pour vous permettre de sélectionner la base color d&#39;origine que la nouvelle couleur remplacera. Activez **Afficher l&#39;Assistant du texte** pour suivre quelle poignée est liée à quelle couleur.
1. Modifiez les valeurs de couleur avec les commandes **Couleur 1 - 10**.
1. Réglez la **variation de luminosité** pour déterminer l&#39;impact du remplacement de couleur sur la luminosité. Avec une **variation de luminosité** faible, vous pouvez aplatir complètement les couleurs de votre matériau ou utiliser une **variation de luminosité** élevée pour conserver les détails des couleurs d&#39;origine.
