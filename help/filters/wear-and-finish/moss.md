---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/wear-and-finish/moss.html"
breadcrumb-title: ''
description: Utilisez le filtre Mousse de Substance 3D Sampler pour ajouter une croissance de mousse réaliste et des effets de surface organiques à vos matériaux.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Wear and Finish > Moss
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mousse
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---


# Mousse

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/moss-filter-icon.png)

**Entrée :** usure et finition

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Utilisez le **filtre Mousse** pour ajouter de la mousse et du lichen à votre matériau. La **mousse** utilise la carte occlusion de votre matériau pour se développer naturellement dans les fissures et les crevasses.

Les images ci-dessous montrent le matériau du dirt avant et après l&#39;application du **filtre Mousse**.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0021-moss-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0020-moss-out.jpg){width="200px"}

</td>
</tr>
</table>

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Générateur aléatoire** :\
  Valeur de départ aléatoire sur laquelle sont basés tous les autres paramètres aléatoires de ce filtre.
* **Répartition globale de la mousse** : 0-1\
  Ajustez la couverture de la mousse sur votre matériau.
* **Couleur de la mousse** : sélection de la couleur\
  Sélectionnez la couleur principale de la mousse.
* **Couleur de mousse secondaire** : sélection de la couleur\
  Sélectionnez la couleur secondaire de la mousse.
* **Répartition de la mousse** :\
  Sélectionnez la méthode utilisée pour appliquer la mousse. Par défaut, l&#39;**Occlusion** utilise la carte AO de votre matériau pour appliquer la mousse, mais les autres options auront des effets différents. Si **Masque personnalisé** **Masque** est sélectionné, la **section** Masque **&#x200B;**&#x200B;s&#39;affiche.

**Masquer**

Cette section apparaît uniquement si **Masque personnalisé** est choisi sous **Paramètres de base > Répartition de la mousse**.

* **Masque personnalisé - Flou** : 0-1\
  Floutez le masque.
* **Masque personnalisé - Inverser** : activer/désactiver\
  Inversez le masque.
* **Masque personnalisé** : image/pinceau\
  Sélectionnez une image à utiliser comme masque ou utilisez le pinceau pour peindre un masque personnalisé directement dans la vue 2D.

**Mousse**

Les paramètres disponibles dans cette section dépendent de l&#39;option sélectionnée sous **Paramètres de base > Répartition de la mousse**.

* **Occlusion**
  * **Propagation De L&#39;Occlusion De Mousse** : 0-1\
    Contrôlez la propagation de la mousse en fonction de l’occlusion.
  * **Masque D&#39;Occlusion De Mousse** : 0-1\
    Ajustez la quantité de mousse à l’aide de la texture occlusion.
* **Globale**
  * **Propagation globale de la mousse** : 0-1\
    Ajustez la quantité de mousse à afficher.
* **Haut**
  * **Seuil de la mousse supérieure** : 0-1\
    Contrôlez le seuil qui détermine si de la mousse apparaît ou non.
  * **Angle de la mousse supérieure** Réglez la façon dont la mousse s&#39;applique au matériau en fonction de la texture normale.
* **Tous**
  * **Tous** inclut tous les paramètres ci-dessus pour **l&#39;Occlusion**, **l&#39;ensemble** et **le haut**.

Les paramètres suivants sont disponibles indépendamment de l&#39;option sélectionnée sous **Paramètres de base > Répartition de la mousse**.

* **Taille des fleurs de mousse** : 0-1\
  Modifiez la granularité de la mousse.
* **Intensité du grain de mousse** : 0-1\
  Réglez la visibilité du grain de la mousse.
* **Taille des amas de mousse** : 0-1\
  Contrôlez la tendance de la mousse à s&#39;agglutiner.
* **Netteté des amas de mousse** : 0-1\
  Réglez l’adoucissement des bords des amas.
* **Intensité des amas de mousse** : 0-1\
  Contrôlez l&#39;intensité des amas de mousse.
* **Contour progressif de la mousse** : 0-1\
  Réglez le contour progressif des bords du masque de mousse.
* **Intensité du relief de la mousse** : 0-1\
  Modifiez le bossage de la mousse.
* **Seuil de la mousse supérieure** : 0-1

**Paramètres techniques**

* **Intensité normale** : 0-1\
  Réglez l’intensité des normales de la mousse.
* **Intensité de l&#39;Occlusion ambiante** Contrôlez l&#39;intensité de l&#39;occlusion ambiante de la mousse.
