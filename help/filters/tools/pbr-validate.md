---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/tools/pbr-validate.html"
breadcrumb-title: ''
description: Utilisez l’outil Validation PBR de Substance 3D Sampler pour valider les normes de rendu physiques et vous assurer que les matériaux sont conformes à ces normes.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > PBR Validate
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Validation PBR
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---


# Validation PBR

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-pbrvalidate-18-n-d.png)

Outils **In:**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Utilisez le **filtre Validation PBR** pour vous assurer que les valeurs PBR de votre matériau sont correctes. Contrairement à la plupart des filtres, le **filtre Validation PBR** ne doit pas faire partie intégrante de la pile de calques. Utilisez-le plutôt pour valider votre matériau, puis supprimez-le afin qu&#39;il ne modifie pas votre matériau.

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Mode de validation** :\
  Indiquez si vous souhaitez valider des valeurs d’albédo (base color ou diffusion), des valeurs métallique ou des valeurs albédo et métallique. Les autres paramètres seront mis à jour en fonction de cette sélection
  * **Mode de validation : Albédo**
    * **Seuil de plage d&#39;obscurité Albédo** :\
      Définissez le seuil pour les valeurs sombres à prélever par le filtre comme non valide.
    * **Mappage d&#39;incrustation** : activer/désactiver\
      Basculer entre les modes d’incrustation : si cette option est activée, la carte de base color sera incrustée avec les pixels non valides.
    * **Masquer la validation dans la Base color** : activer/désactiver\
      Masquez les informations de validation du canal de base color.
  * **Mode de validation : Metal**
    * **Plage de réflectance du métal** :\
      Définissez la plage de valeurs de réflectance que le filtre doit sélectionner comme non valide.
    * **Mappage d&#39;incrustation** : activer/désactiver\
      Basculer entre les modes d’incrustation : si cette option est activée, la carte de base color sera incrustée avec les pixels non valides.
    * **Masquer la validation dans la Base color** : activer/désactiver\
      Masquez les informations de validation du canal de base color.
  * **Mode De Validation : Combiné**
    * **Seuil de plage d&#39;obscurité Albédo** :\
      Définissez le seuil pour les valeurs sombres à prélever par le filtre comme non valide.
    * **Plage de réflectance du métal** :\
      Définissez la plage de valeurs de réflectance que le filtre doit sélectionner comme non valide.
    * **Masquer la validation dans la Base color** : activer/désactiver\
      Masquez les informations de validation du canal de base color.

## Guide d’utilisation

Le **filtre** Validation PBR **** permet d&#39;éviter les problèmes d&#39;albédo et de valeurs métalliques dans un matériau. Pour comprendre le fonctionnement du **filtre Validation PBR**, il est utile de parler d&#39;abord un peu de ce qu&#39;est le PBR.

## Qu’est-ce que le PBR ?

PBR est l’acronyme de Physically Based Rendering (Rendu basé sur le physique). Il s’agit d’une méthode de rendu d’objets et de matériaux qui représente les propriétés physiques d’une surface avec différents canaux. PBR a été créé pour représenter plus précisément le monde réel et physique que les méthodes de rendu et d’ombrage précédentes.

Dans le monde réel, il existe certaines couleurs et combinaisons de propriétés qui sont soit impossibles, soit incroyablement rares. Par exemple, presque rien dans le monde réel n&#39;a un albédo ou une base color blanc pur ou noir pur.

Ainsi, puisque PBR tente de représenter des valeurs réelles, et que certaines valeurs n&#39;apparaissent pas ou apparaissent rarement dans le monde réel, il est possible d&#39;avoir des valeurs PBR « incorrectes ». C&#39;est ce que le **filtre Validation PBR** est conçu pour rechercher.

## Comment utiliser Validation PBR

Pour utiliser **Validation PBR**, ajoutez-le en haut de votre pile de calques. Vous devriez constater une modification radicale de l&#39;apparence de votre matériau, car le **filtre Validation PBR** affiche les résultats de la validation dans le canal albédo.

Le filtre utilise une échelle allant du rouge au vert pour indiquer où se situent les erreurs. Si le matériau entier est vert, il n’y a rien de mal avec les couleurs ou les valeurs métalliques de votre matériau. Cependant, si vous voyez des zones jaunes, orange ou rouges, cela signifie que votre matériau présente des problèmes.

Si vous utilisez le mode de validation des couleurs, les zones non vertes signifient généralement que certaines valeurs de votre base color sont proches du noir ou du blanc complet. Utilisez des filtres de réglage tels que **Teinte/Saturation** ou **Luminosité/Contraste** pour ajuster les valeurs de votre couche de couleur jusqu&#39;à ce que le **filtre Validation PBR** ne montre plus d&#39;erreurs.

Si vous utilisez le mode de validation du métal, les zones non vertes signifient généralement que la combinaison de votre couleur, de votre rugosité et des cartes métalliques dans ces zones est irréaliste. Cela se produit généralement avec des valeurs de couleur foncée, 0 rugosité et 1 valeur métallique. Pour corriger ces erreurs, vous pouvez modifier les valeurs de rugosité, de métallique ou de couleur jusqu&#39;à ce que le **filtre Validation PBR** n&#39;affiche plus d&#39;erreurs.
