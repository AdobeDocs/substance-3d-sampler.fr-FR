---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/tools/warp.html"
breadcrumb-title: ''
description: Utilisez l’outil Déformation de Substance 3D Sampler pour appliquer des effets de déformation directionnelle et de distorsion aux textures et aux calques de matériau.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Warp
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Chaîne
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 1%

---


# Chaîne

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-warp-18-n-d.png)

Outils **In:**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Le **filtre Déformation** vous permet de déformer votre matériau en fonction d&#39;un certain nombre de bruits générés.

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Générateur aléatoire** :\
  La valeur de départ aléatoire détermine les valeurs aléatoires des autres paramètres qui utilisent le caractère aléatoire dans ce filtre.
* **Sélection de Bruit** :\
  Sélectionnez le bruit sur lequel baser la déformation. Différents bruits peuvent produire différents effets.
* **Échelle de Bruit** : 0-10\
  Réglez l’échelle du bruit source. Le bruit sera toujours en mosaïque.
* **Type** :\
  Sélectionnez la méthode à utiliser pour déformer le matériau. Si **Déformation directionnelle** ou **Déformation directionnelle multiple** sont sélectionnées, un paramètre supplémentaire s&#39;affiche :
  * **Angle de déformation** : 0-1\
    Réglage de la direction de la déformation
* **Intensité** : 0-1\
  Réglez la force de la déformation.
* **Bruit personnalisé** : activer/désactiver\
  Activez cette option pour utiliser un bruit personnalisé au lieu de la sélection sous **Sélection de Bruit**. Les paramètres disponibles changeront selon que le **Bruit personnalisé** est activé ou désactivé. Si cette option est activée, les paramètres suivants apparaissent :
  * **Flou de Bruit personnalisé** : 0-1\
    Application d’un flou au bruit personnalisé
  * **Bruit personnalisé** : image/pinceau\
    Importez un placage de bruit personnalisé à utiliser comme source de déformation.
* **Déformation par canal** : basculement\
  Lorsque cette option est activée, des sections supplémentaires apparaissent pour contrôler la déformation de chaque couche indépendamment. Pour chaque canal, les paramètres suivants sont disponibles :
  * ***Nom du canal*** : activer/désactiver\
    Indique si ce canal est affecté par le **filtre Déformation**.
  * **Mode de fusion** :\
    Sélectionnez la manière dont les résultats de la déformation de cette couche sont fusionnés avec le calque sous-jacent
  * **Opacité** : 0-1\
    Modifiez l’opacité des résultats du filtre pour cette couche.
