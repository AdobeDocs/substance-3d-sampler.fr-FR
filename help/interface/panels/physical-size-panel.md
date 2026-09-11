---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/interface/panels/physical-size-panel.html"
breadcrumb-title: ''
description: Apprenez à utiliser le panneau Taille physique de Substance 3D Sampler pour définir des dimensions réelles pour des matériaux et des textures.
helpx_creative_field: ""
helpx_description: Sampler > Interface > Panels > Physical Size Panel
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Panneau taille physique
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0f989901713dd30f8f936de2445caf5dc70a9225
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 13%

---


# Panneau taille physique

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/3-2-0-cover.png)

</td>
<td width="58.30%" style="border: 0;" valign="top">

Utilisez le **panneau Taille physique** pour configurer la taille physique réelle de vos échantillons et images numérisés.

</td>
</tr>
</table>

Faites correspondre la taille physique réelle de vos échantillons et images numérisés dans un cadre numérique pour créer des visuels physiquement précis dans toutes les applications.\
Les outils et paramètres ci-dessous vous permettent de définir la taille physique de vos matériaux et de créer des visuels précis et réalistes lors de l’application de matériau sur un objet.

## Définir la taille physique

>[!NOTE]
>
> Pour définir la Taille physique de votre matériau, vous devez disposer d’un calque d’importation d’image.

Pour calculer la taille physique de votre échantillon/image, activez **Définir la taille physique**.

### Taille de l&#39;image d&#39;entrée

Cette section vous permet de définir manuellement la taille de votre échantillon et fournit des outils pour calculer automatiquement la taille physique.

**Calque de référence :** référencez l&#39;image à partir de laquelle la taille physique est calculée.\
**Largeur (X) :** définissez la largeur physique du calque de référence\
**Height(y):** Définissez l&#39;height physique du calque de référence\
**Outils :**

![](../../assets/screenshot-2022-01-17-at-13-59-37.png)

L&#39;outil Diagnostics de mesure vous permet de mesurer la distance entre deux points de votre image (à titre d&#39;information uniquement).

![](../../assets/screenshot-2022-01-17-at-14-00-06.png)

L&#39;outil Mesure automatique vous permet d&#39;obtenir une estimation de la taille physique de votre échantillon en fonction des métadonnées de l&#39;image (dpi). Cette méthode n&#39;est précise qu&#39;avec des échantillons numérisés.

![](../../assets/screenshot-2022-01-17-at-14-00-24.png)

L’outil Mesure vous permet d’étalonner la taille physique en indiquant la distance physique entre deux éléments de l’échantillon. Il s’agit généralement de la meilleure méthode pour calculer la taille physique de votre échantillon.

### Surface du maillage 3D

Ces outils vous permettent de définir l’aspect de la surface de votre matériau.

**Échelle physique :** activez ou désactivez l&#39;échelle physique. L’échelle physique est la circonférence du maillage le long des trois axes.\
Mettez votre matériau à l’échelle avec des valeurs physiques. Manipulation de la largeur (X), de l’Height (Y) et de la Profondeur (Z).\
**répétition de Texture :** définissez la répétition de votre matériau

### Matériau de sortie

Vous aide à visualiser la sortie de votre matériau avec son aspect réel.

**Affichage avec rapport physique :**\
L’affichage dans le viewport 2D respecte le rapport physique.\
**Échelle d&#39;Height :** définie/calculée à partir du viewport 3D en fonction de l&#39;échelle physique.
