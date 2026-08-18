---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/release-notes/version-4-2.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Sampler version 4.2 pour en savoir plus sur Image vers matériau, la fonctionnalité AI Upscale et les commandes de résolution optimisées par l’IA.
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 4.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---


# Version 4.2

<b>Substance 3D Sampler 4.2</b> introduit une nouvelle version optimisée par l&#39;IA de <b>Image vers matériau</b> et une nouvelle fonctionnalité d&#39;<b>optimisation de l&#39;IA</b>. Cette version inclut un contrôle complet de la résolution par calque.

*Date de publication : 05 septembre 2023*

## Image vers matériau - Nouvelle version

![](../assets/sa_whats-new-screen_v4-2-0_image_to_material.png)

Image en matériau génère des couches de matériau (couleur de base, rugosité, normale, displacement et métallique) pour vous à partir d’une seule image.

La version mise à jour de Image vers matériau améliore la génération de matériau et la gamme de matériaux pris en charge.

Désormais, Image vers matériau a été formé sur tous les types de matériau, générant de meilleurs résultats pour le tissu, le plastique, le bois, etc.

La version mise à jour comporte un nouveau paramètre permettant de sélectionner le type de matériau pour générer avec précision tous les canaux et ajuster automatiquement la plage.

![Substance 3D Sampler à l’aide du nouveau filtre Image vers matériau (optimisé par l’IA)](../assets/Materia_ScreenShot.png "Image vers matériau - Nouvelle version")

## AI Upscale

![](../assets/F5W_vAHaYAQLsz7.jpg)

Grâce au nouveau calque Upscale, Sampler améliore les fonctionnalités de votre matériau ou image en multipliant par 2 ou par 4 la résolution de votre ressource (matériau ou image).

Cela permet d’augmenter la qualité et le niveau de détail des textures basse résolution tout en préservant la cohérence des caractéristiques entre les cartes lors de l’agrandissement des textures.

Le filtre Amélioration améliore la couleur de base, la normale, l’height, la rugosité et les couches métalliques de votre matériau.

Pour optimiser la qualité des résultats, le filtre Agrandissement doit être utilisé sur les données (matériau et image) à leur résolution d’origine, sans modification de la résolution précédente.

![Filtre d’agrandissement ajouté au projet Substance 3D Sampler](../assets/Upscale_Highlighted.png "Filtre d’agrandissement")

## Résolution de calque

![](../assets/sa_whats-new-screen_v4-2-0_layer-resolution.png)

Le nouveau système de résolution de calque vous permet de contrôler entièrement la résolution de chaque calque. Un calque adopte la résolution de la taille de votre document ou les résolutions du calque en dessous.

La résolution est affichée sur chaque calque pour visualiser facilement l’impact de votre travail sur la résolution de votre matériau.

Cela vous permet d’améliorer la qualité de vos matériaux, mais aussi les performances lorsque vous travaillez sur vos ressources.

## Tutoriels

## Note de mise à jour

<b>4.2 DORAYAKI</b>

*(Publié Le 5 Septembre 2023)*

<b>Ajouté</b> :

