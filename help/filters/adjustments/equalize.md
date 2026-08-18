---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/adjustments/equalize.html"
breadcrumb-title: ''
description: Utilisez le filtre Égaliser de Substance 3D Sampler pour redistribuer automatiquement les valeurs de luminosité et améliorer le contraste de l’image.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Adjustments > Equalize
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Égaliser
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---


# Égaliser

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-equalize-18-n-d.png)

**Entrée :** Réglages

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Le filtre Égaliser ajuste le contraste local en fonction d’une plage de distances. L’objectif du filtre Égaliser est de réduire les différences importantes dans chaque couche. Par conséquent, il est généralement utile dans le cadre du workflow Image vers matériau (B2M) : le filtre Image vers matériau (optimisé par l’IA) inclut une passe d’égalisation dans le filtre pour améliorer les résultats.

Les images ci-dessous montrent le **filtre Égaliser** en action.

![](../../assets/3d-2d-filters-cropped-0033-equalizer-in.jpg)

Avant l&#39;ajout du filtre **Égaliser**, il existe des variations importantes entre la carte d&#39;height et la couleur de base de ce matériau.

![](../../assets/3d-2d-filters-cropped-0032-equalizer-out.jpg)

Une fois le **filtre Égaliser** ajouté, la carte d&#39;height et les couches de couleur de base sont plus uniformes sans perdre de détails.

</td>
</tr>
</table>

## Tutoriel sur l’égalisation des filtres

## Paramètres

<b>Paramètres de base</b>

* <b>Mosaïque d&#39;entrée</b> : basculer\
  Lorsque cette option est activée, traitez la matière comme si elle était mosaïquée à plusieurs reprises. Par conséquent, les modifications effectuées près des bordures seront influencées par les valeurs de couleur de la bordure opposée.
* <b>Rayon</b> : 0-1\
  Étalez l’effet Égaliser sur une zone plus large.
* <b>Débordement de couleur</b> : 0-1\
  Contrôlez les couleurs qui se fondent dans la zone environnante.
* <b>Détails locaux</b> : 0-1\
  Réglez la façon dont le filtre Égaliser tente de préserver les détails locaux.

<b>*Canal*</b>

Les commandes de chaque couche fonctionnent de la même manière.

* <b>Remplacer les paramètres courants</b> : activer/désactiver\
  Activez cette option pour personnaliser l’effet Égaliser pour cette couche. Lorsque cette option est activée, des commandes supplémentaires apparaissent :
  * <b>Mosaïque d&#39;entrée</b> : basculer\
    Lorsque cette option est activée, traitez la matière comme si elle était mosaïquée à plusieurs reprises. Par conséquent, les modifications effectuées près des bordures seront influencées par les valeurs de couleur de la bordure opposée.
  * <b>Rayon</b> : 0-1\
    Etalez l’effet d’égalisation sur une zone plus large.
  * <b>Conserver les différences locales</b> : activer/désactiver\
    Activez cette option pour que l’effet d’égalisation fonctionne à une résolution plus élevée afin de conserver les détails
* <b>Mode cible</b> :\
  Sélectionnez la manière de biaiser l’effet Égaliser. Par défaut, l’option Égaliser tente de rapprocher les couleurs de la couleur moyenne de la couche. Utilisez Paramètre pour effectuer un biais vers une couleur ou une valeur choisie. Lorsque Paramètre est sélectionné, une commande supplémentaire apparaît :
  * <b>Cible</b> : sélection de couleur\
    Sélectionnez une couleur ou une valeur qui servira de cible pour l’algorithme d’égalisation.
* <b>Variation de couleur personnalisée</b> : curseurs TSL\
  Réglez la teinte, la chrominance (saturation) et la luminance (luminance) du résultat après avoir exécuté l’algorithme d’égalisation pour la couche spécifiée.

<b>Masquer</b>

* <b>Masque personnalisé</b> : activer/désactiver\
  Activer ou désactiver l’utilisation d’un masque personnalisé pour ce filtre
* <b>Masque personnalisé</b> : image/pinceau\
  Sélectionnez une image à utiliser comme masque ou utilisez le pinceau pour peindre un masque personnalisé directement dans la vue 2D
* <b>Inversion de masque personnalisée</b> : activer/désactiver
