---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/getting-started/export/managing-custom-presets.html"
breadcrumb-title: ''
description: Découvrez comment créer et modifier des paramètres prédéfinis d’exportation personnalisés dans Substance 3D Sampler à l’aide de Substances Designer d’optimisation du workflow.
helpx_creative_field: ""
helpx_description: Sampler > Getting Started > Export > Managing custom presets
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Création et modification de paramètres prédéfinis personnalisés
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---


# Création et modification de paramètres prédéfinis personnalisés

Des paramètres prédéfinis personnalisés peuvent être créés avec Substance 3D Designer.

La création de paramètres prédéfinis personnalisés respecte les mêmes règles que la création d’un filtre personnalisé pour Sampler. Documentation disponible [ici](../../filters/custom-filters.md).

## Création

## Création du graphique

Ouvrez Substance Designer et créez un graphique de Substance.

Ouvrez les propriétés du graphique et renseignez les informations obligatoires suivantes :

* Libellé : saisissez le nom de votre paramètre prédéfini personnalisé qui sera utilisé dans l’interface de Sampler
* Données utilisateur : <b>alchemist::type=filter</b>

## Définition des entrées et des sorties

### Entrées

Les entrées représentent les couches de matériau que vous souhaitez transformer avant l’exportation.

Créez un nœud Couleur d&#39;entrée (ou niveaux de gris) par couche de matériau et ajoutez une <b>utilisation</b> dans les attributs de chaque nœud d&#39;entrée pour vous assurer que la connexion est établie entre votre matériau et votre paramètre prédéfini personnalisé.

Exemple : définition de la couleur de base saisie

![](../../assets/custom-input.png){width="600px"}

### Sorties

Les sorties représentent le résultat de votre exportation de texture.

Créez un nœud de sortie par texture et ajoutez <b>usage</b> et un <b>libellé</b> dans les attributs de chaque nœud de sortie. Le <b>libellé</b> s&#39;affichera dans la liste Couches de la fenêtre Exportateur et dans le nom de votre fichier de texture.

Exemple : définition de la texture personnalisée Opacité de couleur

![](../../assets/custom-output.png){width="600px"}

#### Exemple de packing de canal et de conversion de canal

Packing de 3 couches de niveaux de gris dans une texture RGB :

![](../../assets/channel-packing-example.png){width="600px"}

Conversion des canaux de PBR Métallique/Rugosité en PBR Specular/Brillance :

![](../../assets/channel-conversion.png){width="600px"}

## Importer

Pour importer votre nouveau paramètre prédéfini :

1. Cliquez sur le bouton <b>Gérer les paramètres prédéfinis </b> à droite de la liste déroulante <b>Paramètres prédéfinis</b>.
1. Utilisez le bouton <b>Importer les paramètres prédéfinis</b> en bas de la <b>liste des paramètres prédéfinis</b>.

![](../../assets/Managing-presets-Dropdown.png.img.png){width="400px"}
