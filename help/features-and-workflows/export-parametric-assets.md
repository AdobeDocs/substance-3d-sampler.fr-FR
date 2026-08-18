---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/features-and-workflows/export-parametric-assets.html"
breadcrumb-title: ''
description: Découvrez comment exporter des actifs paramétriques depuis Substance 3D Sampler pour permettre la modification de paramètres dans d’autres applications sans revenir à Sampler.
helpx_creative_field: ""
helpx_description: Sampler > Features and workflows > Export parametric assets
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Exportation d’actifs paramétriques
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 1%

---


# Exportation d’actifs paramétriques

Les paramètres exposés peuvent être modifiés dans d’autres applications sans revenir à Sampler. Cela réduit le temps d’itération afin que vous puissiez vous concentrer sur la recherche du meilleur aspect sans avoir à passer d’une application à l’autre.

## Exposer et annuler l’exposition des paramètres

Pour afficher les paramètres, ouvrez le **panneau Propriétés**. Survolez ou cliquez avec le bouton droit sur le paramètre souhaité, puis cliquez sur l&#39;icône en forme d&#39;épingle ou sur « exposer ce paramètre ».

![](../assets/ezgif-com-gif-maker-2.gif)

Il existe deux façons de désexposer un paramètre :

* Dans le **Panneau Paramètres exposés**, cliquez avec le bouton droit sur le paramètre et choisissez « unexposer ».

  ![](../assets/ezgif-com-gif-maker-3.gif)
* Dans le panneau **Propriétés**, cliquez sur l&#39;icône en forme d&#39;épingle croisée ou cliquez avec le bouton droit sur le paramètre et choisissez « désexposer ce paramètre ».

  ![](../assets/ezgif-com-gif-maker-4.gif)

Les paramètres des filtres suivants ne peuvent pas être affichés :

* Image to Material (basé sur l’IA)
* Remplissage d’après le contenu
* Normal à l’Height
* Upscale

Si vous ajoutez l’un des filtres au-dessus des calques qui contiennent des paramètres exposés, ils ne seront pas exposés lors de l’exportation.\
Pour éviter cela, supprimez le filtre ou placez-le à un endroit où il n’affectera pas les calques dont les paramètres sont exposés.

Si vous avez exposé des paramètres d&#39;un dégradé, ils seront perdus si vous déplacez le calque au bas de la pile.

![](../assets/ezgif-com-gif-maker-10.gif)

## Modification des paramètres

Modifiez le libellé de votre paramètre en cliquant dessus avec le bouton droit sur le **Panneau Paramètres exposés**, saisissez le nouveau nom et cliquez sur Appliquer.

![](../assets/ezgif-com-gif-maker-5.gif)

![](../assets/ezgif-com-gif-maker-6.gif)

Vous pouvez utiliser le paramètre dans le **Panneau Paramètres exposés** comme dans le **panneau Propriétés**.

## Exportation de votre matière

Pour exporter votre matière avec vos paramètres exposés

1. Ouvrez le panneau <b>Exporter.</b>
1. Cliquez sur Exporter.
1. Sélectionnez SBSAR ou SBS.
1. Cliquez sur « Exporter ».

Vous pouvez désormais utiliser votre matière avec vos paramètres exposés dans tout logiciel prenant en charge le format de fichier SBSAR.
