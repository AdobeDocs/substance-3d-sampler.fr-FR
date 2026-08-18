---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/generators/weave.html"
breadcrumb-title: ''
description: Utilisez le générateur d’armure de Substance 3D Sampler pour créer des motifs et des textures de tissu pour la création de matériaux.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Weave
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Tisser
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---


# Tisser

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

Générateurs De **Entrée :**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Utilisez le filtre Tissage pour convertir des images en motifs tissés.

</td>
</tr>
</table>

## Paramètres

**Paramètres prédéfinis**

Utilisez des paramètres prédéfinis pour modifier rapidement les paramètres afin d’afficher différents styles d’armure.

**Paramètres de base**

* **Générateur aléatoire** :\
  Valeur de départ aléatoire sur laquelle sont basés tous les autres paramètres aléatoires de ce filtre.
* **Image** : image/pinceau\
  Sélectionnez une image ou peignez directement dans la **vue 2D**. Le **filtre de tissage** fonctionne mieux lorsqu&#39;une image est sélectionnée.
* **Nombre de couleurs** : 1-10\
  Le **filtre de tissage** décompose automatiquement l&#39;entrée d&#39;image en un certain nombre de couleurs en fonction de ce paramètre. Les paramètres de chaque couleur peuvent être contrôlés indépendamment.
* **Taille de la zone (cm)** : 2-50\
  Modifiez la taille physique représentée par l’espace 2D. Cela modifiera le nombre de points utilisés pour recréer l’image d’entrée.
* **Densité (points par cm)** : 1-105\
  Utilise la commande **Taille de la zone (cm)** pour ajuster le nombre de points dans l&#39;espace 2D.
* **Rugosité globale** : 0-1,0\
  Régler la rugosité du matériau
* **Mode de couleur de trame** :\
  Indiquez si la couleur de la trame dépend de l’image saisie ou des couleurs personnalisées sélectionnées. Si **Remplacement par couleur** est sélectionné, un paramètre **Couleur** supplémentaire apparaîtra dans chaque couleur.

**Couleur X**

Le nombre de couleurs disponibles à modifier dépend de **Paramètres de base > Nombre de couleurs**.

* **Couleur** : sélection de couleur\
  Disponible uniquement si **Paramètres de base > Mode de couleur de trame** est défini sur **Remplacement par couleur**. Choisissez la couleur du matériau pour cette section.
* **Taille de la bordure** : 0-1\
  Ajoutez une bordure sur les bords de la couleur sélectionnée. La bordure augmente la longueur de la trame entre les fils de déformation près du bord de la couleur, évitant ainsi que les points de déformation n’apparaissent près du bord des jeux de couleurs.
* **Décalage de la rugosité** : 0-1\
  Modifier la rugosité de ce jeu de couleurs
* **Métallique** : 0-1\
  Modifier la valeur métallique de ce jeu de couleurs
* **Position Height** : 0-1\
  Réglez l’height de ce jeu de couleurs. Utilisez ceci pour ajouter de la profondeur à la version tissée de votre image.

**Avancé**

* **Couleur de déformation** : sélection de couleur\
  Modifiez la couleur des fils de déformation (par défaut, les fils de déformation s’étendent perpendiculairement aux fils les plus visibles).
* **Déformation - Permutation de trame** :\
  Permutez les fils de déformation et de trame. Ceci a pour effet de faire pivoter les mailles de 90 degrés,
* **Arbres de déformation** : 1-16\
  Ajustez la fréquence relative des filetages de déformation en filetages de trame. Permet de créer différents motifs jacquard.
* **Taille de déformation** : 0-1\
  Augmentez ou diminuez l’épaisseur des filetages de déformation
* **Intensité du flou de la différence d&#39;Height** : 0-1\
  Contrôlez la pente ou le flou causé par les différences de **position de l&#39;Height**. Cela n&#39;a aucun effet, sauf si vous modifiez le curseur **Position de l&#39;Height** pour au moins un jeu de couleurs.

## Guide d’utilisation

Le filtre Tissé peut être un peu confus au début, mais avec quelques paramètres importants pour commencer, vous allez bientôt créer des tissages complexes à ajouter à vos matériaux.

>[!NOTE]
>
> Si vous avez déjà utilisé le filtre [Broderie](embroidery.md)auparavant, le filtre Tissage fonctionne de manière similaire. Ils produisent des effets différents, mais vous pouvez utiliser des images avec eux de la même manière.
> 
> Les images pour le tissage doivent avoir des proportions carrées, une haute résolution (2 Ko minimum) et comporter au maximum 10 couleurs différentes. La couche alpha ou de transparence peut être utilisée pour découper des formes. Idéalement, ils sont vectoriels, mais exportés au format bitmap PNG.

Pour utiliser le filtre Tissage :

1. Glisser-déposer une image dans
1. Ajoutez le filtre Tissage à votre pile de calques.
1. Ajustez **Paramètres de base > Nombre de couleurs** jusqu&#39;à ce que la balance des couleurs soit correcte pour votre image. Avec une limite de 10 couleurs, le filtre Tissé fonctionne mieux avec les couleurs plates et les images illustrées.
1. Réglez d’autres paramètres pour affiner l’apparence de votre correctif.

Il s’agit des principes de base de l’utilisation du filtre Tissage.

Il est possible d&#39;utiliser des images transparentes dans le filtre Tissage, mais par défaut, elles auront également un impact sur la carte d&#39;opacité de votre matériau. Les parties transparentes de l&#39;image rendront également le matériau transparent. Utilisez le filtre Décalcomanie pour créer une pièce avec le filtre Tissage et la placer sur les calques situés en dessous.

1. Créez un filtre Décalcomanie.
1. Ajoutez le filtre Tissage à l’emplacement d’entrée du filtre Décalcomanie.
1. Suivez les étapes normales pour ajuster le motif d’armure.

Le calque de la décalcomanie convertit l’entrée Tissage en décalcomanie. La transparence du calque de la décalcomanie indique donc au calque de la décalcomanie comment masquer le motif tissé. Avec le calque Décalcomanie, vous pouvez également déplacer le motif sur votre matériau ou activer des fonctionnalités telles que la mosaïque.
