---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/tools/upscale.html"
breadcrumb-title: ''
description: Utilisez l’outil Upscale de Substance 3D Sampler pour augmenter la résolution de la texture à l’aide de la technologie d’upscaling optimisée par l’IA.
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Upscale
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 2%

---


# Upscale

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![Icône De Filtre](../../assets/SAPR_SuperResolution_18_N_D.png)

Outils **In:**

</td>
<td style="border: 0;" valign="top">

## Description

Le filtre <b>Upscale </b>utilise l’IA pour suréchantillonner les canaux PBR (Couleur de base, Rugosité, Normal, Métallique, Height) à partir des calques situés en dessous.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">



</td>
<td style="border: 0;" valign="top">

![](../../assets/F5W_vAHaYAQLsz7.jpg)

</td>
</tr>
</table>

Dans cet exemple, nous commençons par une image de 1 024 x 1 024 px, mais le résultat de sortie est de 4 098 x 4 098 px. Les résultats utilisant le filtre <b>Mise à l&#39;échelle</b> sont plus définis.

</td>
<td style="border: 0;" valign="top">

>[!NOTE]
>
> **Filtre avancé**
> 
> L&#39;<b>agrandissement</b> est un filtre avancé.\
> Pour l&#39;utiliser à sa capacité maximale et éviter les résultats flous, nous vous recommandons de définir les calques sous le <b>niveau supérieur</b> dans Entrée de calque max. ou Entrée de calque min.
> 
> Il n&#39;y a aucune limite quant au nombre de filtres <b>Upscale </b>pouvant être utilisés, mais un suréchantillonnage au-dessus de la résolution 8k peut avoir un impact significatif sur les performances.

</td>
</tr>
</table>

## Paramètres

<b>Paramètres de base</b>

* <b>Exemple supérieur</b> : activer/désactiver le groupe de boutons\
  Choisir le facteur de multiplication à augmenter

## Comment

![](../../assets/SAPR_Upscale_screen_001.png)

Dans l&#39;image ci-dessus, une image basse résolution est traitée par [Image vers matériau (optimisé par l&#39;IA)](image-to-material.md).

![](../../assets/SAPR_Upscale_Screen_003.png)

Le filtre <b>Upscale</b> est ajouté pour échantillonner les résultats. Il halucine les détails afin d&#39;atteindre une résolution plus élevée tout en conservant la qualité du matériau. Vous pouvez choisir dans les propriétés de sur-échantillonner par 2 ou par 4.
