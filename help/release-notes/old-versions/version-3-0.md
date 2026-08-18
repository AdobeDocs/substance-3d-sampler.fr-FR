---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/release-notes/old-versions/version-3-0.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Sampler version 3.0 pour en savoir plus sur la refonte de l’interface utilisateur, les éclairages de l’environnement, les filtres et l’intégration du Creative Cloud.
helpx_creative_field: ""
helpx_description: Sampler > Release Notes > Old Versions > Version 3.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 3.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '2019'
ht-degree: 0%

---


# Version 3.0

**Substance 3D Sampler 3.0.0** est le nouveau nom de Substance Alchemist maintenant qu&#39;il est connecté à Adobe Creative Cloud. Il apporte une refonte complète de l&#39;interface utilisateur, la prise en charge de la création de lumières d&#39;environnement, des filtres entièrement retravaillés et nouveaux, la fonctionnalité Envoyer vers et la prise en charge du shader ASM.

Date de publication : *23 juin 2021*

## Principales fonctionnalités

### Nouvelle interface et gestion des panneaux

Avec un nouveau nom, vient un nouveau look. L’interface utilisateur de Sampler a été entièrement remaniée pour permettre une plus grande personnalisation et un accès plus facile.

![](../../assets/ui-dualscreen.jpg){width="600px"}

Les panneaux peuvent être ancrés et non ancrés, ce qui vous permet d’utiliser pleinement une configuration à double écran.

### Nouveau workflow de projet

![](../../assets/ui-project-panel.png)

Sampler fonctionne désormais avec les projets. Le panneau [Projet](../../interface/panels/project-panel.md)vous permet de gérer et de regrouper vos ressources par projet. Les projets sont stockés dans des fichiers Sampler de Substance de données, facilement partagés.

### Nouveau panneau Actifs

![](../../assets/image2021-6-22-17-58-15.png)

Le panneau [Actifs](../../interface/panels/assets-panel.md) est une nouvelle conception commune du panneau Ressources, combinée à vos collections.

* 3 Sections : Ressources de démarrage + Vos ressources + Dossiers locaux connectés
* Prise en charge de nouveaux types de ressources : filtres et images
* Vue étroite/large
* Filtres et filtres de recherche

### Création d’un nouvel environnement clair

![](../../assets/idl.jpg){width="600px"}

Sampler vous permet désormais de faire plus que de simples matériaux. Les éclairages de l&#39;environnement sont un nouveau type de ressource avec leur [propre ensemble de filtres](../../filters/hdri-tools/hdri-tools.md). Commencez à partir de [photos 360 entre crochets](../../filters/hdri-tools/hdr-merge.md), créez un éclairage d&#39;environnement [à partir de zéro](../../filters/hdri-tools/shape-light.md) ou [modifiez un fichier HDR existant](../../filters/hdri-tools/nadir-patch.md).

### Filtres retravaillés et nouveaux

![](../../assets/filter-all-filters.jpg){width="600px"}

Tous les filtres existants ont été retravaillés :

* Prise en charge des couches de spécification technique/brillance.
* Prise en charge des masques personnalisés
* Noms de paramètres normalisés
* Icônes pour presque tous les filtres

Le filtre de réglage a été divisé en différents filtres en fonction de la fonctionnalité, pour imiter Photoshop :

![](../../assets/filter-adjustment-filters.jpg)

Quelques nouveaux filtres ont été ajoutés :

* [Transformation de déformation](../../filters/tools/warp-transform.md)
* [Tisser](../../filters/generators/weave.md)
* [Panneau](../../filters/generators/panel.md)

### Nouvelle fonctionnalité Envoyer vers

![](../../assets/image2021-6-22-18-2-10.png)

Sampler peut désormais [facilement partager des matériaux et des environnements lumineux](../../interface/panels/share-panel.md)avec Substance 3D Painter et Stager, en un seul clic.

### Nouveau moteur de rendu en temps réel