* [Contenu] Filtres Image vers matériau (IA) et Delighter considérablement améliorés
* [Contenu] Nouveau filtre d’agrandissement
* [Contenu] Le filtre Recadrage a désormais une résolution de sortie dynamique.
* [Modèle de création de matériau] Paramètre Ajouter la taille du document.
* [Modèle de création de matériau] Nouveau bouton bascule « Ajouter un recadrage ».
* [Modèle de création de matériau] Nouveau bouton à bascule « Matériau supérieur »
* [Modèle de création de matériau] Afficher la taille de l&#39;image importée
* [Modèle de création de matériau] Donner son avis lorsque certaines images importées ne peuvent pas être utilisées
* [Modèle de création de matériau] Avertir lorsque les tailles d&#39;image sont incohérentes
* [Modèle de création de matériau] Nouveaux avertissements et info-bulles
* [Calques] Affiche la résolution des calques dans la pile de calques
* [Calques] La résolution de calcul des calques peut désormais être définie sur Taille du document ou Taille d’entrée.
* [Calques] Afficher la résolution des calques dans la pile de calques
* [Calques] Basculer une stratégie de résolution de calque vers Document ou Entrée de calque le cas échéant
* [Calques] Avertissez l’utilisateur lorsqu’un filtre Mise à l’échelle est ajouté manuellement et fournissez de la documentation
* [Calques] Avertissez l’utilisateur lors d’une mise à l’échelle linéaire et proposez d’utiliser le filtre Mise à l’échelle à la place
* [Calques] Le calcul d’un calque Image vers matériau (AI) peut désormais être annulé plus rapidement, pour améliorer les temps de rendu lors de l’ajustement de la pile de calques
* [Calques] Le calcul d’un calque Upscale peut désormais être annulé plus rapidement, pour améliorer les temps de rendu lors de l’ajustement de la pile de calques
* [Export] Autoriser la résolution de remplacement des textures exportées
* [Exporter] Les canaux à exporter sont maintenant triés
* [Exporter] Afficher la résolution de canal dans la liste des canaux à exporter
* [Application] Nouvelle préférence pour activer ou désactiver les réseaux neuronaux à accélération GPU
* [UI] Amélioration des listes déroulantes de résolution
* [UI] Nouvelles icônes pour les filtres Transformation de maillage, Post-traitement de maillage et Tissage
* [UI] Renommez le panneau « Partager » en « Exporter ».
* [Scripts] Ajout de la prise en charge de la résolution de sortie des calques à l’API d’exportation
* [Scripting] Ajout de la taille Recadrer, Agrandir et Document à l’API d’importation d’images
* [Intégration] Nouveaux tutoriels
* [Intégration] Mise à jour du contenu des écrans Bienvenue et Nouveautés
* [Engine] Mettez à jour la Substance Engine vers la version 9.0.1

<b>Fixe :</b>

* [capture 3D] Amélioration de la précision du nommage des options dans les paramètres d’alignement
* [Application] L’importation d’images avec un nombre non multiple de 16 dimensions peut entraîner un blocage
* [Application] Blocage lors de la duplication d’une ressource dans le panneau Projet
* [Application] Blocage lors du basculement d’actifs dans le panneau Projet
* [Contenu] La peinture d’un masque personnalisé pour le filtre Snow ne fonctionne pas correctement
* [Paramètres exposés] Les modifications des paramètres exposés peuvent être perdues lors de la permutation de matériaux
* [Interopérabilité] L’envoi d’un matériau à partir du panneau Exportation peut entraîner un blocage
* [Calques] Le remplissage d’après le contenu arrête le calcul lors du passage d’une entrée d’image unique à une entrée de matière
* [Calques] Blocage après la duplication d’une luminosité de l’environnement contenant un matériau
* [Calques] Le calque d’importation d’image affiche un nom d’image incorrect dans le panneau Propriétés si le fichier image a été renommé
* [Calques] Parfois, une double flèche s’affiche sur un calque inactif
* [Calques] Parfois, la modification de l’utilisation de la sortie d’une image dans un calque d’importation d’image ne fonctionne pas
* [Calques] Frappes dans la fenêtre Modèle de création
* [UI] L’info-bulle d’intégration de la fenêtre 3D présente des problèmes de focus
* [UI] Le nom de l&#39;image peut déborder si le nom du fichier est trop long
* [UI] Problèmes mineurs de disposition de la barre d’outils Pinceau lors de l’utilisation de la gomme
* [UI] Les chaînes sont tronquées dans certaines langues dans le panneau Paramètres du visualiseur
* [UI] Lorsque la fenêtre contextuelle de l’info-bulle de la fenêtre d’affichage est affichée, appuyer sur « space » crée un nouveau projet
