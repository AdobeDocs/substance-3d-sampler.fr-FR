---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/release-notes/version-4-0.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Sampler version 4.0 pour en savoir plus sur la création d’objets 3D à partir d’images, le masquage automatique et les améliorations de l’UX.
helpx_creative_field: ""
helpx_description: Sampler > Release Notes > Version 4.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 4.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 1%

---


# Version 4.0

Avec **Substance 3D Sampler 4.0**, vous pouvez utiliser des images réelles pour créer des objets 3D avec masquage automatique du sujet, mappage de texture et décimation de la géométrie. Cette version introduit quelques améliorations UX en tant que nouvelles possibilités dans l&#39;API Python.

*Date de publication : 31 janvier 2023*

![](../assets/main-promo.jpg)

## Capture 3D

Avec Substance 3D Sampler 4.0, vous pouvez désormais créer des objets 3D à partir d’images.

Nous avons intégré des capacités de photogrammétrie. La photogrammétrie est le processus technique de prise de mesures à partir d&#39;images. C’est ainsi que Sampler crée des maillages 3D à partir d’une série de photos.

Tout ce dont vous avez besoin pour commencer est une série de photos qui capturent les surfaces visibles d’un objet - un smartphone ou un appareil photo DLSR fonctionne parfaitement.

Découvrez le workflow étape par étape [ici](../features-and-workflows/3d-capture.md).

## Tons clairs

### Masquage automatique

Supprimez l’arrière-plan de l’objet dont vous souhaitez appliquer la Capture 3D. Créez un masque généré automatiquement de l’objet après avoir importé vos images via l’onglet Masque.

L&#39;utilisation de masques présente de nombreux avantages. Il permet de détecter les éléments et de reconstruire uniquement les zones non masquées.

![](../assets/release-page-masking.jpg){width="500px"}

### Définition de votre zone de reconstruction

Activez/désactivez la Zone d&#39;intérêt pour activer un cadre de sélection après l’alignement de vos images. Définissez et alignez la zone précise à reconstruire.

![](../assets/3d-capture-bounding-box-modified.png){width="500px"}

### Post-traitement connecté

Une fois votre objet 3D reconstruit, optimisez le résultat avec la décimation automatique, le déballage UV et la cuisson.

Le post-traitement vous aide à adapter et à optimiser votre maillage et vos textures en fonction de vos besoins et de la façon dont vous souhaitez les utiliser.

Le résultat de la reconstruction peut générer un maillage avec des millions de polygones et jusqu’à 16K textures. Souvent, cette fonctionnalité n’est pas optimisée pour le rendu, l’expérience en temps réel ou en réalité augmentée.

L&#39;étape de post-traitement enchaîne automatiquement 4 étapes:

* Décimation
* Déballer UV
* Reprojection
* Baking

![](../assets/release-page-post-processing.jpg){width="500px"}

### Export aux principaux formats de fichier

Exportez vos objets 3D reconstruits dans tous les formats de fichiers standard afin de pouvoir les utiliser où vous le souhaitez.

![](../assets/v4-0-0-export.jpg){width="500px"}

## Viewport

Les fenêtres 2D et 3D peuvent être redimensionnées, permutées et empilées verticalement.

![](../assets/screenshot-2023-01-25-at-16-23-09.png){width="500px"}

## Script

Nous avons divisé la fonction d’exportation en 4 éléments :

* exporter les matériaux : `export_material`
* exporter les éclairages de l&#39;environnement : `export_environment_light`
* exporter un filet avec ou sans textures : `export_mesh` ou `export_3d_object`

Nous avons ajouté une nouvelle fonction pour importer des textures avec un usage spécifique : `import_textures`

Sampler charge désormais au démarrage le script et les plug-ins stockés dans des chemins définis par deux variables d’environnement :

* `SAMPLER_PLUGIN_PATH`
* `SAMPLER_SCRIPT_PATH`

## Tutoriels

## Note de mise à jour

1. **0,0 Banane**

   *(Publié Le 31 Janvier 2022)*

   **Ajouté**

