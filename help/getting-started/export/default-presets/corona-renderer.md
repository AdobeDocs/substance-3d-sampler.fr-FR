---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/getting-started/export/default-presets/corona-renderer.html"
breadcrumb-title: ''
description: Découvrez comment exporter des matériaux à partir de Substance 3D Sampler à l’aide du paramètre prédéfini de rendu Corona pour les workflows de visualisation architecturale.
helpx_creative_field: ""
helpx_description: Sampler > Getting Started > Export > Default Presets > Corona Renderer
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Système de rendu Corona
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '91'
ht-degree: 2%

---


# Système de rendu Corona

| Paramètre prédéfini | Compatibilité | Description de la sortie du packing |
| --- | --- | --- |
| Système de rendu Corona | <ul data-preserve-html="true"><li data-preserve-html="true">PBR Métallique/Rugosité</li><li data-preserve-html="true">SPECULAR/brillance PBR</li></ul> | **Diffuse****ReflectionGlossiness** (\*)**ReflectionColor** (\*\*)**FresnelIOR** (\*\*\*)**Normal ****Displacement****&#x200B;Émissif****Opacité** |

>[!NOTE]
>
> **(\*)** Reflet brillance : version carrée du canal de brillance (brillance \* brillance)
> 
> **(\*\*)** Couleur de reflet : exportez une carte où le blanc indique des matériaux diélectriques et d’autres couleurs pour les matériaux métalliques
> 
> **(\*\*\*)** IOR Frenesl : 1 divisé par la valeur ior, ior est généré à partir de la carte métallique : 1,4 pour les diélectriques, 100 pour les métaux (couleur noire)
