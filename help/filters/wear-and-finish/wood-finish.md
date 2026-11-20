---
description: Utilisez le filtre Finition du bois de Substance 3D Sampler pour appliquer diverses textures et finitions de surface en bois à vos matériaux.
title: Finition bois
hold: true
source-git-commit: f281c7ec254de74381b2565f835cc32e4de643d2
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%
---

# Finition bois

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/Filters/S_Wood_18_N_D.png" alt=""/><br><strong>Entrée :</strong> usure et finition</td>
    <td style="border: 0;" valign="top">Description<br>Ajoutez des détails normaux et de rugosité à votre matériau pour ajouter des finitions généralement associées au bois, telles que du vernis, de la céruse ou du grain de bois.<br><em>Une couleur de remplissage unie</em><strong><em> </em></strong><em>donne l’apparence du bois en ajoutant du grain de bois avec le </em><strong><em>filtre de finition du bois</em></strong><em>.</em><br><img src="../../assets/wood-finish-before.png" alt=""/><img src="../../assets/wood-finish-after.png" alt=""/></td>
  </tr>
</table>

## Paramètres

**Paramètres de base**

* **Générateur aléatoire** :

  La valeur de départ aléatoire détermine les valeurs aléatoires des autres paramètres qui utilisent le caractère aléatoire dans ce filtre.

* **Type de finition** :

  Sélectionnez un style à appliquer au métal. Chaque style possède différents paramètres qui vous permettent d’en ajuster l’aspect. Outre la finition **naturelle**, chaque finition dispose d&#39;un ensemble de paramètres pour contrôler l&#39;effet.

  Les finitions suivantes sont disponibles :

  * **Naturel** : une finition naturelle lisse pour le bois traité.
  * **Céruse** : créez un aspect doux et bicolore en remplissant les pores ouverts avec un pigment.
  * **Vernis mat** : ajoutez une finition de vernis mat doux.
  * **Vernis** : ajoutez une finition de vernis très réfléchissante.
  * **Ancien** : ajustez la couleur et la rugosité du matériau sous-jacent pour donner l’impression que le bois est vieilli.
  * **Brut** : ajoutez du grain de bois pour créer l&#39;apparence de bois de sciage brut.
  * **Scié** : ajoutez des traces de sciage pour créer l’apparence de bois frais provenant du sciage.

### Paramètres partagés

Les paramètres suivants apparaissent pour plusieurs finitions :

* **Teinte** : permet de régler la couleur du matériau.
* **Saturation** : réglez la force des couleurs.
* **Luminosité** : réglez la luminosité.
* **Intensité de la Rugosité** : ajustez la Rugosité du matériau.
* **Intensité de la Rugosité des fibres** : ajoute des informations de rugosité haute fréquence à la carte de Rugosité. Utilise conjointement le curseur Intensité de la Rugosité pour modifier les valeurs de Rugosité, que le matériau soit très lisse ou très irrégulier.
* **Intensité normale** : réglez la force de la map normal.
* **Contraste des masques de fibres** :

### Finitions

#### Ceruse

* **Couleur 1** :
* **Couleur 2** :
* **Variations de Base color** :
* **Détails haute fréquence** :

#### Vernis

* **Variations d&#39;orientation normales des fibres** :

#### Ancien

* **Intensité de la Rugosité du vernis** :
* **Rotation de l&#39;effet** :

#### Bruts

* **Informations supplémentaires normales** :

#### Scié

* **Réduction de Rugosité avec les fibres** : ajustez la rugosité le long des lignes de scie pour créer un contraste de rugosité.
* **Nombre de coupes de scie** : ajustez le nombre de lignes de scie.
* **Régularité du masque** : permet de régler la régularité d&#39;affichage des lignes de scie. Plus la valeur est élevée, moins les lignes sont régulières.
* **Fibres supplémentaires** : ajustez le nombre de fibres ajoutées parallèlement aux lignes de scie.
