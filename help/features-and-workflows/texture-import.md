---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/features-and-workflows/texture-import.html"
breadcrumb-title: ''
description: Apprenez à importer des textures dans Substance 3D Sampler pour utiliser les fichiers image existants dans vos workflows de création de matériaux.
helpx_creative_field: ""
helpx_description: Sampler > Features and workflows > Texture Import
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Importation de texture
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0f989901713dd30f8f936de2445caf5dc70a9225
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 8%

---


# Importation de texture

![](../assets/Capture-decran-2025-02-19-162128.png.img.png)

Le modèle **Importation de texture** charge plusieurs images et les connecte automatiquement aux canaux de sortie corrects en fonction de leurs noms de fichier.

La correspondance des canaux est basée sur les conventions de dénomination spécifiques détaillées ci-dessous. En cas de duplicatas ou de textures sans correspondance, les images seront marquées comme telles dans l&#39;interface.

## OpenPBR

Sampler fera correspondre les fichiers avec les identificateurs d’OpenPBR suivants avec le canal équivalent dans le matériau.

>[!NOTE]
>
> Les identificateurs de canal Height sont identiques à ceux utilisés pour ASM.


| Identificateur d&#39;OpenPBR | Utilisation SBSAR |
| --- | --- |
| poids_de_base | baseWeight |
| base_color | baseColor |
| base_metalness | métallisme/métallique |
| rugosité_diffusion_de_base | baseDiffuseRoughness |
| specular_weight | specularWeight |
| specular_color | specularColor |
| Rugosité_specular | spécularRoughness/rughness |
| specular_roughness_anisotropie | specularRoughnessAnisotropy/anisotropyLevel |
| specular_ior | IOR/IOR spéculaire |
| transmission_weight | transmissionWeight |
| transmission_color | transmissionColor/absorptionColor |
| transmission_profondeur | transmissionDepth/absorptionDistance |
| transmission_dispersion | transmissionScatter |
| transmission_dispersion_anisotropie | transmissionScatterAnisotropy |
| transmission_dispersion_scale | transmissionDispersionScale |
| transmission_dispersion_abbe_number | transmissionDispersionAbbeNumber |
| subsurface_weight | subsurfacePoids/translucidité |
| subsurface_color | subsurfaceColor/scatteringColor |
| subsurface_radius | subsurfaceRadius/scatteringDistance |
| subsurface_radius_scale | subsurfaceRadiusScale/scatteringDistanceScale |
| subsurface_dispersion_anisotropie | subsurfaceScatterAnisotropy |
| coat_weight | coatWeight/coatOpacity |
| coat_color | coatColor |
| rugosité_couche | rugosité du pelage |
| anisotropie_rugosité_couche | coatRoughnessAnisotropy |
| coat_ior | coatIOR |
| coat_darkening | coatDarkening |
| fuzz_weight | fuzzWeight/sheenOpacity |
| fuzz_color | fuzzColor/sheenColor |
| rugosité_floue | fuzzRoughness/sheenRoughness |
| emission_weight | emissionWeight |
| emission_luminance | luminance d&#39;émission |
| emission_color | emissionColor/emisive |
| poids_film_fin | thinFilmWeight |
| thickness_film_fin | thinFilmThickness |
| couche mince | thinFilmIOR |
| opacité | opacité |
| fine_paroi | ThinWaled |
| normal | normal |
| tangente | tangente |
| coat_normal | coatNormal |
| coat_tangent | coatTangent |

## Adobe Standard Material

Vous trouverez ci-dessous une liste des conventions de dénomination de fichier prises en charge pour chaque canal :

| **Canal** | **Adobe Standard Material** |
| --- | --- |
| **Occlusion ambiante** | <ul><li>occlusion ambiante</li><li>ao</li><li>occlusion</li><li>ambient_occlusion</li></ul> |
| **Couleur de base** | <ul><li>couleur de base</li><li>couleur</li><li>albédo</li><li>base_color</li><li>base</li><li>col</li><li>couleur</li><li>base_color</li><li>couleur de base</li></ul> |
| **Diffus** | <ul><li>diffuse</li><li>diff</li></ul> |
| **Émissif** | <ul><li>émissif</li></ul> |
| **Lustre** | <ul><li>brillance</li><li>gloss</li></ul> |
| **Height** | <ul><li>hauteur</li><li>heightmap</li><li>displacement</li><li>disp</li></ul> |
| **Métallique** | <ul><li>métallique</li><li>mtl</li><li>métallurgie</li></ul> |
| **Normal** | <ul><li>normal</li><li>nrm</li></ul> |
| **Opacité** | <ul><li>opacité</li><li>alpha</li></ul> |
| **Rugosité** | <ul><li>rugosité</li><li>rugueux</li></ul> |
| **Specular** | <ul><li>spéculaire</li><li>spécification technique</li></ul> |
| **Specular level** | <ul><li>niveau spéculatif</li><li>specular_level</li></ul> |