* Prise en charge des matériaux ASM, permettant des looks cohérents entre les applications avec davantage de canaux de matériaux.
* Basculer entre 2 [moteurs en temps réel](https://helpx.adobe.com/substance-3d/unlisted/documentation/sadoc/viewer-settings-188973164.html)
* Possibilité de contrôler les textures par défaut sur un filet

### Améliorations générales

* Nouvelles langues
* Réactivité des applications
* Prise en charge des textures non carrées
* Outils Annuler/Rétablir
* Attribution d’utilisations personnalisées aux images dans le calque d’importation d’image
* Réinitialisation de la valeur d’un paramètre
* Progression de l’exportation dans la barre des tâches de Windows

## Tutoriels

Vous trouverez ci-dessous nos tutoriels vidéo couvrant les nouvelles fonctionnalités :

## Notes de mise à jour

### 3.0.0 Gaufre

*(Publié Le 23 Juin 2021)*

**Ajouté :**

* [Branding] La Substance Alchemist devient Adobe Substance 3D Sampler
* [Branding] Nouvelles icônes d’application
* [UI] Nouvelle expérience utilisateur et interface utilisateur
* [UI] Nouvel écran de démarrage
* [UI] Les panneaux sont non ancrables et ancrables dans l’interface
* [UI] Ancrez jusqu’à 3 panneaux dans la même colonne
* [UI] Ancrez jusqu’à 3 panneaux dans le même panneau (onglets)
* [UI] Désancrer les panneaux pour créer une fenêtre distincte dans le même écran ou dans un écran différent
* [UI] Fenêtre contextuelle des panneaux fermés lorsque vous cliquez sur leurs icônes
* [UI] Réorganisez vos barres gauche et droite en déplaçant les icônes des panneaux
* [UI] Nouvelle barre d’outils pour accéder directement à des filtres spécifiques (Recadrage, Transformation, Transformation de perspective, Tampon de duplication)
* [UI] Nouveau bouton « Obtenir le contenu » dans la barre de gauche
* [UI] Importez des fichiers directement dans vos ressources à l’aide du bouton Obtenir du contenu
* [UI] Importez des fichiers directement dans vos calques à l’aide du bouton Obtenir du contenu
* [UI] Accès direct au site Web Substance 3D Assets d’Adobe à l’aide du bouton Obtenir le contenu
* [UI] Le widget Résolution est désormais directement accessible dans la clôture
* [UI] Tous les éléments de l’interface utilisateur sont désormais chargés dynamiquement
* [UI] Raccourci : utilisez « 2 » pour activer/désactiver la visibilité de la vue 2D
* [UI] Raccourci : utilisez « 3 » pour activer/désactiver la visibilité de la vue 3D
* [Écran d’accueil] Créez un projet en un clic avec le bouton Nouveau.
* [Écran d’accueil] Nouvelle bannière d’illustration
* [Projet] Tous les projets sont désormais associés à un fichier unique
* [Projet] Nouvelle extension de fichier de projet .ssa
* [Projet] L’option Enregistrer en tant que projet vous demande de sélectionner l’emplacement où enregistrer votre projet
* [Projet] Lors de la fermeture de Sampler, vous serez invité à enregistrer votre projet s’il n’est pas enregistré
* [Projet] Lors de la fermeture de Sampler, vous serez invité à enregistrer votre projet en cas de modifications depuis le dernier enregistrement
* [Projet] Le nom de votre projet s’affiche au-dessus de la clôture
* [Projet] Le nom du projet est en italique avec une étoile s’il n’est pas enregistré ou s’il contient des modifications depuis le dernier enregistrement
* [Projet] Ouvrez un fichier de projet .ssa directement à partir de votre explorateur de système d’exploitation
* [Projet] L’ouverture d’un fichier .sbsar à partir de votre explorateur de système d’exploitation lance Sampler avec un nouveau projet contenant ce fichier .sbsar prêt à l’emploi
* [Projet] Ouvrez un fichier .alch (fichier de Substance Alchemist hérité) à partir de l’explorateur de votre système d’exploitation
* [Panneau Projet] Nouveau panneau contenant tous les actifs créés dans un projet
* [Panneau Projet] Créez un élément (matériau ou éclairage de l’environnement) à l’aide de l’icône +
* [Panneau Projet] Un clic droit sur la ressource ouvre un menu contextuel
* [Panneau Projet] À partir du menu contextuel accessible via un clic droit, vous pouvez supprimer une ressource
* [Panneau Projet] À partir du menu contextuel accessible via un clic droit, vous pouvez dupliquer une ressource
* [Panneau Projet] À partir du menu contextuel accessible via un clic droit, vous pouvez renommer une ressource
* [Panneau Projet] Le basculement entre les ressources ne perdra pas les modifications
* [Résolution] Vous pouvez désormais définir une résolution non carrée pour tous vos actifs
* [Résolution] La valeur de résolution est enregistrée par ressource dans un projet
* [Luminosité de l’environnement] Créer une luminosité de l’environnement dans Substance 3D Sampler
* [Éclairage de l’environnement] Lors de la création d’un éclairage de l’environnement, le glisser-déposer d’images affichera la fenêtre Modèle de création d’éclairage de l’environnement
* [Luminosité de l’environnement] Dans le modèle de création Lumière de l’environnement, sélectionnez Importation de l’environnement pour attribuer votre image à l’environnement dans la vue 3D
* [Éclairage de l’environnement] Dans le modèle de création d’éclairage de l’environnement, sélectionnez Fusion HDR pour créer un éclairage de l’environnement à partir de plusieurs images à 360 degrés avec une exposition différente
* [Luminosité de l’environnement] Dans le modèle de création Lumière de l’environnement, sélectionnez « Utiliser comme bitmap » pour modifier vos images avant de créer une luminosité de l’environnement
* [Luminosité de l’environnement] Affectez l’utilisation de l’environnement dans le calque d’importation d’image pour affecter directement l’image à l’environnement dans la vue 3D
* [Luminosité de l’environnement] Dans la vue 2D de la couche d’environnement, une correction automatique des couleurs permet d’obtenir un rendu identique à celui de la vue 3D
* [Éclairage de l’environnement] Nouveau contenu dédié à la création d’éclairage de l’environnement
* [Panneau Actifs] Les panneaux Ressources et Filtres sont fusionnés dans un nouveau panneau Actifs
* [Panneau Actifs] Le panneau Actifs prend désormais en charge les types d’actifs suivants : matières, filtres et images
* [Panneau Ressources] Toutes les ressources de démarrage sont accessibles dans la section Ressources de démarrage
* [Panneau Actifs] La section Actifs de démarrage est en lecture seule
* [Panneau Actifs] Nouvelle section « Vos actifs »
* [Panneau Actifs] La section « Vos actifs » est l’endroit où vous pouvez importer toutes vos ressources
* [Panneau Actifs] Tous les actifs de « Vos actifs » sont ajoutés dans un dossier spécifique de vos documents
* [Panneau Actifs] Connectez des dossiers locaux dans le panneau Actifs pour ajouter de nouvelles sections
* [Panneau Actifs] La recherche porte sur le dossier actuel et ses sous-dossiers
* [Panneau Actifs] Naviguez entre les dossiers et les sous-dossiers à l’aide des chemins de navigation
* [Panneau Actifs] Filtrez le dossier actuel par matériau, par filtre ou par image
* [Panneau Actifs] Combinez plusieurs filtres pour obtenir uniquement des matières et des images
* [Panneau Actifs] Modifiez l’affichage en basculant entre une grille ou une liste
* [Panneau Actifs] Les filtres sont représentés par leur icône
* [Panneau Actifs] Les images sont représentées avec leur aperçu
* [Panneau Actifs] L’augmentation de la largeur modifie la disposition du panneau avec une vue spécifique pour naviguer entre les dossiers
* [Panneau Actifs] Dans les sections non en lecture seule, supprimez un actif en le faisant glisser sur l’icône du chutier
* [Panneau Ressources] Un clic droit sur la ressource ouvre un menu contextuel
* [Panneau Actifs] À partir du menu contextuel obtenu via un clic droit, accédez aux métadonnées de l’actif (nom, catégorie, emplacement)
* [Panneau Actifs] Dans le menu contextuel accessible via un clic droit, supprimez l’actif (disponible uniquement dans les sections non en lecture seule)
* [Panneau Actifs] Dans le menu contextuel accessible via un clic droit, parcourez votre actif dans Adobe Bridge
* [Panneau Calques] Nouvelle icône pour ajouter directement un matériau de base sur vos calques
* [Panneau Calques] Le raccourci Maj + B ajoute un matériau de base au-dessus de vos calques
* [Panneau Calques] Les calques disposent désormais d’un aperçu en miniature (miniature de matériau, icône de filtre ou aperçu d’image)
* [Panneau Propriétés] Nouvelle conception du titre du panneau Propriétés avec le nom et la vignette de l’actif
* [Panneau Propriétés] Les calques de filtre prennent désormais en charge les paramètres prédéfinis
* [Panneau Propriétés] Sur le calque d’importation d’image, cliquez avec le bouton droit sur l’aperçu de l’image pour la modifier dans Photoshop
* [Adobe Bridge] La fonction Parcourir votre ressource dans Adobe Bridge lance Bridge à l’emplacement de la ressource
* [Adobe Photoshop] La fonction Modifier dans Adobe Photoshop ouvre l’image dans Photoshop, prête à être modifiée
* [Adobe Photoshop] À chaque enregistrement dans Adobe Photoshop, l’image modifiée est rechargée dans Sampler
* [Substance 3D Designer] Les ressources envoyées depuis Adobe Substance 3D Designer arrivent directement dans la section « Vos ressources » du panneau Ressources
* [Export] Envoyer des ressources directement vers Adobe Substance 3D Painter et Adobe Substance 3D Stager
* [Export] Envoyer des matériaux et des éclairages de l&#39;environnement vers Adobe Substance 3D Painter
* [Exporter] Envoyer les éclairages de l’environnement vers Adobe Substance 3D Stager
* [Rendu] Les nouvelles propriétés de matière sont désormais prises en charge et rendues en 3D
* [Rendu] Prise en charge de l’effet Reflet (Couleur de l&#39;éclat, opacité de Reflet et Rugosité de Reflet)
* [Rendu] Ajout de la prise en charge du revêtement (Couleur du revêtement, Rugosité du revêtement, Normale du revêtement, Specular level du revêtement et IOR du revêtement)
* [Rendu] Ajout de la prise en charge d’Anisotropie (niveau d’Anisotropie et angle d’Anisotropie)
* [Rendu] Ajout de la prise en charge de Specular edge color
* [Rendu] Activez ces nouvelles propriétés dans le panneau Paramètres de couche
* [Rendu] Introduction d’un nouveau moteur de rendu en temps réel (2021) dans la version Beta
* [Rendu] Basculez entre les deux versions de rendu dans le panneau Paramètres du visualiseur
* [Rendu] Le moteur de rendu Realtime Engine (2021) prend en charge les propriétés de translucidité, d’absorption et de diffusion des matériaux
* [Rendu] Le moteur de rendu Realtime Engine (2021) introduit une nouvelle façon de calculer les ombres à partir de la lumière de l’environnement
* [Rendu] Le moteur de rendu Realtime Engine (2021) calcule en temps réel l’irradiance de la lumière de l’environnement
* [Panneau Paramètres de l&#39;ombrage] Nouveau panneau Paramètres de l&#39;ombrage pour ajuster des paramètres d&#39;ombrage de matériau spécifiques
* [Panneau Paramètres de l&#39;ombrage] Nouveaux paramètres (Échelle normale, Échelle de l&#39;height, Niveau de l&#39;height, Intensité des émissions, IOR, Intensité normale du revêtement et IOR du revêtement)
* [Panneau Paramètres de l’ombrage] Paramètres spécifiques pour le moteur en temps réel 2021 (Diffusion sous la surface, Distance de diffusion, Décalage rouge et Diffusion Rayleigh)
* [Panneau Paramètres du nuanceur] Les valeurs des paramètres sont enregistrées par ressource
* [Panneau Paramètres de la visionneuse] Ajout d’un aperçu des éclairages de l’environnement par défaut
* [Panneau Paramètres de la visionneuse] Ajout d’un aperçu des maillages par défaut
* [Panneau Paramètres de la visionneuse] Nouveau paramètre d’opacité d’environnement
* [Panneau Paramètres de la visionneuse] Nouveau paramètre de flou d’environnement (spécifique au moteur de rendu Realtime Engine 2021)
* [Localisation] Nouvelles traductions en allemand et français
* [Contenu] Nouvelles matières de base par défaut
* [Contenu] Nouveaux éclairages d’environnement par défaut
* [Contenu] Tous les filtres ont été mis à jour, nettoyés et optimisés
* [Contenu] Le filtre Réglage a été divisé en plusieurs filtres
* [Contenu] Nouveau filtre Luminosité/Contraste
* [Contenu] Nouveau filtre Teinte/Saturation
* [Contenu] Nouveau filtre Vibrance
* [Contenu] Nouveau filtre Netteté
* [Contenu] Nouveau réglage Normal/Height
* [Contenu] Nouveau filtre Panneaux
* [Contenu] Nouveau filtre Doigt
* [Contenu] Nouveau filtre Tissus
* [Contenu] Nouveau filtre de transformation de déformation
* [Contenu] Nouvel Height du filtre AO
* [Contenu] Nouveau filtre Height à Normal
* [Contenu] Remplacement de couleur : remplacez-le dans les nouveaux canaux pris en charge (Reflet, Couchage, Anisotropie,...).
* [Contenu] Variation de couleur - Mode manuel pour sélectionner exactement les couleurs à modifier
* [Contenu] Mosaïque - option pour visualiser les coutures coupées
* [Contenu] Carrelage : option permettant de peindre les coutures découpées pour un carrelage parfait
* [Contenu] Correspondance : option permettant d’ajouter une matière correspondant à sa couleur et à sa rugosité
* [Contenu] Correspondance : fonctionne désormais sur les images pour correspondre à la couleur d’une autre image.
* [Contenu] Luminosité de l’environnement - Nouveau filtre de température de couleur
* [Contenu] Luminosité de l’environnement - Nouveau filtre Exposition
* [Contenu] Luminosité de l’environnement - Nouveau filtre Aperçu de l’exposition
* [Contenu] Luminosité de l’environnement - Nouveau filtre de Nadir patch
* [Contenu] Luminosité de l’environnement - Nouveau filtre de Nadir extract
* [Contenu] Luminosité de l’environnement - Nouveaux filtres Lumières (Sphère, Ligne, Forme, Plan)
* [Contenu] Luminosité de l’environnement - Nouveau filtre Correctif de panorama
* [Contenu] Luminosité de l’environnement - Nouveau filtre Redresser l’horizon
* [Contenu] Luminosité de l’environnement - Nouveau filtre de fusion HDR

**Problèmes Connus :**

* [Moteur en temps réel 2021] La modification de la mise en page entraîne le blocage de l’application
* [Realtime Engine 2021] Calcul lourd, blocage de l’application
* [Panneaux] MacOS : les panneaux non ancrés sont placés devant toutes les applications
* [Widgets] Les widgets Transformation et Positions peuvent disparaître. Masquez et affichez le calque pour les faire apparaître.
* [Exportation] L’exportation SBSAR d’une luminosité de l’environnement perd la précision à 32 nombres de bits par pixel
* [Panneau Actifs] Les actifs peuvent être mis en surbrillance lors de l’ouverture d’un dossier
* [Panneau Propriétés] La réinitialisation des paramètres ne réinitialise pas l’interface utilisateur de la zone de liste déroulante
* [Localisation] La modification de la langue n’affecte pas le panneau de projet tant qu’il n’est pas recréé
