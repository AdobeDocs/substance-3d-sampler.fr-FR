---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/release-notes/version-4-1.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Sampler version 4.1 pour en savoir plus sur le filtre Déformation de la Peinture, les mises à jour du filtre Broderie et les améliorations de capture 3D.
helpx_creative_field: ""
helpx_description: Sampler > Release Notes > Version 4.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 4.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---


# Version 4.1

<b>Substance 3D Sampler 4.1.0 </b>introduit un nouveau contenu avec le filtre <b>Déformation de la Peinture</b> et une version améliorée du filtre <b>Broderie</b>. Cette mise à jour inclut des améliorations de capture 3D.

*Date de publication : 28 mars 2023*

## Déformation de peinture

Le filtre Déformation de Peinture vous permet de déformer des matériaux en dessinant des courbes sur la Vue 2D.\
L’option Redresser vous permet de réaligner les matériaux pour un flux de répétition fluide et facile.

## Broderie

Le nouveau générateur de broderies vous permet de créer des retouches de broderie à partir d’un fichier vectoriel d’image unique ou d’un dessin.\
Il peut broder jusqu&#39;à 6 couleurs et combine plusieurs techniques de couture.

## Tutoriels

## Note de mise à jour

<b>4.1.2 CANNOLI</b>

*(Publié Le 20 Juin 2023)*

<b>Fixe :</b>

* [Calques] Fuite de mémoire lors du réglage des matériaux de Substance et des filtres provoquant des crashs

<b>4.1.1 CANNOLI</b>

*(Publié Le 6 Juin 2023)*

<b>Ajouté</b> :

* [Moteur] Mettre à jour la Substance Engine vers la version 9.0
* [Interopérabilité] Envoi d’objets 3D à Stager et Painter

<b>Fixe :</b>

* [capture 3D] crashs d&#39;applications en cas d&#39;échec du rendu capture 3D
* [capture 3D] Crash lorsqu’une image ne peut pas être chargée
* [capture 3D] Crash lorsque vous atteignez l’étape de reconstruction du Maillage
* [capture 3D] Crash lors du redimensionnement du cadre de sélection
* [capture 3D] L’importation de masques conformes à la convention n’affecte pas le masque correctement
* [capture 3D] Problèmes de rendu lors du réglage du cadre de sélection
* [capture 3D] Le basculement entre les options de rendu de version et de basculement pendant le post-processus Capture 3D est lent
* [capture 3D] Le basculement entre les versions pendant l’étape de post-traitement de capture 3D est parfois interrompu
* crash [Application] au démarrage
* crash [Application] lors de la duplication d’un matériau renommé
* crash [Application] lors de l’ouverture d’un projet .alch hérité sans son dossier de dépendances
* [Application] Crash lors de la connexion/déconnexion d’un écran, l’ordinateur se met en veille ou est accessible à distance
* [Application] Crashs et fuites de mémoire liés à la gestion non persistante des actifs
* [Exporter] Le choix du format de matériau pour les types de fichiers d’objet 3D qui intègrent ou référencent des textures doit être désactivé
* [Exportation] Crash en cas de problème lors de l’exportation d’objets 3D
* [Export] Crash lors de l&#39;exportation d&#39;un fichier .sbs/.fichier sbsar
* [Exporter] Crash lors de l’importation d’un paramètre prédéfini personnalisé ayant la même étiquette mais pas le même nom de fichier
* [Exporter] L’exportation d’un éclairage d&#39;environnement vers un fichier .sbs/.fichier sbsar ne fonctionne pas toujours
* [Export] L’exportation Gltf/Glb code les textures dans base64
* Le champ de texte Nom de [Export] ne fonctionne pas lors du recentrage
* [Exporter] La répétition Conserver ne fonctionne pas lors de l’exportation d’une image vers un calque Matériau (alimenté par l’IA) vers un fichier .sbs/.fichier sbsar
* [Export] Lors de l&#39;exportation gltf et du remplacement de fichiers, la liste des fichiers à remplacer n&#39;est pas correcte
* [Paramètre exposé] La valeur de départ aléatoire ne fonctionne pas dans les fichiers .sbs/.sbsar exportés
* [Calques] L’outil Remplissage d’après le contenu crash parfois lorsqu’il est ajouté pour la deuxième fois
* crash [Calques] lors du calcul d’une pile de calques
* [Calques] Le cache disque Image vers Matériau (AI) ne fonctionne pas
* [Calques] crash possible lors de l’ajustement d’un calque
* [Performance] Fuites de mémoire
* [Projet] Crash lors de l’enregistrement d’un projet
* [Projet] L’importation du même projet deux fois de suite duplique les ressources
* [UI] Les boutons arrondis avec une seule icône ne sont pas rendus correctement

