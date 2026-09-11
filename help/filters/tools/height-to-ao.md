---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/tools/height-to-ao.html"
breadcrumb-title: ''
description: Utilisez l’outil Height vers AO dans Substance 3D Sampler pour convertir des maps height en cartes d’ambient occlusion pour la création de matériaux.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Height to AO
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Height à AO
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 1%

---


# Height à AO

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-hbao-18-n-d.png)

Outils **In:**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Générer une carte d&#39;Ambient occlusion à partir des données d&#39;height et normales.

Voir les résultats du **Height du filtre AO** dans les images ci-dessous.

![](../../assets/3d-2d-filters-cropped-0025-height-to-ao-in.jpg)

Dans l&#39;image ci-dessus, la **Vue 2D** affiche la map height. Le matériau n’inclut aucune information sur l’Ambient occlusion dans cette image.

![](../../assets/3d-2d-filters-cropped-0024-height-to-ao-out.jpg)

Dans cette image, le mappage d&#39;Ambient occlusion a été créé par le filtre **Height à AO** et est visible dans la **Vue 2D**. L&#39;Ambient occlusion est généralement un effet subtil. Il n&#39;est donc pas très facile à voir dans ce matériau. Essayez d&#39;utiliser le **filtre Height à AO** sur vos matériaux pour augmenter l&#39;intensité de l&#39;AO et vous familiariser avec l&#39;Ambient occlusion.

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Mode** :\
  Indiquez si les données doivent être générées à partir de la couche height, de la couche normale ou des deux couches ensemble.
* **Ambient occlusion - Intensité** : 0-1\
  Régler la force des données d’IA générées
* **Ambient occlusion - Planche** : 0-1\
  Réglage du rayon des données d’IA générées
