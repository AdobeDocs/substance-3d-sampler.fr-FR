---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/tools/atlas-splitter.html"
breadcrumb-title: ''
description: Utilisez l’outil Atlas splitter de Substance 3D Sampler pour diviser les atlas de textures en cartes de textures individuelles pour l’édition de matériaux.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Atlas Splitter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Atlas splitter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---


# Atlas splitter

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-atlassplitter-18-n-d.png)

Outils **In:**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

L&#39;**Atlas splitter** est un outil utile pour organiser et afficher les éléments d&#39;un atlas.

Les images ci-dessous montrent l&#39;**Atlas splitter** en action.

![](../../assets/3d-2d-filters-cropped-0039-atlas-splittter-in.jpg)

L’image ci-dessus montre un matériau atlas ajouté à la pile de calques. utilisez l&#39;**Atlas splitter** pour sélectionner des éléments spécifiques dans l&#39;atlas.

![](../../assets/3d-2d-filters-cropped-0038-atlas-splitter-out.jpg)

Avec l&#39;**Atlas splitter** ajouté à la pile de calques, il est possible de se concentrer sur une seule feuille ou tout autre élément du matériau de l&#39;atlas.

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Mode Grille** : basculer\
  Basculer entre le mode Grille et le mode Individuel des éléments. Si cette option est activée, les paramètres supplémentaires suivants apparaissent :
  * **Opacité de la grille** : 0-1\
    Modifier l’opacité de la grille
  * **Opacité de la sélection de grille** : 0-1\
    Modifier l’opacité de la bordure autour de l’élément sélectionné
  * **Mise à l&#39;échelle automatique** : basculement\
    Indiquez si les éléments d’atlas doivent être mis à l’échelle pour remplir chaque carré de grille ou non.
* **Recadrage automatique** : basculer\
  Indiquez si le recadrage de la forme sélectionnée doit être ajusté. Si cette option est activée, une option supplémentaire s’affiche :
  * **Mode de recadrage automatique** :\
    Choisissez la façon dont l’élément sélectionné est recadré pour remplir l’espace du matériau.
* **Sélection de forme** : 1-10\
  Modifiez l’élément de l’atlas sélectionné. Pour les atlas contenant plus de 10 éléments, vous pouvez saisir un nombre dans la valeur **Sélection de forme** pour modifier la plage du curseur.
* **Rotation** : 0-1\
  Rotation d’éléments

**Paramètres avancés**

* **Tolérance de petite forme** : 0-1\
  Ajustez la taille minimale des formes à prélever par l&#39;**Atlas splitter**. Ceci est utile pour filtrer les artefacts
* **Rotation automatique** : activer/désactiver\
  Si cette option est activée, les éléments pivotent automatiquement pour avoir des orientations similaires.
* **Réduire le masque d&#39;opacité** : 0-4\
  Réglez l’échelle du masque d’opacité. Notez que l’augmentation de cette valeur peut diminuer la qualité du masque d’opacité.
* **Précision de la détection de forme** :\
  Sélectionnez l’algorithme de détection de forme à utiliser.
* **Largeur de dilatation** : 0-32\
  Modifier la dilatation : cette opération extrude les couleurs des bordures d’élément dans la zone masquée pour éviter les problèmes de transparence au bord des éléments de l’atlas. Affichez la couche de couleur de base dans la **vue 2D** pour voir les résultats.
* **Couleur d&#39;arrière-plan personnalisée** : activer/désactiver\
  Si cette option est activée, une commande apparaît pour modifier la couleur d’arrière-plan de la couche normale :
  * **Couleur normale** : sélection de la couleur\
    Sélectionnez la couleur d’arrière-plan personnalisée de la couche normale dans les parties transparentes du matériau.
* **Couleur Height Bg** : 0-1\
  Réglez la couleur d’arrière-plan de la couche height. Il est généralement judicieux que l’arrière-plan de l’height corresponde à l’height moyen des bordures des éléments de l’atlas, afin d’éviter les artefacts aux bordures des éléments.