### 4.1.0 Cannoli

*(Publié Le 28 Mars 2023)*

<b>Ajouté :</b>

* [Contenu] Nouveau filtre Broderie
* [Contenu] Nouveau filtre Déformation de Peinture
* [UI] Option Ajouter une exportation dans le menu Fichier
* [capture 3D] Le bouton Précédent est maintenant disponible à l’étape d’alignement
* [capture 3D] Images Gérer l&#39;orientation EXIF du JPEG
* [capture 3D] Script - Nouvelle propriété dataset\_info.caméra
* [capture 3D] Ajout de la prise en charge Linux (voir documentation)
* [capture 3D] Vérifier l’accès en lecture des images importées
* [Intégration] Formation : 2 nouveaux tutoriels (Broderie et déformation de la Peinture)
* [Intégration] Mise à jour du contenu Nouveautés

<b>Fixe :</b>

* [capture 3D] Conserver la position de la caméra lors du changement de version
* [capture 3D] Fusion de tous les groupes d’un objet en un seul
* [capture 3D] maillages générés renommés en Original
* crash [Application] lors de la tentative de génération d’une vignette d’image inexistante
* [Actifs] L’icône de la corbeille ne fait rien dans le panneau Actifs
* [Contenu] La mise à jour des filtres avec des emplacements de matériau ne fonctionne pas comme prévu
* [Export] crash possible lors de l’exportation d’une ressource avec des filtres spécifiques
* [Export] Exportation SBS/SBSAR : les calques d’importation d’image avaient la priorité sur les paramètres d’image
* [Export] Le paramètre prédéfini d&#39;exportation UE4 ne fonctionne pas avec PNG
* [Calques] Crash lors de la suppression simultanée d’un matériau et d’un filtre depuis l’explorateur du système d’exploitation
* [Calques] Crash lors du glissement d’un Fichier sbsar avec un fichier image
* [Calques] La couche d’opacité de la broderie peut être entièrement blanche
* [Localisation] Le chinois peut être affiché par défaut sous Linux
* [Performance] Correction d’un problème de mémoire lors de la suppression d’un calque d’une ressource
* [Projet] crash possible lors de l’enregistrement
* [UI] Ajouter un espacement manquant sur le bouton de menu de la version
* [UI] Le bouton Annuler ne s’affiche pas correctement
* [UI] Désactivation de l’animation des curseurs pour les paramètres de post-traitement capture 3D
* [UI] La fenêtre Modèle de création de Matériau ne se ferme pas lorsque vous cliquez en dehors
* [UI] L’outil d’accès rapide du filtre se ferme lorsqu’il clique en dehors

<b>Problèmes Connus :</b>

* [Sélecteur de couleurs] Le choix d’une couleur sur un deuxième moniteur avec une résolution différente peut ne pas fonctionner
* [Contenu] Le widget Lumière de forme ne fonctionne pas en mode projection sphérique
* [Interopérabilité] Le Matériau avec displacement envoyé à Stager perdra les contrôles de displacement
