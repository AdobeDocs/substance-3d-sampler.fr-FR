---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/generators/brickwall.html"
breadcrumb-title: ''
description: Utilisez le générateur de mur de briques de Substance 3D Sampler pour créer des motifs de mur de briques et des textures de maçonnerie réalistes pour les matériaux.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Brickwall
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Brickwall
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---


# Brickwall

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-brickwall-18-n-d.png)

Générateurs De **Entrée :**

</td>
<td width="58.30%" style="border: 0;" valign="top">

DescriptionLe filtre de mur de briques génère un motif de briques en fonction des calques situés en dessous. Ceci est utile pour créer des murs de briques (comme son nom l&#39;indique), mais aussi des sols, ou partout où des briques sont utilisées.

Dans les images ci-dessous, un matériau argileux est converti en mur de briques avec le **filtre de mur de briques**.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0053-brickwall-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0052-brickwall-out.jpg){width="200px"}

</td>
</tr>
</table>

</td>
</tr>
</table>

## Paramètres

**Paramètres prédéfinis**

Faites votre choix parmi de nombreux paramètres prédéfinis pour émuler rapidement un style spécifique.

**Paramètres de base**

* **Générateur aléatoire** : nombre aléatoire\
  Valeur aléatoire utilisée pour déterminer d&#39;autres valeurs aléatoires dans ce filtre.\
  Cliquez sur le nombre pour obtenir une nouvelle valeur aléatoire. Lorsqu’une valeur aléatoire a été sélectionnée, cliquez sur le nom du paramètre pour la réinitialiser à 0.
* **Reliure en brique** :\
  Fusionner les briques en fonction du style sélectionné
* **Type de brique** :\
  Sélectionner le style de la brique
* **Mosaïque** : 1-25\
  Modifiez la quantité de mosaïque sur les axes X et Y.
* **Décalage** : 0-1\
  Modifiez le décalage de chaque ligne de briques par rapport à la ligne précédente.
* **Utiliser la couleur personnalisée** : activer/désactiver\
  Fusionner les briques en fonction du style sélectionné

**Mix**

* **Mode de mélange** :\
  Modifier l’organisation des briques. L&#39;utilisation d&#39;un **mode de mélange** crée un deuxième ensemble de briques qui peut être contrôlé indépendamment de l&#39;ensemble de base.\
  Avec le **Mode de mélange** défini sur **Aucun**, aucun autre paramètre n&#39;apparaîtra dans cette section.
* **Type de brique 2** :\
  Sélectionnez le style du deuxième ensemble de briques.
* **Décalage Height** : 0-1\
  Décaler l’height du deuxième ensemble de briques

**Ciment**

* **Couleur du ciment** : sélecteur de couleurs\
  Changez la couleur du ciment entre les briques.
* **Rugosité du ciment** : 0-1\
  Modifiez la rugosité du ciment entre les briques.
* **Interstice de ciment** : 0-1\
  Modifiez la largeur du ciment entre les briques. Modifie la taille de la brique.
* **Niveau De Ciment** : 0-1\
  Modification de l’height du ciment
* **Trouble Cimentaire** : 0-1\
  Réglez la planéité du ciment. A des valeurs élevées, le ciment peut monter au-dessus des briques.

**Âge**

* **Problème de briques** : 0-1\
  Ajustez de manière aléatoire la rotation de chaque brique en 3 dimensions.
* **Éclat de briques** : 0-1\
  Ajout de fissures dans des briques
* **Bord de la brique** : 0-1\
  Endommager et casser les bords des briques
* **Brique Débloquée** : 0-1\
  Supprimer les briques de manière aléatoire
* **Variation de couleur de la brique** : 0-1\
  Variation de la couleur des briques pour rendre le mur moins uniforme
* **Sale Des Briques** : 0-1\
  Ajouter du dirt aux briques

**Paramètres avancés**

* **Intensité du mélange d&#39;Heights** : 0-1\
  Ajustez la fusion de l’height à partir du matériau de base. La valeur 0 ignore l’height du matériau de base et utilise uniquement les paramètres de filtre de brique pour générer des informations sur l’height. Une valeur de 1 utilise le matériau de base pour générer des informations d’height.
* **Intensité normale** : 0-1\
  Réglez l’intensité des normales générées par le filtre de mur de briques. Une valeur de 0 signifie qu’il n’y a pas de normales.
* **Intensité de l&#39;Occlusion ambiante** : 0-1\
  Réglez l’intensité de l’AO. Une valeur de 0 signifie en fait qu’il n’y a pas d’Occlusion ambiante.

Guide d’utilisation

Le filtre de briques divise le matériau sous-jacent en briques individuelles qu’il réorganise ensuite. Pour cette raison, le filtre Brickwall fonctionne mieux avec les surfaces dures comme les roches ou les métaux - en d&#39;autres termes, les matériaux les plus adaptés pour être des briques dans le monde réel.

Le filtre de mur de briques est utile pour créer un matériau de base sur lequel vous pouvez ensuite superposer d’autres effets, comme la mousse, la neige ou le dirt.
