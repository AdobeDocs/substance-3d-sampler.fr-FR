---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/release-notes/old-versions/version-2019-1.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Sampler version 2019.1 pour en savoir plus sur la gestion de projet, les améliorations des piles de calques et les mises à jour de Delighter.
helpx_creative_field: ""
helpx_description: Sampler > Release Notes > Old Versions > Version 2019.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 2019.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '2043'
ht-degree: 0%

---


# Version 2019.1

**Substance Alchemist 2019.1 « Sésame »** vous permet de partager vos ressources avec sa nouvelle gestion de projet. La pile de calques a été entièrement reconstruite pour améliorer le workflow. Des contrôles et des informations supplémentaires ont été ajoutés au viewport. Une nouvelle version de notre delighter améliore la qualité et la précision de vos matériaux.

Date de publication : *4 novembre 2019*

>[!NOTE]
>
> **Remarque :** le contenu produit avec la version bêta 0.8.1 ou antérieure n&#39;est pas compatible avec la version 2019.1. Cependant, rien n&#39;est perdu et ces données sont toujours accessibles en lançant la version 0.8.1.

## Principales fonctionnalités

### Nouvel écran d’accueil

![](../../assets/sa-notes-welcomescreen.jpg)

Substance Alchemist dispose désormais d&#39;un écran d&#39;accueil qui vous permet de sauter rapidement sur votre dernier projet mais aussi d&#39;en créer de nouveaux. L&#39;écran d&#39;accueil fournit également quelques liens vers nos plateformes existantes, telles que [Substance Academy](https://academy.substance3d.com/).

### Gestion de projet

![](../../assets/sa-notes-openproject.png)

La version 2019.1 introduit la notion de projets, qui peuvent rassembler des collections de matériaux. Les projets peuvent également être exportés pour être partagés avec d’autres ordinateurs.

Pour en savoir plus sur les projets, voir : [Gestion de projets](../../getting-started/project-management.md).

### New Delighter

![](../../assets/sa-notes-delighter.jpg)

Nous avons amélioré notre delighter, qui est utilisé pour supprimer les ombres de vos photos. Il préserve désormais les détails et les couleurs d’origine des différentes surfaces, ce qui devrait améliorer la précision des matériaux générés.

### Nouvelle Pile de calques

![](../../assets/sa-notes-layerstack.png)

La Pile de calques a été reconstruite à partir de zéro pour élargir ses possibilités et ses actions. Les modifications notables sont les suivantes :

* **Les Matériaux et masques sont désormais accessibles directement via leur icône dédiée**\
  Lors de l’ajout d’un matériau dans la pile de calques, une nouvelle icône apparaît. Cliquez sur cette deuxième icône pour afficher les paramètres de fusion du matériau.

  ![](../../assets/sa-notes-layermask.png)
* **Le mode Fusion peut être modifié directement à partir de la barre d&#39;outils**\
  Désormais, lorsqu’un calque de Matériau est sélectionné, son mode de fusion peut être modifié directement à partir de la barre d’outils Pile de calques, sans avoir à cliquer dessus.

  ![](../../assets/sa-notes-layerstackblendmode.png)
* **Affecter un bitmap à des entrées de numérisation spécifiques**\
  Lors de l’importation d’un bitmap pour la création de vos matériaux à partir d’une numérisation, vous pouvez attribuer la bonne utilisation par bitmap.

  ![](../../assets/sa-notes-scanusage.png)

### Améliorations du viewport

![](../../assets/sa-notes-viewport.jpg)

