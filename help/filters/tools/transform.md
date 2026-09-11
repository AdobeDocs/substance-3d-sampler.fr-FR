---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/tools/transform.html"
breadcrumb-title: ''
description: Utilisez l’outil Transforme de Substance 3D Sampler pour mettre à l’échelle, faire pivoter, translater et manipuler des textures et des calques de matériau.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Transform
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Transformation
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 1%

---


# Transformation

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-transformgeneric-18-n-d.png)

Outils **In:**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Utilisez l&#39;**outil Transforme** pour déplacer, redimensionner ou faire pivoter votre image ou votre matériau.

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Mode de contrôle** :\
  Choisissez d&#39;afficher ou non les paramètres pour contrôler le transforme avec des curseurs en plus des poignées **Vue 2D**.

  Avec **Widget et paramètres** sélectionnés, les commandes supplémentaires suivantes apparaîtront :

  * **Transforme sécurisé** : activer/désactiver\
    Activez ou désactivez les transformations sécurisées. Lorsque cette option est activée, le nœud de transforme conserve la répétition et évite de perdre des détails de pixel en raison de petits décalages et rotations. Cela réduit la liberté dont vous disposez pour contrôler la transformation et l&#39;activation du **Transformé sécurisé** masquera certains paramètres.
  * **Conserver le rapport** : activer/désactiver\
    Lorsque cette option est activée, un seul paramètre **Échelle** est visible pour contrôler la mise à l&#39;échelle sur les deux axes simultanément. Lorsque cette option est désactivée, les commandes permettant de modifier séparément l’échelle sur les axes horizontal et vertical sont disponibles.

    * **Échelle** : 0-1\
      Selon que le paramètre **Conserver le rapport** est activé ou désactivé, 1 ou 2 curseurs seront disponibles pour ajuster l&#39;échelle.
  * **Rotation**; 0-360\
    Faites pivoter l’entrée dans les poignées.
  * **Inclinaison** : -1 à 1\
    Inclinez la saisie dans les poignées sur les axes horizontal et vertical.
* **Décalage de position** : -1 à 1\
  Décalez le transforme par rapport à la position de départ sur les axes horizontal et vertical.
* **Symétrie horizontale** : basculer\
  Symétrie horizontale de l’entrée
* **Symétrie verticale** : basculer\
  Symétrie verticale de l’entrée

**Paramètres avancés**

* **Transformation** :\
  Ajustez la transformation des poignées à l&#39;aide de curseurs au lieu de la **Vue 2D**.
  * **Échelle X** : 0-2
  * **Inclinaison verticale** : -7,44 à 2
  * **Inclinaison horizontale** : 0-1
  * **Échelle Y** : 0 - 13,15
* **Désactiver le Transforme par canal** : basculer\
  Lorsque cette option est activée, des commandes supplémentaires s’affichent pour vous permettre de désactiver ce transforme pour chaque canal.

## Guide d’utilisation

Cliquez sur l&#39;**outil Transforme** pour ajouter un nouveau calque de Transforme en haut de la pile de calques.

La création ou la sélection d&#39;un calque de Transforme ouvre automatiquement la **Vue 2D**. Avec le calque de Transforme sélectionné, une **barre d&#39;outils** apparaît en haut de la **Vue 2D**.

## Fonctionnalité

![](../../assets/alchemist-2020-2-transform-1.gif){width="300px"}

### Déplacer

Pour déplacer le calque :

1. Survol de la souris dans la zone de transforme
1. Votre curseur se transforme en quatre flèches
1. Cliquez et faites glisser pour déplacer la zone de transforme.

### Échelle

Pour mettre le calque à l’échelle :

1. Placez le curseur de la souris sur l’une des poignées situées au bord ou dans l’angle de la zone de transforme
1. Votre curseur se transforme en quatre flèches.
1. Cliquez et faites glisser pour mettre à l’échelle la zone de transforme.

>[!NOTE]
>
> Les poignées situées dans l’angle de la zone de transforme vous permettent de modifier simultanément l’échelle en deux dimensions, tandis que les poignées situées dans le bord de la zone de transforme vous limitent à une seule dimension.

### Rotation

Pour faire pivoter le calque :

1. Survolez votre souris en dehors de la zone de transformé, mais dans la **Vue 2D**.
1. Une petite flèche horizontale apparaît à côté du curseur.
1. Cliquez et faites glisser pour faire pivoter la zone de transforme.

>[!NOTE]
>
> Vous pouvez modifier le centre de rotation en faisant glisser le petit cercle au centre de la zone de transforme. La boîte de transforme tourne toujours autour de ce cercle.

## Barre d’outils

![](../../assets/transform-toolbar.png){width="200px"}

La barre d’outils contient les raccourcis suivants :

* Créer un carré : ajustez l’échelle de la transformation actuelle pour la rendre carrée.
* Rotation +90° (à droite) : rotation de 90° dans le sens des aiguilles d’une montre.
* Rotation -90° (à gauche) : rotation de 90° dans le sens inverse des aiguilles d’une montre.
* Réinitialiser le centre de rotation : réinitialisez le centre de rotation au centre de la zone de Transforme.
* Réinitialiser la transformation : réinitialisez l’outil Transforme à sa position par défaut.
