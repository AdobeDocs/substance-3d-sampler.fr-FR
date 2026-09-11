---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/generators/panel.html"
breadcrumb-title: ''
description: Utilisez le générateur de panneaux de Substance 3D Sampler pour créer des motifs de panneau et des textures de surface segmentées pour les matériaux.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Panel
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Panneau
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---


# Panneau

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-metalpanels-18-n-d.png)

Générateurs De **Entrée :**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Convertissez votre matériau en panneaux. Le filtre Panneaux est particulièrement bien adapté aux matériaux métalliques.

*Un matériau métallique continu converti en panneaux.*

![](../../assets/3d-filters-cropped-0015-panel-in.jpg){width="200px"}

![](../../assets/3d-filters-cropped-0014-panel-out.jpg){width="200px"}

</td>
</tr>
</table>

## Paramètres

**Paramètres prédéfinis**

Utilisez les paramètres prédéfinis pour modifier rapidement les paramètres et créer un effet spécifique.

**Paramètres de base**

* **Générateur aléatoire** :\
  La valeur de départ aléatoire détermine les valeurs aléatoires des autres paramètres qui utilisent le caractère aléatoire dans ce filtre.
* **X Amount** : 0-20\
  Modification du nombre de panneaux dans l’axe X
* **Quantité Y** : 0-20\
  Modification du nombre de panneaux dans l’axe Y
* **Type de Seam** :\
  Sélection de différents styles de seams entre les panneaux
* **Utiliser des attaches** :\
  Ajoutez des attaches entre les panneaux. Lorsque cette option est activée, la section Attaches apparaît dans la liste des paramètres.

**Panneaux**

* **Quantité de décalage** : 0-1\
  Décalez chaque ligne de panneaux par rapport à la ligne précédente d’un pourcentage de la taille du panneau.
* **Décalage aléatoire** : 0-1\
  Ajouter une valeur aléatoire au décalage de chaque ligne
* **Décalage vertical** : basculer\
  Basculez entre le décalage horizontal et le décalage vertical.
* **Tension de renflement** : -1 à 1\
  Modifiez les normales de chaque panneau pour qu’il donne l’impression qu’il est renflé vers l’intérieur ou vers l’extérieur sous l’effet de la pression.
* **Rides** : 0-1\
  Ajout de bosses et de plis subtils aux panneaux
* **Variation de couleur** : 0-1\
  Variation aléatoire de la couleur entre des panneaux individuels
* **Variation de réflexion** : 0-1\
  Variation aléatoire de la rugosité de panneaux individuels

**Seams**

La sélection des paramètres dans cette section dépend de la valeur que vous avez choisie dans **Paramètres de base > Type de Seam**.

* ***Écart***
  * **Largeur du Seam** : 0-1\
    Modification de la largeur entre les panneaux
  * **Variation d&#39;espace** : 0-1\
    Décalez légèrement les panneaux pour faire varier la largeur des espaces entre les panneaux
  * **Arrondi de l&#39;angle de l&#39;espace** : 0-1\
    Arrondissement des bords des panneaux
  * **Biseau d&#39;espace** : 0-1\
    Biseautage des bords des panneaux
* ***Souder***
  * **Largeur du Seam** : 0-1\
    Modification de la largeur entre les panneaux
  * **Qualité de la soudure** : 0-1\
    Régler l&#39;uniformité de la soudure
  * **Décoloration de la soudure** : 0-1\
    Modifiez la quantité de décoloration de la soudure par rapport à la couleur des panneaux.
  * **Remplacer le Matériau de soudure** : activer/désactiver\
    Activez cette option pour personnaliser le matériau utilisé pour créer la soudure. Les paramètres supplémentaires suivants apparaissent si cette option est activée :
    * **Couleur du Matériau de soudure** : sélection de couleur\
      Sélectionnez la couleur de la soudure. Cela sera toujours affecté par la **décoloration de la soudure**.
    * **Rugosité du Matériau de soudure** : 0-1\
      Ajuster la rugosité du seam de soudure entre les panneaux
* ***Chevauchement***
  * **Largeur du Seam** : 0-1\
    Modification de la largeur entre les panneaux
* ***Seam debout***
  * **Largeur du Seam** : 0-1\
    Modification de la largeur entre les panneaux

**Attaches**

* **Type de fixation** :\
  Sélectionner le style de boulon à utiliser entre les panneaux
* **Quantité de fixation** : 3-10\
  Modifiez le nombre d&#39;attaches à utiliser le long du bord entre deux panneaux.
* **Taille du boulon** : 0-1\
  Modifier la taille des attaches
* **Variation de l&#39;élément de fixation** : 0-1\
  Décaler la position des attaches
* **Remplacer le Matériau du boulon** : activer/désactiver\
  Modifiez le matériau utilisé pour les boulons séparément du matériau de base. Lorsque cette option est activée, les paramètres suivants apparaissent :
  * **Couleur du Matériau du boulon** : sélection de la couleur\
    Sélectionner la couleur du matériau du boulon
  * **Rugosité du Matériau de fixation** : 0-1\
    Modifier la rugosité du matériau du boulon

**Avancé**

* **Normal** **Intensité** : 0-3\
  Régler l’intensité normale globale du matériau
* **Plage d&#39;Height des Seams** : 0-1\
  Modifier la hauteur des seams personnalisés au-dessus des panneaux
* **Plage d&#39;Height du boulon** : 0-1\
  Modifier l&#39;height des attaches
* **Profondeur Height AO** : 0-1\
  Modification de la force de l’AO
* **Rayon AO** : 0-1\
  Modifier le rayon de l’AO
