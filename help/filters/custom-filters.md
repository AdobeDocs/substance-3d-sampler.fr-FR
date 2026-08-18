---
helpx_url: 'https://helpx.adobe.com/fr/substance-3d-sampler/filters/custom-filters.html'
breadcrumb-title: ''
description: Découvrez comment utiliser des filtres personnalisés dans Substance 3D Sampler pour étendre les fonctionnalités avec des filtres de Substance Designer et des effets personnalisés.
helpx_creative_field: ''
helpx_description: Sampler > Filters > Custom Filters
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Filtres personnalisés
user-guide-description: ''
user-guide-title: ''
source-git-commit: dc832dc546735437051226f4e1e731b55147b3ea
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 1%

---


# Filtres personnalisés

## Substance de filtres personnalisés

Vous pouvez importer des filtres créés avec Adobe Substance 3D Designer via le bouton *Importer* dans les actions de pile de calques.

### Création d’un filtre de Substance

Les filtres doivent être configurés de manière spécifique dans Designer pour fonctionner correctement une fois importés dans Sampler.

Les nœuds d&#39;entrée et de sortie du filtre doivent avoir un identifiant ou une utilisation définis.

>[!NOTE]
>
> Il est possible d&#39;utiliser l&#39;**utilisation** ou l&#39;**identifiant** (l&#39;utilisation a la priorité).

#### Format

Exportation du filtre sous forme de fichier d’archive de Substances (.SBSAR)

>[!NOTE]
>
> Vous pouvez exposer les paramètres de filtre pour contrôler le filtre directement dans Sampler. Voir comment [ici](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/manage-parameters/exposing-a-parameter)

#### Création d’un filtre pour modifier les images

![](../assets/image-template.png)

| Nom des images | Utilisation |
| --- | --- |
| *Scan1* | **scan1** |
| *Scan2* | **scan2** |
| *...* | **...** |

#### Création d’un filtre pour modifier les couches

![](../assets/material-template.png)

| Nom du canal | Utilisation |
| --- | --- |
| *Couleur de base* | **basecolor** |
| *Diffus* | **diffusion** |
| *Specular* | **specular** |
| *Specular level* | **niveau spéculaire** |
| *Métallique* | **métallique** |
| *Rugosité* | **rugosité** |
| *Lustre* | **brillance** |
| *Normal* | **normal** |
| *Height* | **height** |
| *Occlusion ambiante* | **ambianteOcclusion** |
| *Opacité* | **opacité** |

>[!IMPORTANT]
>
> Lors de la création d’un filtre personnalisé pour Sampler, vous devez ajouter les données utilisateur suivantes dans votre graphique de Substance :
>
> alchemist::type=filter ;

>[!IMPORTANT]
>
> Si, dans votre pack, vous disposez d’un graphique pour traiter les images (scan1 à scanX) et d’un graphique pour traiter les matériaux (canaux PBR), Sampler peut choisir le graphique approprié en fonction de l’endroit où le filtre est inséré dans la pile de calques.
>
> Dans votre graphique « image », ajoutez les données utilisateur suivantes :
>
> * alchemist::type=filter;alchemist::variation::type=multi
>
> Sur votre graphique « matière », ajoutez les données utilisateur suivantes :
>
> * alchemist::type=filter;alchemist::variation::type=material

### Paramètres spécifiques

Des paramètres spécifiques sont gérés globalement par l’application. C’est un moyen d’utiliser les paramètres globaux de l’application, du projet et de la pile de calques dans vos filtres personnalisés.

#### Format des normales

Contrôle du format normal sur l’application. Définir sur DirectX dans Sampler

**Identificateur de paramètre** : normalformat, normal_format, $normalformat, $normal_format

#### Nombre d’entrées

Lorsque vous souhaitez modifier des images (scan1 à scanX), vous pouvez utiliser le nombre d&#39;images dans la pile de calques à l&#39;aide du paramètre **Nombre d&#39;images**.

* **Identificateur de paramètre** : input_count
* **Type de paramètre** : entier1

#### Entrée de matière

Si vous souhaitez afficher un emplacement de matériau dans la pile de calques comme l’atlas scatter ou la projection :

* Ajouter un nouvel ensemble de nœuds d’entrée (Couleur de base, Normal, ... )
* Tous les nœuds d&#39;entrée de l&#39;arrière-plan (matériau inférieur dans la pile de calques) doivent se trouver dans le groupe **Matériau1**
* Tous les nœuds d&#39;entrée du premier matériau que vous souhaitez ajouter doivent se trouver dans le groupe **Matériau2** et autres si vous souhaitez plusieurs emplacements de matériau.
* Ajoutez un paramètre d&#39;entrée matière :
  * **Identificateur de paramètre** : Material_input
  * **Type de paramètre** : entier1

#### Type de workflow

Si vous souhaitez afficher/masquer certains paramètres en fonction du workflow de votre projet (Métal PBR/Rugosité ou Specular PBR/Glossité), vous pouvez utiliser le paramètre Type de workflow

**Identificateur de paramètre** : workflow_type

**Type de paramètre** : entier1, liste déroulante

options :

* 0 : PBR métallique/rugosité
* 1 : Specular/brillance PBR

![](../assets/workflow-type.jpg){width="300px"}
