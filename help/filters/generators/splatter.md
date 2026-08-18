---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/generators/splatter.html"
breadcrumb-title: ''
description: Utilisez le générateur d’éclaboussures de Substance 3D Sampler pour créer des effets d’éclaboussure de peinture et de motif aléatoire pour les textures de matériau.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Splatter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Éclaboussure
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 0%

---


# Éclaboussure

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-splatter-18-n-d.png)

Générateurs De **Entrée :**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Éclaboussez des instances d’autres matériaux sur votre matériau.

>[!NOTE]
>
> Pour les matériaux atlas, utilisez plutôt le filtre Atlas scatter.

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Générateur aléatoire** :\
  La valeur de départ aléatoire détermine les valeurs aléatoires des autres paramètres qui utilisent le caractère aléatoire dans ce filtre.
* **Entrée matière** :\
  Sélectionnez le nombre de matières à utiliser comme entrées. Remarque : un calque de projection avec 3 emplacements d’entrée, mais un seul emplacement rempli d’une entrée, s’affichera différemment pour un calque de projection avec 1 emplacement d’entrée et cet emplacement rempli de la même entrée. Pour cette raison, il est recommandé de n&#39;utiliser qu&#39;autant d&#39;intrants que nécessaire.
* **Taille De La Grille** : 1-64\
  La taille de la grille détermine le nombre d’instances créées par le filtre Éclaboussure.
* **Profondeur Height AO** : 0-1\
  Réglez l’intensité de l’AO pour les instances créées par le filtre.

**Forme**

* **Échelle** : 0-5\
  Ajustement de la taille de base de toutes les instances
* **Échelle aléatoire** : 0-1\
  Réglage du caractère aléatoire de la valeur d’échelle pour chaque instance
* **Aucun Chevauchement D&#39;Échelle** : 0-1\
  Modifier la taille des instances pour éviter les chevauchements
* **Position aléatoire** : 0-2\
  Contrôle du caractère aléatoire de la diffusion des instances
* **Rotation Aléatoire** : 0-1\
  Contrôle du caractère aléatoire de la rotation des instances
* **Rotation à partir de la Pente d&#39;arrière-plan** : 0-1\
  Modifiez l’impact des normales de la matière sous-jacente sur la rotation des occurrences.

**Couleur de base**

* **Correspondance Albédo** : 0-1\
  Faire correspondre la couleur des instances à la couleur du matériau sous-jacent
* **Réglage TSL** : 0-1\
  Réglage de la teinte, de la saturation et de la luminosité des instances
* **HSL aléatoire** : 0-1\
  Contrôlez le caractère aléatoire de la teinte, de la saturation et de la luminosité de chaque occurrence

**Normal**

* **Normal à partir de** **Arrière-plan** : 0-1\
  Ajustez l&#39;impact de la normale de la matière sous chaque occurrence sur la normale de l&#39;occurrence.
* **Aléatoire de l&#39;angle normal** : 0-1\
  Inclinez les normales de chaque occurrence selon un angle aléatoire.

**Rugosité**

* **Réglage de la rugosité** : -1 à 1\
  Ajout ou soustraction uniforme de la valeur de rugosité entre les instances
* **Rugosité aléatoire** : -1 à 1\
  Ajout ou soustraction aléatoire de la valeur de rugosité de chaque instance
* **Rugosité De L&#39;Arrière-Plan** : 0-1\
  Ajustez l’impact de la valeur de rugosité du matériau sous-jacent sur la valeur de rugosité de chaque occurrence

**Height**

* **Décalage Height** : -1 à 1\
  Décalage de l’height des instances. Cela peut avoir un impact sur la façon dont les instances se fondent dans le matériau sous-jacent.
* **Décalage Height aléatoire** : 0-1\
  Ajoutez une valeur aléatoire au décalage d&#39;height de chaque instance
* **Échelle D&#39;Height** : 0-2\
  Réglez l’height de toutes les instances.
* **Échelle D&#39;Height Aléatoire** : 0-1\
  Ajouter une valeur aléatoire à l&#39;height de chaque instance
* **Inclinaison par rapport à la Pente principale** : 0-1\
  Ajoutez une pente à chaque occurrence pour la faire correspondre à la pente de la matière sous-jacente
* **Smoothness de Pente d&#39;arrière-plan** : 0-2\
  Ajustez la pente de l&#39;arrière-plan pour les besoins du paramètre **Inclinaison par rapport à la Pente de la balance**
* **Se conformer à l&#39;arrière-plan** : 0-1\
  Contrôlez l’impact du mappage d’height d’arrière-plan sur le mappage d’height des instances. Cela vous permet de réduire les instances autour des détails de l’arrière-plan
* **Arrière-Plan Conforme Lisse** : 0-1\
  Ajuster la quantité de détails visibles en raison de la **conformité à l&#39;arrière-plan**

**Métallique**

* **Réglage métallique** : -1 à 1\
  Contrôle des valeurs métalliques des instances
* **Métallique aléatoire** : -1 à 1\
  Ajout ou soustraction de valeurs aléatoires du métallique de chaque occurrence
* **Métallique à partir de l&#39;arrière-plan** : 0-1\
  Ajustez l’impact des valeurs métalliques d’arrière-plan sur chaque occurrence

**Masquer**

* **Utiliser un masque personnalisé** : activer/désactiver\
  Activez cette option pour utiliser un masque personnalisé et accéder aux commandes de masque personnalisé :
  * **Masque personnalisé** : image/pinceau\
    Importez une image à utiliser comme masque personnalisé ou peignez directement dans la **vue 2D**
  * **Flou de masque personnalisé** : 0-1\
    Flouter les bords du masque personnalisé
  * **Inversion de masque personnalisée** : activer/désactiver
  * **Opacité de masque personnalisée** : 0-1\
    Régler l’intensité du masque personnalisé

Guide d’utilisation

Le filtre Éclaboussure est un moyen utile de dispersion des ressources sur votre matériau, telles que les feuilles, les pierres ou les déchets.

Pour utiliser le filtre Éclaboussure :

1. Ajout du filtre Éclaboussure à la pile de calques
1. Sous le calque Éclaboussure, des emplacements d’entrée apparaissent
1. Modifiez éventuellement le nombre d&#39;emplacements d&#39;entrée disponibles avec **Paramètres de base > Entrée matière**
1. Faites glisser des matières dans les emplacements d’entrée Éclaboussures

Vous pouvez ajuster les paramètres de dispersion dans le **panneau Propriétés** en sélectionnant le calque Éclaboussure.

Vous pouvez ajuster les paramètres des matériaux d&#39;entrée dans le **panneau Propriétés** en sélectionnant le matériau dans l&#39;emplacement d&#39;entrée.
