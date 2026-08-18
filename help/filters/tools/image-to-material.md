---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/tools/image-to-material.html"
breadcrumb-title: ''
description: Utilisez l’outil Image vers matériau de Substance 3D Sampler pour convertir des images uniques en matériaux PBR complets à l’aide d’un traitement optimisé par IA.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Image To Material
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Image en matériau
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 1%

---


# Image en matériau

![](../../assets/sat-icon-image-to-material.png)

Le modèle **Image vers matériau** permet de générer un matériau PBR de haute qualité à partir d&#39;une image en entrée unique.

Ce modèle comporte deux algorithmes principaux :

* **Optimisé par l&#39;IA**
* **B2M**

Voir ci-dessous pour une explication détaillée de chaque algorithme.

## Exemple

Voici un exemple de couches de matériau générées à partir d’une seule image d’entrée :

![](../../assets/sat-image-to-material.jpg){width="500px"}

## Algorithmes

Pour modifier l&#39;algorithme du modèle **Image en matériau**, cliquez sur le menu déroulant sous le nom du modèle :

![](../../assets/image-to-material-algo-setting.png)

### Basé sur l&#39;IA

L&#39;algorithme <b>optimisé par l&#39;IA</b> utilise le machine learning pour reconnaître les formes et les objets et générer avec précision des cartes de normales, d&#39;Height et de rugosité, ainsi que pour éliminer les albédos des ombres ou des hautes lumières.

Le réseau neuronal a été formé sur une large gamme de matériaux tels que les tissus, les matières organiques, les surfaces intérieures et extérieures.

>[!NOTE]
>
> Le traitement Image vers matériau (optimisé par l&#39;IA) prendra plus de temps sur les images haute résolution. Nous vous recommandons d&#39;utiliser le système [Layer Resolution](../../interface/preferences/layer-resolution.md) pour optimiser votre workflow pendant votre travail.

### B2M

L&#39;algorithme **B2M** utilise la méthode Bitmap to Material basée sur la Substance pour générer plusieurs couches, telles que la couleur de base, la normale, la métallique, la rugosité et l&#39;occlusion ambiante, à l&#39;aide de techniques procédurales.

Cet algorithme peut produire des résultats moins précis, mais fonctionnera sur une plus large gamme d’images en entrée.

## Adobe Capture

Cette fonctionnalité est également disponible sur l’application mobile Adobe Capture (Android et iOS). Vous pouvez prendre une photo où que vous soyez et obtenir un aperçu du résultat directement sur votre téléphone.

Envoyez facilement les résultats à Substance 3D Sampler pour d’autres éditions.

![](../../assets/capture-qr-code.gif)

>[!NOTE]
>
> Cette fonctionnalité est uniquement disponible avec un abonnement Substance 3D Collection Adobe.
