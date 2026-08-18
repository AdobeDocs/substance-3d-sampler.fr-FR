---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/features-and-workflows/flatten-layers.html"
breadcrumb-title: ''
description: Apprenez à aplatir les calques dans Substance 3D Sampler pour améliorer les performances et simplifier votre pile de calques tout en comprenant l’impact.
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Aplatir les calques
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 1%

---


# Aplatir les calques

L’aplatissement des calques est un moyen utile d’améliorer les performances et de simplifier la pile de calques, mais il est important de connaître l’impact que peut avoir l’aplatissement des calques sur votre projet.

## À quoi sert le bouton Aplatir les calques ?

L’option Aplatir les calques fusionne tous les calques situés sous le calque actuellement sélectionné en un seul calque. Le calque aplati obtenu a le même aspect que les calques d’origine, mais vous ne pouvez plus apporter de modifications aux calques individuels d’origine.

### Pourquoi aplatir les calques ?

Chaque fois que vous modifiez un calque dans la pile de calques, Sampler doit recalculer la sortie de ce calque et de tous les calques situés au-dessus. Chaque couche supplémentaire à calculer signifie un temps de traitement et une utilisation de la mémoire supplémentaires. L’aplatissement de plusieurs calques réduit le temps et la mémoire nécessaires au traitement de ces calques. Par exemple, au lieu de recalculer 10 calques, Sampler n’a besoin de traiter qu’un seul calque.

En outre, l’aplatissement des calques simplifie la pile de calques, ce qui facilite la navigation et la compréhension.

### À quel moment ne devrais-je pas aplatir les calques ?

Tous les calques aplatis ne sont pas accessibles individuellement dans la pile de calques. Vous ne pourrez donc pas modifier les paramètres dans le résultat aplati. Par conséquent, vous ne devez aplatir les calques que si vous n’avez plus besoin de modifier le résultat de ces calques.

## Paramètres du calque aplati

Les paramètres des calques d’origine sont perdus, mais les calques aplatis disposent de leur propre jeu de paramètres que vous pouvez ajuster pour contrôler l’utilisation de chaque couche obtenue.

Pour chaque canal, vous pouvez :

* <b>Utilisation de la sortie</b> : modifiez le canal pour lequel la sortie est utilisée. Lorsque vous aplatissez des calques, un TIFF est créé et nommé pour chaque couche, puis automatiquement affecté à cette couche.
* <b>Opacité à partir de la couche alpha</b> : indiquez si l&#39;opacité dépend du résultat de la couche Alpha.
* <b>Supprimer</b> : supprimez le canal de ce calque. Cela peut être utile pour les canaux qui ne contiennent pas d’informations utiles. Par exemple, il est conseillé de supprimer une couche d’opacité entièrement blanche, car cela libère de la mémoire sans affecter les résultats visuels.
