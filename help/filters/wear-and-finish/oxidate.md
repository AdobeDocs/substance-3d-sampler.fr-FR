---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/wear-and-finish/oxidate.html"
breadcrumb-title: ''
description: Utilisez le filtre Oxyder de Substance 3D Sampler pour ajouter des effets d’oxydation et de ternissement aux matériaux métalliques destinés aux effets de vieillissement.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Wear and Finish > Oxidate
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Oxyder
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---


# Oxyder

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-oxidate-18-n-d.png)

**Entrée :** usure et finition

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Ajoutez une couche d&#39;oxydation sur le dessus de votre matériau.*Une surface ridée a le **filtre Oxydé**&#x200B;appliqué.*

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0019-oxidate-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0018-oxidate-out.jpg){width="200px"}

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
* **Zones cibles** : basculer\
  Activez cette option pour modifier la façon dont l’effet d’oxydation est appliqué sur le matériau. Lorsque cette option est activée, le contrôle suivant s’affiche :
  * **Force des zones cibles** : 0-1\
    Ajustez l’étendue de l’effet des zones cibles.
  * **Diffusion** : 0-1\
    Réglez l’étendue de l’oxydation.
* **Couleur** : sélection de couleur\
  Sélectionnez la couleur de base du filtre. Les couleurs de base modifient la teinte de toutes les couleurs qui composent l’effet oxydant.
* **Variations de couleur** : 0-1\
  Réglez l’échelle de l’effet de variation chromatique.
* **Densité** : 0-1\
  Modifiez la densité de couverture de l&#39;effet.
* **Fond perdu** : 0-1\
  Modifiez la façon dont les bords de l&#39;effet d&#39;oxydation se fondent dans les zones non oxydées.
* **Correctifs** : 0-1\
  Il s’agit d’une commande distincte permettant de modifier le masque entre les zones oxydées et non oxydées. Combinez-la avec les commandes Densité et Autres pour affiner les bords des zones oxydées.
* **Écaillage** : 0-1\
  Réduisez la zone oxydée pour révéler le matériau sous-jacent.
* **Taches** : 0-1\
  Ajustez la quantité de tache superposée sur le matériau.
* **Rugosité de corrosion** : 0-1\
  Réglez la rugosité des zones oxydées.
* **Corrosion métallique** : 0-1\
  Réglez les valeurs métalliques des zones oxydées.
* **Intensité du bruit** : 0-1

**Masquer**

* **Utiliser un masque personnalisé** : activer/désactiver\
  Activez ou désactivez l’utilisation d’un masque personnalisé. Si cette option est activée, les paramètres suivants apparaissent :
  * **Masque** : image/pinceau\
    Sélectionnez une image à utiliser comme masque ou utilisez le pinceau pour peindre un masque personnalisé directement dans la vue 2D.
  * **Masque personnalisé - Flou** : 0-1\
    Floutez le masque.
  * **Masque personnalisé - Inverser** : activer/désactiver\
    Inversez le masque.
  * **Opacité de masque personnalisée** : 0-1\
    Réglez l’opacité du masque.

**Paramètres techniques**

Les paramètres suivants vous permettent d&#39;ajuster la valeur nommée pour l&#39;ensemble du matériau sans ajouter de calque de réglage tel que **Luminosité/Contraste** ou **Teinte/Saturation**

* **Luminosité** : 0-1
* **Contraste** : -1 à 1
* **Décalage de teinte** : 0-1
* **Saturation** : 0-1
* **Intensité normale** : 0-1
* **Plage d&#39;Height** : 0-1
* **Position Height** : 0-1
* **Intensité de l&#39;Occlusion ambiante** : 0-1
