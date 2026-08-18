---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/release-notes/version-5-1-substance-3d-sampler.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Sampler version 5.1 pour en savoir plus sur les nouvelles fonctionnalités, les améliorations et les améliorations de workflow.
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 5.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 2%

---


# Version 5.1

![](../assets/welcome_digitization_tool.jpg)

Passez moins de temps entre la capture de vos matériaux et l&#39;exportation de leurs jumeaux numériques avec des outils nouveaux et améliorés dans <b>Substance 3D Sampler 5.1</b> !

Les principales nouveautés sont les suivantes :

## Répétition automatique des matériaux structurés

Gagnez du temps en traitant des matériaux structurés ou à motifs (comme les tissus) en générant automatiquement des carreaux homogènes.

Plus d&#39;informations *[ici](../filters/tools/auto-tiling.md)*.

![](../assets/WhatsNew_Auto-tiling-5_1.jpg)

## Workflows de calques efficaces

Améliorez les performances et réduisez le temps de calcul avec le calque d’aplatissement en transformant les résultats des calques empilés en un seul ensemble de cartes au sein d’un calque unifié. Renommez-les et dupliquez-les pour plus d’efficacité !

Plus d&#39;informations *[ici](../features-and-workflows/flatten-layers.md)*.

![](../assets/WhatsNew_Flatten-Layers-5_1.png)

## Des outils puissants pour le traitement des numérisations

Grâce aux filtres Égaliser et Tampon de duplication améliorés, ainsi qu’à une nouvelle fonctionnalité de suppression automatique des plis pour les tissus, vous pouvez obtenir des numérisations parfaites en quelques clics, quelle que soit la complexité du matériau.

![](../assets/WhatsNew_Equalize-5_1.jpg)

## Prise en charge améliorée de HP Z Captis

Désormais, avec la génération de cartes de rugosité et la détection automatique de taille physique en mode Studio, vous obtenez un jumeau numérique de matériau plus détaillé et précis que jamais !

![](../assets/whatsnew-hp-z-captis-5-1.jpg)

## Notes de mise à jour V5.1

*(sortie : 7 août 2025)*

## Ajouté :

* [Vue 2D] La taille du pinceau s’adapte désormais à la résolution de texture actuelle
* [Vue 3D] Activez l’échelle d’affichage native pour le rendu 3D dans les préférences.
* [Application] Mise à jour du moteur de rendu
* [Captivate] Ajout de la possibilité de « rendre carré » lors de la prévisualisation
* [Captis] Détection automatique des tailles physiques
* [Captivate] La capture d’un nouveau matériau crée une nouvelle ressource.
* [Captivate] Modifiez la résolution de la sélection dans la liste déroulante en pixels par pouce ou centimètre au lieu de la résolution en pixels de la zone maximale
* [Captivate] Aide contextuelle sur l’étalonnage de l’alignement
* [Captivate] Générer une carte de rugosité
* [Captivate] Avertissez l’utilisateur si les fichiers d’étalonnage par défaut sont manquants
* [Filtres] Filtre Mosaïque automatique pour matériaux structurés et numérisations
* [Filtres] Nouveau filtre Suppression de pli
* [Filtres] Nouvelles fonctionnalités du filtre Tampon de duplication
* [Filtres] Nouvelles fonctionnalités du filtre Égaliser
* [Calques] Possibilité d’aplatir les calques
* [Calques] Menu contextuel lors d’un clic droit sur un calque pour renommer, dupliquer, supprimer ou aplatir le calque
* [Intégration] Mise à jour du contenu des écrans Bienvenue et Nouveautés
* [Performances] Meilleures performances lors de l’utilisation du filtre Recadrage
* [Performances] Amélioration de l’utilisation de la mémoire pour la vue 3D
* [Performances] La mise à jour de la vue 3D est plus rapide
* [Taille physique] Activer « Afficher avec rapport physique » lors de l’utilisation de filtres de Substance lorsque la Taille physique est activée
* [Taille physique] Lorsque vous importez des images dans une pile vide, proposez une résolution plus cohérente avec le rapport d’image
* [Actions rapides] 3 nouvelles actions rapides pour le traitement de la numérisation
* API [de script] pour aplatir les calques
* [Scripts] Obtenir le nom de fichier de chaque image d’un calque d’importation d’image
* [Scripting] Nouvelle fonction pour activer/désactiver un canal donné d’une ressource
* [UI] Retravaillez les icônes et les boutons du panneau Calques pour les adapter aux nouvelles fonctionnalités
* [UI] Avertir de la dépréciation de la création de luminosité de l’environnement

