---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/generators/floor-tiles.html"
breadcrumb-title: ''
description: Utilisez le générateur de carreaux d’Arrondi aux inférieurs de Substance 3D Sampler pour créer des motifs de carreaux de sol et des textures en céramique réalistes pour les matériaux.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Floor Tiles
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Carreaux d’Arrondi aux inférieurs
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '787'
ht-degree: 0%

---


# Carreaux d’Arrondi aux inférieurs

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-floortiles-18-n-d.png)

Générateurs De **Entrée :**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Le filtre Carreaux d’Arrondi aux inférieurs décompose le matériau sous-jacent et le convertit en un arrangement de Carreaux d’Arrondi aux inférieurs.

Les images ci-dessous montrent un matériau en béton converti en carrelage avec un motif en damier.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0031-floor-tiles-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0030-floor-tiles-out.jpg){width="200px"}

</td>
</tr>
</table>

</td>
</tr>
</table>

Paramètres

<b>Paramètres de base</b>

* <b>Générateur aléatoire</b> : \
  La valeur de départ aléatoire détermine les valeurs aléatoires des autres paramètres qui utilisent le caractère aléatoire dans ce filtre.
* <b>Nombre de matériaux</b> : \
  Modifiez le nombre de matériaux à convertir en carrelage. Le premier matériau est déterminé par les calques situés sous le calque de filtre Carreaux d’Arrondi aux inférieurs. Si cette option est sélectionnée, la seconde peut être ajoutée comme entrée
* <b>Intensité des Matériaux d&#39;entrée</b> : 0-1 \
  Degré de visibilité des détails des matériaux d’entrée dans les vignettes
* <b>Inverser les Matériaux</b> : basculer \
  Lorsque vous utilisez deux matériaux, exchange à l’endroit où ils apparaissent dans les mosaïques.
* <b>Variation de couleur</b> : 0-1 \
  Degré de variation de la couleur entre chaque carreau d’un même matériau
* <b>Rayon de biseau</b> : 0-1 \
  Taille de la tuile par rapport à la taille du mortier
* <b>Profondeur en biseau</b> : 0-1 \
  Profondeur du mortier
* <b>Arrondi du biseau</b> : 0-1 \
  Détermine les angles extérieurs des carreaux
* <b>Grain De Surface</b> : 0-1 \
  Détermine le niveau de détail du matériau d’origine sur la normale et les maps height des mosaïques
* <b>Masque de motif</b> : entrée.  \
  Chaque masque de motif de mosaïque d’Arrondi aux inférieurs dispose d’un ensemble de paramètres différent. Ici, nous ne couvrons que les paramètres disponibles pour <b>carreau</b>

  * <b>Graine aléatoire </b>\
    La valeur de départ aléatoire détermine les valeurs aléatoires des autres paramètres qui utilisent le caractère aléatoire dans ce filtre.
  * <b>X Quantité </b>\
    Ajuster le nombre de colonnes de mosaïques
  * <b>Quantité Y</b> \
    Ajuster le nombre de lignes de mosaïques
  * <b>Dégradé </b> \
    Ajuste la proportion de la taille du carreau par rapport à la taille du mortier.
  * <b>Luminance aléatoire</b>\
    Comme la luminance influe sur la map height, ce paramètre supprime aléatoirement certaines mosaïques
  * <b>Rotation du motif</b> : 0-1 \
    Fait pivoter l’angle des carreaux, en les maintenant éloignés les uns des autres pour éviter toute superposition
  * <b>Échelle de forme :</b> 0-1 \
    Ajuste la proportion de la taille du carreau par rapport à la taille du mortier.
  * <b>Échelle de forme aléatoire </b>\
    Ajoute de manière aléatoire une différence de taille des vignettes
  * <b>Taille de forme </b>\
    Réglage de la longueur et de la largeur des carreaux
  * <b>Taille de forme aléatoire </b>\
    Ajout d’un effet aléatoire à la longueur et à la largeur des carreaux
  * <b>Mode de décalage de position</b> : liste déroulante
  * <b>Décalage de position </b>\
    Décale de manière aléatoire les colonnes de mosaïques afin qu’elles ne soient pas alignées horizontalement
  * <b>Position aléatoire</b> \
    Positionne les carreaux de manière aléatoire sur la surface, avec une certaine superposition potentielle entre les carreaux
  * <b>Rotation de la forme </b>\
    Faites pivoter l&#39;angle des carreaux dans la même direction, tout en les gardant aussi proches que possible avec une superposition potentielle
  * <b>Rotation aléatoire de la forme </b>\
    Faites pivoter aléatoirement l&#39;angle des carreaux, tout en les gardant aussi proches que possible avec une superposition potentielle

