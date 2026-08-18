---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/generators/atlas-scatter.html"
breadcrumb-title: ''
description: Utilisez le générateur d’Atlas scatter de Substance 3D Sampler pour dispersion des éléments à partir d’atlas de textures sur des surfaces de matériau.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Atlas Scatter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Atlas scatter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 0%

---


# Atlas scatter

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/S_AtlasScatter_18_N_D.png)

Générateurs De **Entrée :**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Le filtre Atlas scatter dispersion les instances des éléments d’un matériau atlas sur le matériau sous-jacent. Les Atlas scatters sont utiles pour disperser naturellement des éléments tels que des feuilles, des rochers ou des déchets sur un matériau.

Les images ci-dessous montrent le **filtre d&#39;Atlas scatter** en action.

![](../../assets/3d-2d-filters-cropped-0037-atlas-scatter-in.jpg)

Avant d&#39;utiliser le **filtre Atlas scatter**, nous avons un matériau de boue de base, pas très excitant.

![](../../assets/3d-2d-filters-cropped-0036-atlas-scatter-out.jpg)

En ajoutant le **filtre Atlas scatter** avec un atlas de galets, le matériau devient plus intéressant car les galets sont dispersés et se mélangent de manière réaliste à la boue sous-jacente.

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **X Quantité** : 1-64\
  Nombre d’instances sur l’axe X
* **Quantité Y** : 1-64\
  Nombre d’instances sur l’axe Y
* **Mode de fusion** :\
  Méthode de fusion avec les calques sous-jacents
* **Échelle** : 0-5\
  Échelle des instances
* **Position aléatoire** : 0-2\
  Augmente ou diminue le décalage aléatoire des instances par rapport aux positions de la grille
* **Échelle D&#39;Height** : 0-1\
  Régler l’height des instances
* **Se conformer à l&#39;arrière-plan** : 0-1\
  Modifier l’impact des valeurs d’height sous-jacentes sur les instances disséminées
* **Couleur d&#39;arrière-plan** :
  * **Teinte :** 0-1\
    Réglage de la teinte des instances
  * **Saturation :** 0-1\
    Réglage de la saturation des instances
  * **Valeur :** 0-1\
    Ajuster la valeur des instances

**Masquer**

* **Masque personnalisé** : activer/désactiver\
  Activez ou désactivez l’utilisation d’un masque personnalisé. Lorsque cette option est activée, les commandes suivantes apparaissent :
  * **Masque personnalisé :**\
    Sélectionnez un fichier à utiliser comme masque ou utilisez le mode Pinceau pour masquer manuellement.
  * Activer/Désactiver **Inverser le masque :**\
    Inverser la valeur du masque
* **Aléatoire du masque** : 0-1\
  Masquage aléatoire d’un pourcentage d’instances

**Taille**

* **Échelle aléatoire** : 0-1\
  La quantité d’échelle aléatoire à appliquer à chaque instance
* **Aucun Chevauchement D&#39;Échelle** : 0-1\
  Réglez l’échelle de chaque instance pour éviter le chevauchement d’instances

**Height**

* **Décalage Height** : -1 à 1\
  Décalage de l&#39;height des instances par rapport au niveau de base 0
* **Décalage Height aléatoire** : 0-1\
  Ajout d’une valeur aléatoire au décalage d’height pour chaque instance
* **Inclinaison par rapport à la Pente principale** : 0-1\
  Ajustement de l’inclinaison des normales en fonction de la pente de l’arrière-plan
* **Smoothness en arrière-plan** : 0-2\
  Ajuster le Smoothness de l’arrière-plan

**Rotation**

* **Rotation** : 0-1\
  Rotation de toutes les instances selon une valeur définie
* **Rotation Aléatoire** : 0-1\
  Ajouter une valeur aléatoire à la rotation de chaque instance
* **Rotation à partir de la grande Pente** :\
  Rotation d’instances en fonction de la pente de la matière sous-jacente

**Réglages Des Matériaux Atlas**

* **Réglage des couleurs** :\
  Réglage des valeurs TSL pour l’atlas
* **Color Random** :\
  Ajoutez du caractère aléatoire aux valeurs HSV définies dans **Réglage des couleurs**
* **Rugosité de l&#39;arrière-plan** : 0-1\
  Utilisez la rugosité de l’arrière-plan au lieu de la rugosité de chaque occurrence.
* **Réglage de la rugosité** : -1 à 1\
  Ajouter ou soustraire de chaque occurrence des valeurs de rugosité.
* **Aléatoire normal** : 0-1\
  Faire pivoter les normales de chaque occurrence d’une valeur aléatoire par occurrence
* **Recalculer l&#39;Occlusion ambiante** : activer/désactiver\
  Si cette option est activée, les valeurs d’Occlusion ambiante sont recalculées en fonction des valeurs d’height modifiées

**Détection de forme Atlas**

* **Plage de motifs** :\
  Limitez les ressources disponibles de l’atlas en fonction de la position. Laissez les valeurs X et Y à 0 pour utiliser toutes les ressources de l’atlas.
* **Opacité de l&#39;atlas de réduction** : 0-4
* **Précision de la détection de forme** :\
  Sélectionnez l’algorithme de détection des formes. Différents atlas seront adaptés à différents algorithmes de détection. Aucun mode de défaillance n’est plus coûteux en termes de calcul que les autres options.
* **Ignorer la forme inférieure à** : 0-1\
  Utilisez cette option pour éviter d’utiliser de très petites formes comme éléments individuels.

Guide d’utilisation

Le filtre Atlas scatter est un moyen utile de mettre en dispersion des ressources dans votre matériau, telles que des feuilles, des pierres ou des déchets. Pour utiliser le filtre Atlas scatter, vous aurez besoin d’un atlas de matières à traiter.

>[!NOTE]
>
> Un atlas est un matériau qui contient une collection (ou un atlas) de ressources distinctes. Par exemple, Sampler inclut par défaut les feuilles de laurier séché - il s&#39;agit d&#39;un matériau de l&#39;atlas car il contient une collection de feuilles dans un seul matériau où chaque feuille est séparée de l&#39;autre feuille. Le nœud d&#39;Atlas scatter utilise un algorithme pour traiter chaque feuille du matériau de l&#39;atlas comme un élément séparé.

Pour utiliser le filtre Atlas scatter :

1. Ajout du filtre Atlas scatter à la pile de calques
1. Sous le calque Atlas scatter, un emplacement Entrée apparaît
1. Faites glisser votre matière atlas dans l’emplacement d’entrée Atlas scatter

Vous pouvez ajuster les paramètres de dispersion dans le **panneau Propriétés** en sélectionnant le calque d&#39;Atlas scatter.

Vous pouvez ajuster les paramètres du matériau de l&#39;atlas dans le **panneau Propriétés** en sélectionnant le matériau dans l&#39;emplacement d&#39;entrée.
