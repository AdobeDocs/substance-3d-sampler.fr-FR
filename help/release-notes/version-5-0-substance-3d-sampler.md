---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/release-notes/version-5-0-substance-3d-sampler.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Sampler version 5.0 pour en savoir plus sur les nouveaux outils de numérisation, les fonctionnalités et les améliorations des workflows.
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 5.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---


# Version 5.0

![](../assets/welcome_digitization_tool.jpg)

<b>Substance 3D Sampler 5.0</b> introduit des moyens plus simples d&#39;accéder à Material Digital Twin avec des numérisations et des rendus de meilleure qualité.

Les principales nouveautés sont les suivantes :

## Actions rapides

Démarrez tous les principaux workflows de Sampler en un clic et préparez la pile de calques pour vous !

Plus d&#39;informations *[ici](../interface/panels/quick-actions-panel.md)*.

![](../assets/quick_actions_1440x810.png)

## Nouvelle disposition de l’écran d’accueil

Retrouvez tous vos projets, tutoriels et commencez votre travail directement à partir de la page d’accueil.

Plus d&#39;informations *[ici](../interface/the-home-screen.md)*.

![](../assets/new_home_screen_layout_1440x810.png)

## Nouveau moteur de rendu

Choisissez entre le temps réel et le traçage de chemin pour améliorer la cohérence visuelle et prendre en charge de nouvelles propriétés de matériau. Enregistrez des instantanés de votre travail directement depuis la vue 3D.

Plus d&#39;informations *[ici](../interface/2d-and-3d-viewport.md)*.

![](../assets/eclair_support_1440x810.png)

## Intégration de HP Z Captis

Avec HP Z Captis et Substance 3D Sampler, transposez des matériaux du monde réel au format numérique en quelques minutes.

Fonctionnalité disponible pour les comptes Entreprise, Équipes et Éducation.

Plus d&#39;informations *[ici](../pipeline-and-integrations/hp-z-captis-support/hp-z-captis-support.md)*.

![](../assets/hp_z_captis_1440x810.png)

## Notes de mise à jour V5.0

*(sortie : 20 février 2025)*

<b>Ajouté</b> :



* [Intégration] Nouvelle page d’accueil avec un accès rapide au contenu d’apprentissage, aux exemples de projet, aux actions rapides et aux projets récents.
* [Intégration] Démarrez rapidement avec les nouvelles actions rapides, accessibles depuis la page d’accueil et à partir du panneau dédié
* [Intégration] [Contenu] Les actions rapides sont des workflows prédéfinis qui remplissent la pile de calques avec la plupart des calques utilisés
* [Intégration] Possibilité de créer un nouveau projet via un nouveau menu Démarrage rapide, via des actions rapides ou un projet personnalisé
* [Intégration] Possibilité de créer un projet vide directement depuis la page d’accueil via un bouton dédié
* [Vue 3D] Nouveau pixelliseur et traceur de tracé avancés apportant de nouvelles fonctionnalités de rendu (propriétés telles que le revêtement, la brillance, la translucidité, la diffusion sous la surface) et une cohérence visuelle dans l’écosystème de Substance
* [Vue 3D] Les paramètres de la visionneuse sont désormais accessibles directement dans la vue 3D
* [Vue 3D] Possibilité d’enregistrer un instantané de rendu dans le Presse-papiers ou dans des fichiers
* [Vue 3D] Afficher une grille pour visualiser l’origine de la scène
* [Vue 3D] Activez le plan au sol pour capturer les ombres et les reflets
* [Vue 3D] Contrôlez le degré de réflexion et d’opacité de votre plan au sol
* [capture 3D] Positionner le filet sur le sol
* [Application] Vérifier la compatibilité matérielle au démarrage de l’application
* [Application] La fenêtre de rapport d’incident s’ouvre désormais juste après un blocage
* [Contenu] Ouvrez un exemple de projet pour commencer facilement
* [Export] Exporter le nuanceur de matériaux Adobe Standard dans des fichiers USD
* [IA générative] Cochez la case « Ne pas déduire » lors de l’utilisation d’une image comme entrée dans les workflows Image vers Texture.
* [Projet] Les vignettes sont stockées dans le fichier de projet pour une ouverture plus rapide des projets
* [Projet] Définition dans les préférences pour stocker les données de cache dans le fichier de projet, avec différents modes (pas de cache, cache léger, cache complet)
* [Scripts] [Rupture de changement] Migration de Qt vers Qt6.15 - Impact de la compatibilité des plug-ins existants
* [Scripts] Les plug-ins par défaut et le dossier de scripts se trouvent désormais dans le dossier Documents
* [Scripts] Nouvelle interface utilisateur pour les plug-ins pour une cohérence visuelle avec les panneaux principaux de Sampler
* [Scripts] Accédez à 2 exemples de plug-in pour découvrir les fonctionnalités du plug-in Sampler
* [Scripting] Nouvelle fonction open\_3d\_catpure()
* [Scripts] Lors de l’insertion d’un calque, indiquez s’il est inséré au-dessus ou au-dessous de la position cible

<b>Fixe :</b>

* [capture 3D] Blocage si la capture d’objet ne peut pas être démarrée sur macOS
* [Application] Blocage à la sortie
* [Application] Blocage à la fermeture lors de l’ajout d’actifs au panneau Projet
* [Application] Renommer un actif de projet ne fonctionne pas, sauf si vous appuyez sur Entrée
* [Application] Les entrées de menu Annuler et Rétablir ne sont pas désactivées alors qu’elles devraient l’être
* [Actifs] Impossible de supprimer les actifs de la section Toutes les bibliothèques du panneau Actifs
* [Contenu] Créateur d’atlas : utilisez la carte d’opacité existante, le cas échéant.
* [Contenu] Mélange d’ID de couleur : corrigez le choix des couleurs dans la couleur de base
* [Calques] Éviter les calculs inutiles lors de l’utilisation de générateurs
* [Calques] Le réglage d’un générateur peut entraîner le déclenchement d’un trop grand nombre d’ordinateurs
* [Performances] Améliorer la gestion de la mémoire GPU
* [Performance] Le cache de rendu ne peut pas être utilisé lors du redémarrage de l’application
* [Ressources] Les fichiers en lecture seule ne sont pas visibles dans le panneau Actifs
* [Scripts] Autoriser la réutilisation d’un calque après l’avoir ajouté un autre
* [Scripts] La modification de la structure de la pile de calques plusieurs fois dans un script peut échouer

<b>Supprimé(e) :</b>

* [Application] Suppression de la prise en charge des fichiers image .dng et .nef