Quelques nouvelles fonctionnalités ont été ajoutées au viewport qui améliorent son utilisation. Ces nouveaux paramètres sont accessibles dans le [panneau Paramètres du visualiseur](https://helpx.adobe.com/substance-3d/unlisted/documentation/sadoc/viewer-settings-188973164.html).

* **Mode Caméra**\
  Le mode de projection caméra permet de choisir entre Perspective et Orthographique.

  ![](../../assets/sa-notes-cameramode.png)
* **champ de vision de Caméra**\
  Vous pouvez désormais modifier le Champ de vision de caméra (FOV) du viewport. Le réglage de cette valeur peut aider à visualiser vos matériaux de manière réaliste. Le Champ de vision ne peut être contrôlé que lorsqu&#39;il est en mode projection de Perspective.

  ![](../../assets/sa-notes-viewport-fov.png)
* **Résolution et nombre de bits par pixel par canal**\
  La Vue 2D affiche désormais la résolution et le nombre de bits par pixel de texture de chaque couche.

  ![](../../assets/sa-notes-2dviewresolutiondepth.png)

## Notes de mise à jour

### 2019.1.4 Sésame

*(Publié Le 30 Janvier 2020)*

**Ajouté :**

* [Ressources] Invite de confirmation lors de l’effacement d’un dossier de ressources

**Fixe :**

* [Calques] Déplacez les calques vers deux calques ou plus en dessous ou au-dessus
* [Créer] Allocation d&#39;un budget VRAM suffisant pour avoir de bonnes performances

**Problèmes Connus :**

* Importer beaucoup de ressources peut vraiment ralentir la Substance Alchemist
* Les filtres Fond basé sur le contenu sont lents en haute résolution
* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Le filtre Normal à l’Height peut effectuer un crash sur MacOS

### 2019.1.3 Sésame

*(Publié Le 28 Janvier 2020)*

**Ajouté :**

* [Workflow] Prise en charge de plusieurs workflows
* [Workflow] Prise en charge du workflow de Brillance de Specular PBR
* [Workflow] Nouveau panneau Paramètres de canal
* [Workflow] Sélection du workflow lors de la création du projet
* [Paramètres des canaux] Activer/désactiver un calcul de canal spécifique
* [Paramètres des canaux] Affiche la liste des canaux personnalisés disponibles dans le matériau actif
* [Paramètres des canaux] calcul automatique des canaux personnalisés si nécessaire
* [Paramètres des canaux] Forcer/Bloquer le calcul des canaux personnalisés
* [Calques] Nouvelle interface utilisateur de l’espace réservé d’entrée de matériau dans les filtres Atlas scatter et Éclaboussure
* [Calques] Le Paramètre d&#39;entrée d’image d’un filtre peut être alimenté par les calques sous-jacents
* [Calques] Affiche une notification lorsque certains calques sont obsolètes
* [Calques] Possibilité de mettre à jour vers la dernière version des calques obsolètes via la notification
* [Projet] Nouveaux champs de métadonnées lors de la création du projet
* [Inspire] Les variations générées sont spécifiques à un projet
* [vue 2D] Basculer entre les entrées de calque, les sorties de calque et les sorties de matériau
* [Écran d’accueil] Option Ajouter un projet d’importation (.alch)
* [Préférences] Nouvelle fenêtre Préférences pour définir l’emplacement du cache et les paramètres de confidentialité des analyses
* [UI] Nouveaux boutons d’interface utilisateur
* [Performance] Amélioration globale du système de parallélisation
* [Performance] Optimisation du nombre de calculus de matériau
* [Moteur] Mise à jour de la Substance Engine
* [Framework] Mise à niveau vers Qt 5.13
* [MacOS] Améliorations globales de la prise en charge de macOS Catalina
* [Contenu] Filtre de réglage - Intensité normale et paramètres d’inversion

**Fixe :**

* [Calques] Désactiver le Paramètre d&#39;entrée de l’image lors de la suppression du calque
* [Calques] Correction d’un crash lors de l’ajout d’un calque de patch de duplication
* [Calques] Correction de certains crashs lors de la fusion de matériaux de pile de calques dans d’autres matériaux de pile de calques
* [Exportation] La sélection de canaux pour l’exportation est maintenant respectée.
* [Ressources] Ne pas effectuer de crash lors de la navigation dans le panneau Ressources
* [Ressources] Correction du crash lors de l’importation de fichiers de Substance corrompus
* [Ressources] Réduire le nombre de crashs lors du chargement de dossiers volumineux
* [Vignette] Le calcul de la vignette ne fige pas l’interface
* [Importation d’image] Uniformisation du type d’image prise en charge dans l’application
* [Paramètre prédéfini] Enregistre la description lors de la création d’un paramètre prédéfini à partir d’un SBSAR
* [Inspire] Correction du glisser-déposer d’image
* [Application] Corriger les crashs à la sortie
* [Application] Correction des crashs à la sortie lors de l’exportation de matériaux
* [UI] Correctifs et améliorations
* [UI] Renommer la ressource temporaire en « matériau non enregistré »
* [Contenu] Mise à jour globale et nettoyage de tous les filtres

**Problèmes Connus :**

* Importer beaucoup de ressources peut vraiment ralentir la Substance Alchemist
* Les filtres Fond basé sur le contenu sont lents en haute résolution
* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Le filtre Normal à l’Height peut effectuer un crash sur MacOS

### 2019.1.2 Sésame

*(Publié Le 11 Décembre 2019)*

**Ajouté :**

* [Workflow] Prise en charge de plusieurs workflows
* [Workflow] Prise en charge du workflow de Brillance de Specular PBR
* [Workflow] Nouveau panneau Paramètres de canal
* [Workflow] Sélection du workflow lors de la création du projet
* [Paramètres des canaux] Activer/désactiver un calcul de canal spécifique
* [Paramètres des canaux] Affiche la liste des canaux personnalisés disponibles dans le matériau actif
* [Paramètres des canaux] calcul automatique des canaux personnalisés si nécessaire
* [Paramètres des canaux] Forcer/Bloquer le calcul des canaux personnalisés
* [Calques] Nouvelle interface utilisateur de l’espace réservé d’entrée de matériau dans les filtres Atlas scatter et Éclaboussure
* [Calques] Le Paramètre d&#39;entrée d’image d’un filtre peut être alimenté par les calques sous-jacents
* [Calques] Affiche une notification lorsque certains calques sont obsolètes
* [Calques] Possibilité de mettre à jour vers la dernière version des calques obsolètes via la notification
* [Projet] Nouveaux champs de métadonnées lors de la création du projet
* [Inspire] Les variations générées sont spécifiques à un projet
* [vue 2D] Basculer entre les entrées de calque, les sorties de calque et les sorties de matériau
* [Écran d’accueil] Option Ajouter un projet d’importation (.alch)
* [Préférences] Nouvelle fenêtre Préférences pour définir l’emplacement du cache et les paramètres de confidentialité des analyses
* [UI] Nouveaux boutons d’interface utilisateur
* [Performance] Amélioration globale du système de parallélisation
* [Performance] Optimisation du nombre de calculus de matériau
* [Moteur] Mise à jour de la Substance Engine
* [Framework] Mise à niveau vers Qt 5.13
* [MacOS] Améliorations globales de la prise en charge de macOS Catalina
* [Contenu] Filtre de réglage - Intensité normale et paramètres d’inversion

**Fixe :**

* [Calques] Désactiver le Paramètre d&#39;entrée de l’image lors de la suppression du calque
* [Calques] Correction d’un crash lors de l’ajout d’un calque de patch de duplication
* [Calques] Correction de certains crashs lors de la fusion de matériaux de pile de calques dans d’autres matériaux de pile de calques
* [Exportation] La sélection de canaux pour l’exportation est maintenant respectée.
* [Ressources] Ne pas effectuer de crash lors de la navigation dans le panneau Ressources
* [Ressources] Correction du crash lors de l’importation de fichiers de Substance corrompus
* [Ressources] Réduire le nombre de crashs lors du chargement de dossiers volumineux
* [Vignette] Le calcul de la vignette ne fige pas l’interface
* [Importation d’image] Uniformisation du type d’image prise en charge dans l’application
* [Paramètre prédéfini] Enregistre la description lors de la création d’un paramètre prédéfini à partir d’un SBSAR
* [Inspire] Correction du glisser-déposer d’image
* [Application] Corriger les crashs à la sortie
* [Application] Correction des crashs à la sortie lors de l’exportation de matériaux
* [UI] Correctifs et améliorations
* [UI] Renommer la ressource temporaire en « matériau non enregistré »
* [Contenu] Mise à jour globale et nettoyage de tous les filtres

**Problèmes Connus :**

* Importer beaucoup de ressources peut vraiment ralentir la Substance Alchemist
* Les filtres Fond basé sur le contenu sont lents en haute résolution
* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Le filtre Normal à l’Height peut effectuer un crash sur MacOS

### 2019.1.1 Sésame

*(Publié Le 26 Novembre 2019)*

**Ajouté :**

* [Fusion] Nouveau mode de Fusion d’opacité
* [Moteur] Nouvelle version de Substance Engine

**Fixe :**

* [Calques] Corriger le crash lors de la suppression d’un calque en cours de calcul
* [Calques] Corriger le crash lors de la suppression du calque inférieur
* [Calques] Corriger le crash lorsque le nom du matériau contient des caractères spéciaux
* [Calques] Arrêtez de calculer tous les filtres qui utilisent un widget
* [Calques] Éviter les crashs lors de l’utilisation des filtres Correctif de Clone et Remplissage d’après le contenu
* [Calques] Correction du crash lors du glisser-déposer d’un filtre dans des emplacements d’entrée de projection
* [Ressources] Correction du crash lors de la liaison de dossiers locaux ou de l’importation de ressources dans la Substance Alchemist
* [Collection] Corriger le crash lors du basculement rapide entre les matériaux
* [UI] Corriger le crash lorsque la valeur est nulle ou non valide dans la répétition, curseurs de displacement sur le viewport
* [Inspire] Correction du crash lors de l’accès à l’onglet Inspire
* [Inspire] Corriger le crash tout en inspirant sur un matériau de pile de calques qui vient d’être enregistré
* [Performances] Les matériaux et les filtres à Substance lourde (Répétition) se calculent plus rapidement
* [Aide] Correction du fichier journal d’exportation
* [Contenu] Le filtre Aléatoire fonctionne sur tous les canaux
* [Contenu] Le workflow multiangle prend en compte toutes les numérisations
* [Contenu] Fusion correcte de la Fusion AO
* [Contenu] Fusion correcte de la Fusion de Courbure
* [Contenu] Mélange correct de la Fusion d’ID de couleur
* [Contenu] Fusion correcte de la Fusion de masque personnalisée
* [Contenu] Filtre Correction pour la modification des rugosités
* [Contenu] Correction du filtre de Matériau de base pour le téléchargement de canaux normaux personnalisés
* [Contenu] Correction du modèle d’importation personnalisé du filtre Estampage

**Problèmes Connus :**

* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Le filtre Normal à l’Height peut effectuer un crash sur MacOS

### 2019.1 Sésame

*(Publié Le 4 Novembre 2019)*

**Ajouté :**

* [Projet] Création d&#39;un projet
* [Projet] Introduction du format de fichier .alch qui contient les données du projet
* [Projet] Exportez un projet .alch contenant les collections et leurs matériaux
* [Projet] Importer un projet .alch
* [Projet] Ouvrir les projets récents
* [Écran d’accueil] Un écran d’accueil s’affiche au lancement
* [Écran d’accueil] Créer un projet à partir de l’écran d’accueil
* [Écran d’accueil] Accédez à la liste de tous vos projets dans l’écran d’accueil
* [Écran d’accueil] Liens rapides pour accéder à la documentation, aux informations sur les fenêtres contextuelles et la gestion des licences
* [Menu Fichier] Intégration d&#39;un menu Fichier
* [Menu Fichier] Accédez aux commandes du projet à partir de l’onglet Fichier et de l’enregistrement de la pile de calques
* [Menu Fichier] Accédez aux commandes Annuler et Rétablir depuis l’onglet Edition
* [Menu Fichier] Le menu Aide précédent a été déplacé dans le menu Fichier sous l’onglet Aide
* [Calques] Nouvelle architecture de la pile de calques
* [Calques] Nouvelle interface utilisateur de la pile de calques
* [Calques] Sélectionnez le mode de fusion directement dans la barre d’outils
* [Calques] Accédez séparément aux paramètres de fusion et aux paramètres de matériau
* [Calques] Ajoutez des matériaux directement dans les entrées dédiées du filtre Éclaboussure de la pile de calques
* [Calques] Modifier l’ordre de numérisation directement dans le calque d’importation d’image
* [Viewport] Contrôle du champ de vision de caméra
* [Viewport] Possibilité de basculer entre la caméra orthographique ou perspective
* [Viewport] Affichage des informations de résolution et de nombre de bits par pixel pour chaque couche
* [Ressources] Matériaux de base ouverts par défaut
* [Cache] Recherchez le dossier de cache des vignettes.
* [Cache] Recherche du dossier de cache de rendu
* [Panneaux] Le panneau Paramètres de Matériau est temporairement masqué
* [Workflow] Specular/Brillance temporairement désactivé
* [MacOS] Authentification notariale de la version du système d’exploitation Catalina
* [Contenu] Nouvelle version du filtre Delighter
* [Contenu] Nouveau filtre Image avec fond basé sur le contenu
* [Contenu] Nouveau filtre Matériau Fond basé sur le contenu
* Le filtre de Transforme [Contenu] dispose d’une option de transforme sécurisée

**Fixe :**

* Tous les bugs précédents liés à Créer ne sont pas valides aujourd’hui avec la nouvelle version de l’interface utilisateur et de l’architecture
* Les info-bulles ne masquent pas les icônes de la barre supérieure (3D, 2D, 2D/3D).
* [Contenu] Le filtre Éclaboussure accepte Atlas avec une map height complète
* [Contenu] Le filtre Transforme fonctionne sur les images (scan1, scan2,...)

**Problèmes Connus :**

* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Le filtre Normal à l’Height peut effectuer un crash sur MacOS

**Ajouté :**

* [Fusion] Nouveau mode de Fusion d’opacité
* [Moteur] Nouvelle version de Substance Engine

**Ajouté :**

* [Fusion] Nouveau mode de Fusion d’opacité
* [Moteur] Nouvelle version de Substance Engine

**Ajouté :**

* [Workflow] Prise en charge de plusieurs workflows