## Fixe :

* [Vue 2D] La sélection de l&#39;option « Afficher avec rapport physique » peut ne pas fonctionner lors de l&#39;utilisation de filtres de Substance
* [capture 3D] Les fichiers Svg sont répertoriés dans le sélecteur de fichiers, mais ne sont pas pris en charge
* [Vue 3D] Le paramètre d’intensité d’émission dans les paramètres du nuanceur ne fonctionne pas
* [Vue 3D] Parfois, la position du maillage est incorrecte lors de la création d’une ressource
* [Vue 3D] Le passage au rendu de traçage de chemin se bloque sur le matériel non pris en charge
* [Application] L’application se bloque lors de la fermeture de la fenêtre contextuelle de mesure manuelle sans définir de taille
* Blocage de [Application]
* [Application] Blocage sous Windows lors de l’affichage du bureau (touche Windows + raccourci clavier D)
* [Application] Blocage possible lors du changement de langue
* [Captis] Blocage lorsque les données d’aperçu ne sont pas valides
* [Captivate] Impossible d’effectuer un zoom arrière complet après un zoom avant
* [Captis] Localisation manquante sur certaines étapes de l&#39;Assistant
* [Captis] Blocage possible à la sortie lors de l’utilisation de Captis
* [Captivate] L’analyse ne fonctionne pas si des fichiers d’étalonnage sont manquants sur l’appareil
* [Filtres] L’aperçu du pinceau lors de l’utilisation du filtre Tampon de duplication peut être incorrect en fonction de la texture et de l’épaisseur du pinceau
* [Filtres] Taille de sortie incorrecte après l’utilisation du filtre Agrandissement
* [Filtres] Icônes manquantes pour les filtres Rotation de l’environnement et Stylisation
* [Filtres] La mise à jour de certains filtres peut entraîner un rendu incorrect
* [Calques] Premier rendu incorrect lors de la fusion de deux matériaux
* [Calques] Le bouton de mise à jour des calques affiche « Tout mettre à jour » même s’il n’y a qu’une seule mise à jour
* [Calques] Calculs inutiles lors de l’importation d’images dans la pile de calques
* [Performances] Amélioration de la gestion des formats de map normaux pour réduire les temps de rendu
* [Taille physique] La fenêtre contextuelle Mesure manuelle ne fonctionne qu’après une mesure automatique
* [Taille physique] Résolution d’exportation incorrecte dans la fenêtre contextuelle Exporter lorsque la Taille physique est activée
* [Actions rapides] Localisation manquante sur les noms d’actifs générés
* [UI] L’aperçu de la ressource au survol peut ne pas s’afficher
* [UI] Cliquer sur le bouton Rétablir la valeur par défaut peut rompre certains contrôles
* [UI] Les messages d’erreur ne sont pas effacés lors du changement de projet
* [UI] Vérifiez que le nom de la matière dans la clôture et le panneau Propriétés est vide lorsqu’il n’y a aucun actif.
* [UI] Le bouton Rétablir la valeur par défaut du paramètre Point de vue ne fonctionne pas
* [UI] Rétablir la valeur par défaut du chevauchement de boutons
* [UI] Certains boutons ne sont pas cliquables lorsqu’un panneau est désancré
* [UI] Paramètre V de remplissage de texture partiellement masqué dans les paramètres du visualiseur et la vue 3D

## Supprimé :

* [capture 3D] Supprimer la prise en charge de capture 3D
* [Application] Supprimer la prise en charge de macOS x86
