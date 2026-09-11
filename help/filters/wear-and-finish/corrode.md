---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/wear-and-finish/corrode.html"
breadcrumb-title: ''
description: Utilisez le filtre Corrode de Substance 3D Sampler pour ajouter des effets de corrosion et de dégradation chimique aux matériaux métalliques.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Wear and Finish > Corrode
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Corroder
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---


# Corroder

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/corrode-filter-icon.png)

**Entrée :** usure et finition

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Le filtre corrode imite l&#39;effet de l&#39;acide qui dévore votre matériau, laissant des trous et des dommages à la surface.

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Générateur aléatoire** :\
  La valeur de départ aléatoire détermine les valeurs aléatoires des autres paramètres qui utilisent le caractère aléatoire dans ce filtre.
* **Zones affectées** :\
  Sélectionnez l’impact de la courbure de la surface sur l’effet du filtre.
* **Niveau De Perforation** : 0-1\
  Ajustez le nombre de trous créés.
* **Position De La Courbure** : 0-1\
  Modifiez la plage de courbures à modifier.
* **Courbure lisse** : 0-1\
  Lissez la map curvature.
* **Distance De Dommage** : 0-1\
  Contrôlez le rayon d&#39;endommagement autour des zones corrodées.
* **Intensité des dommages** : 0-1\
  Ajustez l&#39;étendue des dommages dans les zones touchées.
* **Intensité de l&#39;Height** : 0-1\
  Contrôlez l&#39;impact des dommages sur la map height.
* **Extrusion de position** : basculer\
  Changez la direction des dommages sur la map height. Lorsque cette option est désactivée, l&#39;endommagement mange la surface. Lorsque cette option est activée, l&#39;endommagement se construit vers l&#39;extérieur à partir de la surface.

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

Certains des paramètres avancés ont une incidence sur l’ensemble du matériau et non uniquement sur les zones modifiées par celui-ci.

* **Luminosité** : 0-1\
  Réglez la luminosité ou la luminosité pour le matériau complet.
* **Contraste** : -1 à 1\
  Réglez le contraste de l’albédo pour le matériau complet.
* **Décalage de teinte** : 0-1\
  Décalage de la valeur de teinte des couleurs dans le matériau entier.
* **Saturation** : 0-1\
  Réglez la saturation pour le matériau entier.
* **Intensité normale** : 0-1\
  Réglez l&#39;intensité de la map normal là où elle a été affectée par le **filtre Corrode**.
* **Plage d&#39;Height** : 0-1\
  Augmentez la plage de valeurs dans la map height pour le matériau complet.
* **Position Height** : 0-1\
  Décalage de l’height du matériau complet.
* **Intensité de l&#39;Ambient occlusion** : 0-1\
  Ajustez la force de l&#39;impact de l&#39;AO en raison du **filtre Corrode**.