* [capture 3D] Création d’objets 3D à partir d’images
* [capture 3D] Assistant capture 3D dédié
* [capture 3D] Importer ou générer des masques noir et blanc sur votre jeu de données
* [capture 3D] Résultat de l’alignement : affichez toutes les fonctions correspondantes sous forme de nuage de points
* [capture 3D] Résultat de l’alignement : visualisation et interaction avec les caméras associées à chaque photo alignée
* [capture 3D] Définition de la zone de reconstruction avec un widget de cadre de sélection
* [capture 3D] Redimensionnez, faites pivoter et translatez tous les axes du widget du cadre de sélection
* [capture 3D] Définir la précision de la géométrie pour le maillage reconstruit
* [capture 3D] Optimisez votre maillage et vos textures en créant une nouvelle version
* [capture 3D] Chacune des versions est automatiquement décimée selon le nombre de visages cibles défini
* [capture 3D] L’étape de post-traitement se déroule automatiquement, reprojette les textures, puis cuit les informations d’height et d’AO normales à partir du filet high-poly
* [capture 3D] Ajout du résultat original ou d’une version au projet Sampler
* [capture 3D] Nouveau calque de post-traitement du filet pour décimer, déballer, reprojeter les textures et ancrer automatiquement les détails du calque de filet sous-jacent
* [capture 3D] Nouveau calque de transformation de filet pour mettre à l’échelle, faire pivoter ou convertir le calque de filet sous-jacent
* [Exporter] Nouvelle fenêtre d’exportation
* [Exporter] Paramètres et interface utilisateur dédiés en fonction du type de ressource (matière, éclairage de l’environnement, filet)
* [Export] Exportez le maillage en tant que USD, USDA, USDZ, glTF, glb, obj, fbx, stl
* [Export] Définir le type de matériau lors de l&#39;exportation de fichiers de Substance (SBSAR, SBS)
* [UI] Déplacer les paramètres de cache vers un nouvel onglet dans le menu contextuel Préférences
* [Application] Les fenêtres 2D et 3D peuvent désormais être redimensionnées, permutées et empilées verticalement
* [Application] Nouvelle variable d’environnement SAMPLER\_RESOURCES\_PATH pour ajouter des ressources de démarrage supplémentaires
* [Scripting] Ajout de variables d’environnement SAMPLER\_PLUGIN\_PATH et SAMPLER\_SCRIPT\_PATH pour importer des plug-ins et des scripts au démarrage
* [Scripts] Ajout de fonctions d’exportation pour les matières, les éclairages de l’environnement et les objets 3D
* [Scripting] Ajout d’un identificateur, d’une valeur par défaut, de valeurs minimales et maximales, de libellés et de valeurs d’énumération aux paramètres
* [Scripts] Ajout de la fonction import\_textures pour définir une utilisation personnalisée lors de l’importation d’images

**Fixe**

* [Application] Blocage lors de l’ouverture d’un projet récent et de l’enregistrement dans la boîte de dialogue de confirmation
* La boîte de dialogue Fichier [Application] empêche l’ouverture des fichiers .ssa
* Les boîtes de dialogue de fichier [Application] peuvent apparaître dans une fenêtre en arrière-plan sur macOS
* [Application] Blocage potentiel lors de l’ouverture de projets 3.2
* [Application] La sélection d’un fichier ferme la boîte de dialogue Fichier avant d’afficher les avertissements
* [Paramètres exposés] L’exportation d’éclairages d’environnement paramétriques ne fonctionne pas
* [Calques] Le lien « Cliquer ici pour parcourir » dans la pile de calques ne fonctionne plus
* [Calques] Parfois, il n’est pas toujours possible de peindre plusieurs images dans un même calque
* [Calques] La définition d’une image dans les propriétés du calque ne met pas à jour la vignette du sélecteur d’images
* [Calques] L’ajustement d’une ressource Sampler ajoutée en tant que calque ne fonctionne pas
* [Projet] Mise à jour de ressource indésirable lors de l’ouverture d’un projet
* [Scripts] L’accès au dossier du plug-in échoue parfois sous Windows
* [Script] Blocage lors de l’utilisation de &#39;open\_project()&#39; dans un script Python
* [Scripts] L’exportation du JPEG est manquante dans l’API
* [Scripts] Le panneau Journal n’est pas en lecture seule
* [Scripting] la valeur du paramètre image\_picker ne fonctionne pas
* [UI] Icône d’élément manquante pour les éclairages de l’environnement dans le panneau Projet
* [UI] Le menu déroulant Envoyer au format Designer dans la fenêtre contextuelle Préférences peut être vide
* [UI] Certains boutons ont un style incorrect
* [UI] Le libellé chevauche les boutons dans les widgets Groupe de boutons
* [UI] La position de l&#39;info-bulle est incorrecte pour « Outils » dans le menu Définir la taille physique
* [UI] Lors de la modification de la langue, le menu Fichier est mal aligné

**Problèmes connus**

* [capture 3D] Lors de l’utilisation de masques, la projection de la texture peut être rompue
* [capture 3D] De petits artefacts peuvent apparaître sur votre objet si l’échelle de la transformation Filet est trop petite
* [capture 3D] Le maillage exporté peut être très petit. Réinitialiser l’échelle de la transformation de filet et réexporter
* [Sélecteur de couleurs] Le choix d’une couleur sur un deuxième moniteur avec une résolution différente peut ne pas fonctionner
* [Contenu] Le widget Lumière de forme ne fonctionne pas en mode projection sphérique
* [Interopérabilité] Le matériel avec displacement envoyé à Stager perdra les contrôles de displacement
