---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/scripting-and-development/create-a-script-with-python.html"
breadcrumb-title: ''
description: Découvrez comment créer des scripts Python pour Substance 3D Sampler afin d’automatiser les workflows et d’étendre les fonctionnalités de l’application.
helpx_creative_field: ""
helpx_description: Sampler > Scripting and Development > Create a Script with Python
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Création d’un script avec Python
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---


# Création d’un script avec Python

Ce guide décrit comment créer un plug-in d’enregistrement automatique simple avec Python.

## Structure de script

Les scripts nécessitent un seul fichier PY pour être importés dans Sampler. Vous pouvez enregistrer l’exemple de script ci-dessous en tant que fichier PY et l’importer dans Sampler.

## Exemple de script

Le script ci-dessous crée automatiquement des variations de votre matériau en sélectionnant une nouvelle valeur de départ aléatoire pour chaque calque du matériau. Ceci est utile pour s&#39;assurer que votre matériel peut être utilisé dans un cas général au lieu de s&#39;appuyer sur des graines aléatoires spécifiques.

### random\_seed\_variations.py

```
import substance_sampler as ssa 

from random import randrange 

 

## Get the current asset loaded in the layer stack

my_asset = ssa.get_selected_asset() 

 

## Create a list of all layers of the current asset

my_asset_layers = my_asset.get_layers() 

 

## Go through the layers list

for layer in my_asset_layers: 

## Go through all parameters of each layer

    for parameter in layer.parameters: 

## if the parameter is Random Seed, change is value

        if parameter.label == "$randomseed": 

            parameter.value = randrange(10000) 

            print(f"Random Seed for layer {layer.name}: {parameter.value}") 

 
```


Le code ci-dessus inclut des commentaires pour expliquer ce qui se passe sur chaque ligne.

## Importation du script

Une fois que vous avez enregistré le script ci-dessus en tant que fichier PY sur votre ordinateur, vous pouvez l’importer avec Modifier > Préférences > Plug-ins et scripts. Une fois importé, une option **Scripts** apparaît dans la barre de menus en regard de **Fichier** et **Modifier**. À partir de là, vous pouvez exécuter le script.

Vous pouvez en savoir plus sur la gestion de vos scripts [ici](../manage-installed-plugins-and-scripts.md).
