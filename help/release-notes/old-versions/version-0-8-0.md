---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/release-notes/old-versions/version-0-8-0.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Sampler version 0.8.0 pour en savoir plus sur les nouvelles fonctionnalités, les mises à jour et les améliorations.
helpx_creative_field: ""
helpx_description: Sampler > Release Notes > Old Versions > Version 0.8.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 0.8.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---


# Version 0.8.0

**Ajouté :**

* [Ressources] Connectez et mettez en miroir vos dossiers de matières sur vos disques locaux
* [Ressources] Parcourez vos dossiers de matières et leurs sous-dossiers
* [Ressources] Dissociez le panneau Ressources matérielles dans une fenêtre distincte pour afficher vos ressources en plein écran
* [Ressources] Nouvelle disposition du panneau Ressources pour prendre en charge la navigation dans les dossiers et sous-dossiers
* [Ressources] Utilisez le chemin de navigation pour naviguer dans vos dossiers
* [Ressources] Forcez la synchronisation de votre dossier local avec l’option Synchroniser accessible via un clic droit.
* [Ressources] Déconnectez votre dossier local avec l’option Déconnecter accessible via un clic droit
* [Gérer] Afficher les balises incorporées des fichiers de Substance
* [Gérer] Ajoutez, modifiez et supprimez des balises de vos matériaux
* [Gérer] Évaluer vos matières
* [Calques] Prise en charge de la sortie en panorama
* [Calques] Vous pouvez supprimer les entrées d’image dans le calque Importation d’image
* [Calques] Sélection automatique du nouveau calque ajouté
* [Calques] Sélection automatique du calque en dessous après une suppression de calque
* [UX] Maintenir la visibilité des panneaux de gauche lors du passage à un autre laboratoire
* [UX] Ne créez pas de calque de base et n’ouvrez pas la fenêtre contextuelle Workflow de matériau lors de l’importation d’images dans une pile de calques non vide
* [UI] Nouveau style de champ de texte
* [UI] Nouveau style de zone de recherche
* [UI] Nouveau style d’en-tête de panneau
* [UI] Nouveau style d&#39;indicateur Occupé
* [UI] Nouveau style d’arrière-plan de pile de calques
* [UI] Utiliser la police Adobe Clean
* [UI] Supprimer l’icône de pipette de l’espace réservé du paramètre d’entrée de couleur
* [Performance] Optimisation de l&#39;indicateur Occupé
* [Contenu] Nouveau filtre Générateur de motifs
* [Contenu] Nouveau filtre Flou

**Fixe :**

* [Inspire] Correction du blocage lors de l’utilisation de plus de 10 couleurs
* [Vue 2D] Corriger la barre de défilement dans la liste des canaux de la vue 2D
* [Visualiseur] Correction d’un blocage lors de l’importation d’une carte d’environnement non Power of 2
* [Contenu] Correction de l’importation au format PNG du motif personnalisé des filtres d’estampage et de perforation
* [Export] Correction de l’exportation normale et height 16 bits par canal
* Correction d’une boucle infinie lors de l’importation d’un matériau avec deux paramètres prédéfinis portant le même nom
* Correction de l’affichage du chemin de fichier long dans le calque de Matériau de base

**Problèmes Connus :**

* L’utilisation de plusieurs charmants dans un même matériau n’est pas recommandée
* Delighter se bloque avec les anciens pilotes NVIDIA (moins de 400.x)
* Le basculement rapide de visibilité d’une scène Delighter n’est pas recommandé
* Les images Tif ne s’affichent pas dans le panneau Propriétés du calque d’importation d’image
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Le filtre Normal à l’height peut se bloquer sur MacOS
* Peut se bloquer de manière aléatoire lors de la fermeture sur MacOS
