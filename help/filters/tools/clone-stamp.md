---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/tools/clone-stamp.html"
breadcrumb-title: ''
description: Utilisez l’outil Tampon de Clone de Substance 3D Sampler pour cloner et peinture des zones de texture afin de modifier et réparer le matériau en toute transparence.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Clone Stamp
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Tampon clone
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---


# Tampon clone

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-clonestamp-18-n-d.png)

Outils **In:**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

L&#39;**outil Tampon de Clone** vous aide à dupliquer ou à corriger manuellement des parties de votre matériau. Cela permet de corriger des seams ou de supprimer des erreurs de votre matériau. Le **filtre Tampon de Clone** est l&#39;un des outils disponibles dans la barre latérale gauche.

Les images ci-dessous montrent le **tampon de Clone** utilisé pour retirer les débris d&#39;un matériau à neige.

![](../../assets/3d-2d-filters-cropped-0049-clone-stamp-in.jpg)

Dans l’image ci-dessus, le matériau de neige comprend un certain nombre de brindilles et d’autres débris éparpillés un peu partout.

![](../../assets/3d-2d-filters-cropped-0048-clone-stamp-out.jpg)

L&#39;outil **Tampon de Clone** est utilisé pour supprimer certaines brindilles et les remplacer par de la neige propre.

</td>
</tr>
</table>

## Tutoriel Tampon de clone

## Paramètres

<b>Paramètres de base</b>

* <b>Développer le masque</b> : 0-1\
  Ajustez la distance autour de la zone peinte sur laquelle le filtre tentera de correspondre au matériau sous-jacent.
* <b>Fusion Atténuation</b> : 0-1\
  Adoucissez le bord de la zone clonée pour faciliter la fusion avec le matériau sous-jacent.
* <b>Masque de flou</b> : 0-1\
  Ajustez le niveau de détail du bord du tampon de duplication. Si vous augmentez cette valeur, les bords de la zone clonée auront davantage l’aspect d’une tache.
* <b>Conserver le rapport</b> : activer/désactiver\
  Lorsque cette option est désactivée, elle vous permet d’ajuster les proportions de la zone dupliquée.
  * <b>Horizontal</b> : 0-2
  * <b>Vertical</b> : 0-2
* <b>Rotation</b> : -180 à 180\
  Faites pivoter la zone tamponnée.
* <b>Symétrie horizontale</b> : basculer\
  Permet de refléter la zone tamponnée le long d’un axe horizontal.
* <b>Symétrie verticale</b> : basculer\
  Permet de refléter la zone tamponnée le long d’un axe vertical.

<b>Fusion Atténuation</b>

Utilisez les commandes Fusion Atténuation pour régler individuellement la fusion Atténuation de chaque couche de votre matériau.

<b>Avancé</b>

* <b>Intensité normale</b> : 0-2\
  Ajustez la force des normales dans la zone estampée.
* <b>Position source</b> : \
  0-1 : Ajustez la position horizontale de la source.\
  0-1 : Ajustez la position verticale de la source.
* <b>Position cible</b> :\
  0-1 : Ajustez la position cible horizontale.\
  0-1 : Ajustez la position verticale cible.
* <b>Mode Répétition</b> : liste déroulante\
  Activer ou désactiver la répétition.

## Guide d’utilisation

Cliquez sur l&#39;**outil Tampon de Clone** pour créer un calque de filtre Tampon de Clone en haut de votre pile de calques. Vous pouvez également ajouter un filtre Tampon de Clone à l&#39;aide du **bouton Ajouter un calque** dans le **panneau Calques**.

La création d&#39;un calque de filtre Tampon de Clone ouvre automatiquement la **Vue 2D** dans le **Viewport**. Une **barre d&#39;outils** apparaît en haut de la **Vue 2D** lorsque le calque Tampon de Clone est sélectionné.

![](../../assets/alchemist-2020-2-clone.gif){width="300px"}

Pour commencer à utiliser l&#39;outil Tampon de Clone, cliquez et faites glisser la souris sur la zone problématique dans la **Vue 2D**. Le matériau commencera à se mettre à jour automatiquement en fonction de la source. Les zones dans lesquelles vous utilisez l&#39;**outil Tampon de Clone** sont mises en surbrillance.

## Barre d’outils

<table>
<tr style="border: 0;">
<td width="16.67%" style="border: 0;" valign="top">

![](../../assets/CloneStampBrushToolbar.png)

</td>
<td width="83.33%" style="border: 0;" valign="top">

Lorsque le calque de tampon de Clone est sélectionné, une barre d’outils contenant des commandes supplémentaires s’affiche dans la Vue 2D.

* Sélectionnez l&#39;outil <b>Pinceau </b> pour l&#39;ajouter au masque ou l&#39;outil <b>Effacer </b> pour le supprimer du masque.
* Définissez la taille de l’outil actuellement sélectionné.
* Accéder à des commandes supplémentaires :
  * <b>répétition de pinceau</b> : \
    Activer/désactiver la répétition des pinceaux X et Y.
  * <b>Incrustation :</b>\
    Indique si l’incrustation doit s’afficher lorsque vous survolez la Vue 2D.
* Afficher les commandes vue 2D.

</td>
</tr>
</table>

>[!NOTE]
>
> Comme pour les autres barres d’outils de Viewport, vous pouvez faire glisser la poignée en haut de la barre d’outils pour la repositionner dans le viewport, double-cliquer sur la poignée pour passer du mode vertical au mode horizontal ou utiliser le double chevron pour masquer ou développer la barre d’outils.

## Sélection de source

Utilisez Ctrl + Clic dans la vue 2D pour ajouter une nouvelle source. L&#39;ajout d&#39;une nouvelle source entraîne la création d&#39;un tampon supplémentaire sous le calque Tampon de Clone dans le <b>panneau Calques</b>. Vous pouvez contrôler chaque tampon individuellement.

>[!NOTE]
>
> Il est généralement conseillé d’éviter que le point source ne soit proche de la zone sur laquelle vous dupliquez. Si le point source est proche de la zone problématique, il est possible de cloner la zone problématique.

## Raccourcis

| Action | Windows + Linux | MacOs |
| --- | --- | --- |
| Augmenter l’épaisseur du pinceau | ] ou Ctrl + Molette de la souris | ] ou Cmd + Molette de la souris |
| Diminuer l’épaisseur du pinceau | [ ou Ctrl + Molette de la souris | [ ou Commande + Molette de la souris |
| Définir la source | Ctrl + clic gauche | Cmd + clic gauche |
