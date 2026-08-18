---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/hdri-tools/hdr-merge.html"
breadcrumb-title: ''
description: Utilisez l’outil Fusion HDR de Substance 3D Sampler pour fusionner plusieurs images d’exposition en une seule image de plage dynamique élevée.
helpx_creative_field: ""
helpx_description: Sampler > Filters > HDRI Tools > HDR Merge
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Fusion en HDR
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 2%

---


# Fusion en HDR

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/S_HDRMerge_18_N_D.png)

**Entrées :** Outils HDRI

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Le **filtre de fusion HDR** **filtre** vous permet de fusionner une collection d’images SDR (Plage dynamique standard) pour créer une image HDR.

Les images ci-dessous montrent les résultats de la **fusion HDR**.

![](../../assets/3d-2d-filters-cropped-0027-hdr-merge-in.jpg)

Avant que la **fusion HDR** ne soit terminée, la sphère dans la **vue 3D** reflète la lumière d&#39;environnement par défaut. La **vue 2D** affiche par défaut les données d&#39;image importées pour la première image numérisée, qui est dans ce cas l&#39;image exposée la plus basse.

![](../../assets/3d-2d-filters-cropped-0026-hdr-merge-out.jpg)

Après l&#39;ajout du **filtre de fusion HDR** **filtre**, la sphère reflète une nouvelle luminosité de l&#39;environnement : l&#39;image HDR générée à partir des images d&#39;entrée.

</td>
</tr>
</table>

## TParameters

**Paramètres de base**

* **Delta d&#39;exposition en entrée (EV)** : 0-2\
  Définissez la différence d’exposition entre les expositions en entrée les plus élevées et les plus basses. Un delta d’exposition élevé augmente le contraste résultant de l’opération de fusion.
* **Exposition automatique de sortie** : activer/désactiver\
  Activez ou désactivez le réglage automatique de l’exposition.
* **Décalage de l&#39;exposition de sortie (EV)** : -5 à 5\
  Décalage de l’exposition.

## Guide d’utilisation

Regardez ceci pour savoir comment utiliser le **filtre de fusion HDR** ainsi que d&#39;autres filtres qui peuvent aider à convertir des images SDR en éclairage d&#39;environnement HDR.

Les étapes de base pour utiliser le **filtre** Fusion HDR **HDR** sont les suivantes :

1. Importez l’ensemble d’images à fusionner dans la pile de calques.
1. Ajoutez le **filtre de fusion HDR** à la pile de calques.
1. Modifiez les paramètres pour vous assurer que les valeurs d’exposition sont correctes.
