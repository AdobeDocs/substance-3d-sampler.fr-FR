---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/wear-and-finish/metal-finish.html"
breadcrumb-title: ''
description: Utilisez le filtre Finition métallique de Substance 3D Sampler pour appliquer diverses textures et finitions de surface métallique à vos matériaux.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Wear and Finish > Metal Finish
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Finition métallique
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---


# Finition métallique

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/metal-finish-filter-icon.png.img.png)

**Entrée :** usure et finition

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Convertissez votre matériau en métal avec un certain nombre de finitions et de styles.

*Un matériau en métal brut est converti en une surface métallique brossée avec le filtre **Metal Finish***.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0023-metal-finish-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0022-metal-finish-out.jpg){width="200px"}

</td>
</tr>
</table>

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Générateur aléatoire** :\
  La valeur de départ aléatoire détermine les valeurs aléatoires des autres paramètres qui utilisent le caractère aléatoire dans ce filtre.
* **Modification Métallique uniquement** : basculer\
  Lorsqu’il est activé, ce filtre limite ses modifications au canal métallique.
* **Mode colorimétrique Metal** :\
  Sélectionnez une couleur basée sur un métal existant ou choisissez la vôtre. Avec l&#39;option **Couleur personnalisée** sélectionnée, le contrôle suivant s&#39;affiche :
  * **Couleur métallique** : sélection de couleur\
    Sélectionnez une couleur personnalisée pour votre finition métallique.
* **Type de finition** :\
  Sélectionnez un style à appliquer au métal. Chaque style possède différents paramètres qui vous permettent d’en ajuster l’aspect. Les paramètres suivants peuvent apparaître :
  * **Intensité** : 0-1\
    Réglez l’intensité de la finition choisie.
  * **Échelle** : 0-1\
    Modifiez l’échelle du motif pilotant la finition choisie.
  * **Rugosité** : 0-1\
    Contrôlez la valeur de rugosité du métal.
  * **Échelle Beads** : 0-1\
    Disponible pour **Sandblasted**. Définissez la taille des perles utilisées pour créer l’effet sablage.
  * **Poli** : 0-1\
    Disponible pour **Convertir**. Réglez la quantité de polissage qui lisse les parties supérieures du matériau.
  * **Motif** :\
    Disponible pour **Grinded**. Définissez le motif utilisé par le broyeur.
  * **Détails du Relief** : 0-1\
    Disponible pour **Raw**. Réglez la force normale.
  * **Orientation** : 0-1\
    Disponible pour **Formé**. Modifiez la direction de l’effet de pinceau.
  * **Longueur du pinceau** : 0-1\
    Disponible pour **Formé**. Modifiez la longueur des contours utilisés pour créer l’effet de pinceau.
  * **Brossé** : 0-1\
    Disponible pour **Galvanisé**. Superposez un aspect brossé sur la finition galvanisée.

**Masquer**

* **Utiliser un masque personnalisé** : activer/désactiver\
  Activez ou désactivez l’utilisation d’un masque personnalisé. Si cette option est activée, les paramètres suivants apparaissent :
  * **Masque** : image/pinceau\
    Sélectionnez une image à utiliser comme masque ou utilisez le pinceau pour appliquer un peinture personnalisé directement dans la Vue 2D.
  * **Masque personnalisé - Flou** : 0-1\
    Floutez le masque.
  * **Masque personnalisé - Inverser** : activer/désactiver\
    Inversez le masque.

**Paramètres avancés**

* **Base color** : activer/désactiver\
  Définissez si le canal de base color est affecté par le filtre.
* **Métallique** : activer/désactiver\
  Définissez si la couche métallique est affectée par le filtre.
* **Rugosité** : activer/désactiver\
  Définissez si le canal de rugosité est affecté par le filtre.
* **Specular level** : activer/désactiver\
  Détermine si la couche de specular level est affectée par le filtre. Si cette option est activée, une commande supplémentaire apparaît :
  * **Specular level** **- Valeur** : 0-1\
    Réglez la valeur de la couche de specular.

>[!NOTE]
>
> Il existe actuellement un bogue connu dans lequel le contrôle **Specular level** peut disparaître s&#39;il est désactivé sans contrôle pour le réactiver. Si vous perdez le contrôle **Specular level** mais que vous en avez besoin, vous pouvez utiliser la commande Annuler (Ctrl + z ou Cmd + z sur macOS) pour annuler la désactivation du bouton bascule.

* **Normal** : activer/désactiver\
  Indique si le canal normal est affecté par le filtre. Si cette option est activée, une commande supplémentaire apparaît :
  * **Intensité normale** : 0-1\
    Réglez la force de la modification normale à l’aide du filtre.
* **Height** : activer/désactiver\
  Définissez si le canal d’height est affecté par le filtre.
* **Emissive** : activer/désactiver\
  Définissez si le canal d’emissive est affecté par le filtre. Si cette option est activée, une commande supplémentaire apparaît :
  * **Emissive - Couleur** : sélection de la couleur\
    Définissez la couleur de la couche emissive.
* **Ambient occlusion** : activer/désactiver\
  Définissez si le canal d’ambient occlusion est affecté par le filtre. Si cette option est activée, les commandes supplémentaires suivantes apparaissent :
  * **Ambient occlusion - Intensité** : 0-1\
    Réglez la force de l’AO généré.
  * **Ambient occlusion** **- Rayon** : 0-1\
    Réglez le rayon de l’effet AOP.
* **Opacité** : activer/désactiver\
  Définissez si la couche d’opacité est affectée par le filtre. Si cette option est activée, une commande supplémentaire apparaît :
  * **Opacité - Valeur** : 0-1\
    Modifiez l’opacité du matériau.
