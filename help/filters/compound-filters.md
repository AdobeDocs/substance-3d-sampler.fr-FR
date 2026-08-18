---
helpx_url: 'https://helpx.adobe.com/substance-3d-sampler/filters/compound-filters.html'
breadcrumb-title: ''
description: Apprenez à créer et à utiliser des filtres complexes dans Substance 3D Sampler pour combiner plusieurs filtres en un seul calque réutilisable.
helpx_creative_field: ''
helpx_description: Sampler > Filters > Compound Filters
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Filtres composés
user-guide-description: ''
user-guide-title: ''
source-git-commit: dc832dc546735437051226f4e1e731b55147b3ea
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---


# Filtres composés

Cette fonction vous permet de créer un nouveau type de filtres représentés sous la forme d’un calque unique dans l’interface et composés de plusieurs filtres.

>[!NOTE]
>
> Pris en charge depuis Substance 3D Sampler 3.1.0

## Description

Un filtre composé est un fichier **.ssafilter** qui est un dossier compressé .7zip de :

* un fichier de description utilisant le formatage JSON : **myfilter\_name.json**
* un dossier **resources** contenant :
  * la vignette du filtre : icon.png
  * dépendances de fichiers externes

### Contenu du fichier de description

* Nom : libellé de votre filtre composé affiché dans l’interface
* Id : identifiant unique de votre filtre composé
* Catégorie : catégorie du filtre composé utilisé dans le panneau Actifs lorsque vous regroupez vos actifs par catégorie
* Version : numéro incrémentiel pour définir la version de votre filtre composé.
* Nœud : liste des nœuds à utiliser
* Lien : liste des connexions entre les différents nœuds

### Exemple

```JSON
{ "SamplerFilter":  
 { 
 "Name": "My filter", 
 "Category": "My filter category", 
 "Id": "my_unique_id", 
 "Version": 2, 
 "Node": [ 
        { 
            "Id": "foo", 
            "InternalFilter": "Foo" 
        }, 
        { 
            "Id": "bar", 
            "File": "bar.sbsar" 
        } 
    ], 
    "Link": [ 
        { 
            "From": { "Node": "FilterInput", "Usage": "baseColor" }, 
            "To": { "Node": "foo", "Usage": "baseColor"} 
        }, 
        { 
            "From": { "Node": "FilterInput", "Usage": "normal" }, 
            "To": { "Node": "foo", "Usage": "normal"} 
        }, 
        { 
            "From": { "Node": "foo", "Usage": "baseColor" }, 
            "To": { "Node": "bar", "Usage": "baseColor"} 
        }, 
        { 
            "From": { "Node": "bar", "Usage": "baseColor" }, 
            "To": { "Node": "FilterOutput", "Usage": "baseColor"} 
        }, 
        { 
            "From": { "Node": "foo", "Usage": "normal" }, 
            "To": { "Node": "FilterOutput", "Usage": "normal"} 
        } 
    ] 
}}
```

## Création étape par étape

1. Créez un nouveau fichier : **my\_new\_filter.json**
1. Définir son nom, son ID, sa catégorie,...
1. Définition de la liste des nœuds dont vous avez besoin
1. Si vous avez besoin de fichiers externes, créez un dossier **resources** en regard de votre fichier **.json**
1. Ajoutez vos fichiers dans le dossier **resources**
1. Écrire la liste des liens entre vos nœuds
1. Vérifiez que votre fichier JSON est valide (absence de faute de frappe, coma manquant ou crochet manquant).
1. Si vous souhaitez une vignette, ajoutez une image **icon.png** dans le dossier **resources**
1. Sélectionnez le fichier **.json** et le dossier **resources**, puis compressez-les en 7zip

## Documentation

### Version

L’utilisation d’un numéro de version vous permet de suivre vos différentes itérations. Lorsque vous ouvrez une pile de calques terminée avec une version précédente de votre filtre composé, une notification s’affiche pour vous suggérer d’effectuer la mise à niveau vers la dernière version.

### Nœud

Un nœud peut faire référence à un filtre interne de Substance 3D Sampler. Définissez un identificateur unique **Id** à utiliser pour définir les liens entre les nœuds et le libellé du filtre interne **InternalFilter**

```JSON
{ 
  "Id": "step1_identifier", 
  "InternalFilter": "Dirt" 
}
```

Un nœud peut faire référence à un fichier SBSAR qui ne se trouve pas dans Substance 3D Sampler. Définissez un identifiant unique **Id** à utiliser pour définir les liens entre les nœuds et le nom de fichier **Fichier** du fichier SBSAR. Le fichier SBSAR doit se trouver dans un dossier **resources** à côté du fichier .alchfilter.

```JSON
{ 
  "Id": "step1_identifier", 
  "File": "foo.sbsar" 
}
```

>[!NOTE]
>
> **filterImg** et **filterMat** ne peuvent pas être utilisés comme ID de nœud

### Chaînon

Un lien est une description de la façon dont deux nœuds sont liés et sont composés de deux éléments :

* De : utilisation à utiliser par le nœud
* Vers : sortie d&#39;utilisation du nœud

Chaque élément possède 3 attributs :

* Nœud : déclarez **Id** du nœud que vous souhaitez utiliser
  * définissez l&#39;entrée du filtre composé, l&#39;ID de nœud est **FilterInput**
  * Définissez la sortie de votre calque composé, l&#39;ID de nœud est **FilterOutput**
* Utilisation : déclarez l’utilisation que vous souhaitez utiliser. Il existe 3 options :
  * Utilisation unique à la fois et déclarer lien par lien (baseColor, normal, height, ambiguOcclusion, rugosité, métallique, diffuse, specular, brillance, spécularLevel, opacité, émissif, scan1, ...)
  * Vous pouvez également spécifier une liste [« baseColor », « normal »]. Le premier élément de la liste **De** correspondra au premier élément de la liste **À**. etc.
  * Utilisez **\*** pour permettre à Substance 3D Sampler d&#39;effectuer la correspondance entre les utilisations identiques de tous les nœuds De et Au (il n&#39;est pas possible de combiner **\*** avec un autre lien, alors que des liens uniques et des liens de liste sont possibles entre les mêmes nœuds)
* Groupe : si un nœud a plusieurs fois la même utilisation, vous pouvez utiliser l’attribut Groupe pour sélectionner une utilisation spécifique. c&#39;est-à-dire : pour les filtres de fusion, pour obtenir la baseColor du matériau inférieur, utilisez *Material1* et pour obtenir la baseColor du matériau supérieur, utilisez *Material2*

```JSON
Link between two nodes  
{ 
  "From": { "Node": "node1","Usage": "baseColor", "Group": ""}, 
  "To": { "Node": "node2", "Usage": "baseColor"} 
} 
 
Link between outputs of layers below of the compound filter and the compound filter: 
{ 
  "From": { "Node": "FilterInput", "Usage": "*" }, 
  "To": { "Node": "node1", "Usage": "*"} 
} 

Link to declare outputs of the compound filter: 
{ 
  "From": { "Node": "node1", "Usage": "*" }, 
  "To": { "Node": "FilterOutput", "Usage": "*"} 
}
```
