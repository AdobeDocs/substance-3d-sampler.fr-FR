---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/features-and-workflows/texture-generators.html"
breadcrumb-title: ''
description: Apprenez à utiliser les générateurs de textures de Substance 3D Sampler pour créer des textures et des motifs procéduraux destinés à la création de matériaux.
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Générateurs de textures
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 1%

---


# Générateurs de textures

![](../assets/sa_whats-new-screen_v4-3-0_generators.png)

Les générateurs de texture offrent un meilleur contrôle sur la création de matériaux à l&#39;aide des options <b>bruits, motifs </b> et<b> grunges</b> paramétriques. Les images générées peuvent être utilisées dans des masques ou des couches colorées.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../assets/Capture-decran-2024-01-31-105700.png)

</td>
<td style="border: 0;" valign="top">

Les générateurs de textures sont un type de fichier dans Substance 3D Sampler. Ils peuvent être filtrés dans le panneau Actifs avec l’icône Générateurs de textures.

</td>
</tr>
</table>

## Comment utiliser les générateurs de textures

### Cartes de couches

Glissez-déposez un générateur de textures dans la vue 3D, la vue 2D ou la pile de calques et sélectionnez un canal pour l’utiliser.

![](../assets/DndTexgen.gif)

Un filtre Remplissage sera créé dans la pile avec le générateur de textures dans la bonne entrée. Vous pouvez accéder aux propriétés du Générateur de textures dans le panneau Propriétés.

#### Filtres

Certains filtres tels que <b>Parquet</b> utilisent par défaut des générateurs de textures pour les masques de motif. D&#39;autres fonctionnent avec une image ou un générateur de textures comme le filtre <b>Motif</b>.\
Dans les filtres, vous pouvez utiliser des générateurs de textures dans n&#39;importe quelle propriété d&#39;image, par exemple <b>masques personnalisés</b>.

Les filtres peuvent suggérer des générateurs à utiliser ; ils s’affichent dans le nouveau sélecteur d’actifs, lorsque vous cliquez sur une propriété d’image.

![](../assets/suggested-filter.png)

#### Tutoriel

Tous les tutoriels Substance 3D Sampler sont disponibles sur notre [page d’apprentissage](https://creativecloud.adobe.com/cc/learn/app/substance-3d-sampler).

[Conception de textiles avec les générateurs de texture Sampler](https://creativecloud.adobe.com/cc/learn/substance-3d-sampler/web/fabric-texture-generator?locale=en)

[Matériaux en fibres de carbone en quelques minutes avec Substance 3D Sampler](https://creativecloud.adobe.com/cc/learn/substance-3d-sampler/web/create-carbon-fiber-material?locale=en)

[Tissu plaid en quelques minutes avec Substance 3D Sampler](https://creativecloud.adobe.com/cc/learn/substance-3d-sampler/web/create-plaid-fabric-material?locale=en)

## Création de générateurs de textures personnalisés

Vous pouvez importer des générateurs de textures créés avec Adobe Substance 3D Designer via le bouton *Importer* dans les actions de pile de calques. Ils doivent être configurés d’une manière spécifique dans Designer pour fonctionner correctement lors de leur importation dans Sampler.

### Type

Choisissez « Générateur de textures » comme type de graphe<b></b>.

![](../assets/typetexgen.png)

#### Sorties

Le nœud de sortie des filtres du filtre doit avoir l&#39;<b>identificateur</b> ou l&#39;<b>utilisation </b> défini :

* La sortie principale du Générateur de textures ne doit pas être utilisée. Il peut alors être reconnu comme la sortie principale de 3D Sampler.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../assets/patternMask.png)

</td>
<td style="border: 0;" valign="top">

![](../assets/PatternMaskusage.png)

</td>
</tr>
</table>

* La <b>sortie secondaire</b> du générateur de textures nécessite <b>utilisation</b> pour être utilisée.\
  Leur nom de groupe sera le <b>identificateur</b> de sortie principal.

>[!NOTE]
>
> Si vous créez vos propres filtres et générateurs de textures pour travailler ensemble, nous vous recommandons d&#39;utiliser des <b>utilisations personnalisées</b> en fonction des <b>identificateurs de sortie</b>.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../assets/patterndata2.png)

</td>
<td style="border: 0;" valign="top">

![](../assets/patterndata2usage2.png)

</td>
</tr>
</table>

>[!IMPORTANT]
>
> Si vous souhaitez que votre générateur de textures personnalisé figure dans une liste de ressources suggérées, vous devez ajouter les données utilisateur suivantes dans votre graphique de Substance :
> 
> alchemist::sugtedfilters=[FilterName,FilterName2];

>[!NOTE]
>
> Les données utilisateur peuvent être utilisées avec [filtres personnalisés](../filters/custom-filters.md).

#### Format

Exportez votre filtre en tant que fichier d’archive de Substance de données (.sbsar)

>[!NOTE]
>
> Vous pouvez exposer les paramètres de filtre pour contrôler le filtre directement dans Sampler. Voir comment [ici](https://experienceleague.adobe.com/fr/docs/substance-3d-designer/using/substance-graphs/manage-parameters/exposing-a-parameter)