<b>Écart</b>

* <b>Couleur d&#39;espace</b> : sélection de la couleur \
  Modification de la couleur d’une mosaïque à l’autre
* <b>Rugosité d&#39;espace</b> : 0-1 \
  Modifiez la valeur de rugosité du matériau entre les mosaïques.
* <b>Espace Métallique</b> : 0-1 \
  Modifiez la valeur métallique du matériau entre les mosaïques.
* <b>Height de l&#39;espace</b> : 0-1 \
  Modifiez la valeur d’height du matériau entre les mosaïques.
* <b>Irrégularité d&#39;espace</b> : 0-1 \
  Ajustez la netteté de l&#39;application du mortier entre les carreaux.

<b>Âge</b>

* <b>Inclinaison de l&#39;Arrondi aux inférieurs</b> : 0-1 \
  Ajouter une inclinaison aux mosaïques aléatoires
* <b>Height aléatoire</b> \
  Ajout aléatoire d’une différence d’height entre les mosaïques
* <b>Dirt</b> : 0-1 \
  Ajouter du dirt aux carreaux et à l’espace
* <b>Dommages</b> : 0-1 \
  Supprimez de manière aléatoire certaines taches sur le bord du biseau de chaque carreau
* <b>Imperfections</b> \
  Ajout de petits trous et d’imperfections dans les carreaux

<b>Paramètres techniques</b>

* <b>Échelle De Matériau</b> : 0-1 \
  Échelle du matériau dans les carreaux
* <b>Intensité normale</b> : 0-1 \
  Réglez l’intensité de la normale de l’espace, des carreaux et du matériau intérieur

<b>Guide d&#39;utilisation</b>

Le filtre Carreaux d’Arrondi aux inférieurs vous permet de convertir rapidement votre matériau en carreaux. La plupart des filtres Carreaux d’Arrondi aux inférieurs sont assez simples à utiliser, sauf lorsque vous utilisez plusieurs matériaux. Pour utiliser deux matériaux :

1. Définissez <b>Paramètres de base > Nombre de matériaux</b> sur 2.
1. Faites glisser le deuxième matériau dans l’emplacement d’entrée qui apparaît sous le filtre Carreaux d’Arrondi aux inférieurs dans la pile de calques.
1. Ajustez les paramètres du matériau d’entrée jusqu’à ce que vous soyez satisfait du résultat.

Bien qu&#39;il soit possible d&#39;ajouter plusieurs matériaux et filtres dans un seul emplacement d&#39;entrée, il est généralement conseillé d&#39;éviter cette opération, car elle ajoute de la complexité et peut rendre la lecture de votre matériau plus difficile lorsque vous y reviendrez plus tard. Au lieu de cela, créez de nouveaux matériaux dans votre projet, puis faites glisser une instance de votre nouveau matériau dans l’emplacement d’entrée. Lorsque vous mettez à jour le matériau dans votre projet, il met automatiquement à jour le matériau dans l&#39;emplacement d&#39;entrée, ce qui vous donne un contrôle total et simplifie la pile de calques.
