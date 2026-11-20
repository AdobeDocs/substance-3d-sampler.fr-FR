---
description: Consultez les notes de mise à jour de Substance 3D Sampler version 6.1 pour en savoir plus sur les nouvelles fonctionnalités, les améliorations et les améliorations de workflow.
title: Version 6.1
hold: true
source-git-commit: 99bb504f8dd5c485bf0d208a85cc3825d186c55f
workflow-type: tm+mt
source-wordcount: '1167'
ht-degree: 0%
---

# Version 6.1

**Kouign amann** (pâtisserie bretonne en couches)

![Texte optionnel](../../help/assets/Sampler_splash_large.jpg)

Cette version introduit le mode Performances, qui permet à chacun de désactiver des paramètres susceptibles de ralentir son workflow, ainsi que des améliorations automatiques de la stabilité, qui protègent les utilisateurs sur du matériel plus léger.

Les principales nouveautés sont les suivantes :

## Mode Performances

Bénéficiez d’une expérience plus rapide et plus réactive dans Sampler. Le nouveau **mode Performances** réunit tous les paramètres susceptibles de ralentir votre workflow : les limites de résolution, les ombres, la qualité du displacement et le traçage de chemin. Désactivez les fonctionnalités dont vous n’avez pas besoin pour améliorer les performances et la réactivité.

Plus d&#39;informations [*ici*](https://www.adobe.com/go/substance-3d-sampler-6.1-performance-mode_fr)

![](../assets/v6.1/6_1-Performance_Mode.png)

## Prise en charge améliorée des machines à spécifications minimales

Si votre matériel est inférieur à la [spécification minimale](../getting-started/system-requirements.md), Sampler s&#39;ajuste désormais automatiquement pour assurer la stabilité. Les fonctions les plus susceptibles de ralentir les choses ou de provoquer un crash sont automatiquement désactivées.

Plus d&#39;informations [*ici*](https://www.adobe.com/go/substance-3d-sampler-6.1-low-specs-mode_fr)

![](../assets/v6.1/6_1-Checked.png)

## Notes de mise à jour V6.1

*(sortie : 19 novembre 2026)*

## Ajouté

* &amp;lbrack ; Application&amp;rbrack ; Nouvelle façon de signaler les avertissements de configuration matérielle minimale requise
* &amp;lbrack ;Captis&amp;rbrack ; Ajouter une option pour choisir entre 4 et 8 angles de polarisation
* &amp;lbrack ; Captis&amp;rbrack ; Nouvelle action rapide Captis
* &amp;lbrack ;Export&amp;rbrack ; Signale correctement les échecs d&#39;exportation à l&#39;utilisateur
* &amp;lbrack ;Export&amp;rbrack ; Update Unreal Moteur 4 export preset (renommé Unreal Moteur 5)
* &amp;lbrack ; Performance&amp;rbrack ; La création de ressources à partir du fichier est désormais asynchrone
* &amp;lbrack ; Performance&amp;rbrack ; Déplacer la charge de travail du thread principal vers les threads de travail
* &amp;lbrack ; Performance&amp;rbrack ; Nouveau mode de performance
* &amp;lbrack ;Project&amp;rbrack ; Avertir l&#39;utilisateur si l&#39;enregistrement du projet échoue
* &amp;lbrack ; Scripting&amp;rbrack ; Nouvelle méthode generate_thumbnail pour les actifs et nouvelle propriété type pour les ressources
* &amp;lbrack ; Scripting&amp;rbrack ; Rendu d&#39;un instantané de vue 3D dans un fichier à partir du module Python
* &amp;lbrack ;UI&amp;rbrack ; Cliquer n&#39;importe où sur une zone de dépôt ouvre la boîte de dialogue du fichier
* &amp;lbrack ; UI&amp;rbrack ; Raccourcis de la barre de navigation de gauche vers les outils (égaliser, recadrer, répétition, transformer, réparer, couleur, ...)
* &amp;lbrack ; UI&amp;rbrack ; Mettez à niveau qt-spectrum pour obtenir les dernières icônes

## Fixe

* &amp;lbrack ; vue 3D&amp;rbrack ; Corriger immédiatement le Décalage des UV et la rotation, supprimer l&#39;échelle normale pour l&#39;OpenPBR
* &amp;lbrack ;vue 3D&amp;rbrack ; Empêcher un crash en s&#39;assurant qu&#39;aucune modification de scène ne se produit pendant la suppression du viewport
* &amp;lbrack ;vue 3D&amp;rbrack ; Supprimez correctement les informations de displacement (height) lors de la modification de l&#39;actif affiché
* &amp;lbrack ;vue 3D&amp;rbrack ; Mettre correctement à jour le document lors de la suppression du maillage
* &amp;lbrack ; Application&amp;rbrack ; Garantir que la surface reste active lors du calcul des informations de débogage du filtre dynamique
* &amp;lbrack ; Application&amp;rbrack ; Corriger le crash à la sortie de la Scène
* &amp;lbrack ;Application&amp;rbrack ; Corriger un crash potentiel lors de la suppression d&#39;un actif pendant l&#39;arrêt du service de base de données d&#39;actifs
* &amp;lbrack ;Application&amp;rbrack ; Sécuriser le thread des informations de débogage du cache pour empêcher un crash
* &amp;lbrack ;Application&amp;rbrack ; Empêcher un crash en testant que le nœud n&#39;est pas nul avant d&#39;y accéder
* &amp;lbrack ; Application&amp;rbrack ; Empêcher un crash causé par l&#39;accès au premier élément d&#39;un vecteur vide
* &amp;lbrack ;Application&amp;rbrack ; Empêcher un crash dans invalidateVisibleIfs
* &amp;lbrack ;Application&amp;rbrack ; Empêcher un crash lors de la création d&#39;actifs pendant l&#39;arrêt du service de base de données
* &amp;lbrack ; Application&amp;rbrack ; Empêcher la condition de course à la sortie
* &amp;lbrack ; Assets&amp;rbrack ; Assurez-vous que les ressources sont correctement sécurisées derrière le bon verrou
* &amp;lbrack ; Captis&amp;rbrack ; Bogue avec valeur d&#39;intensité en mode manuel
* &amp;lbrack ; Captis&amp;rbrack ; Empêcher l&#39;utilisateur de sélectionner une zone plus grande que celle autorisée par le back-end
* &amp;lbrack ; Channel Settings&amp;rbrack ; Double occurrence de SpecularColor dans ASM
* &amp;lbrack ; Channel Settings&amp;rbrack ; Corriger l&#39;identifiant d&#39;une utilisation créée à partir d&#39;une chaîne
* &amp;lbrack ; Content&amp;rbrack ; problème d&#39;opacité d&#39;Atlas scatter
* &amp;lbrack ;Content&amp;rbrack ; Le filtre Broderie n&#39;a pas de fonction métallique
* &amp;lbrack ; Content&amp;rbrack ; Réparer le filtre de perforation
* &amp;lbrack ; Content&amp;rbrack ; Correction de la catégorie du filtre de stylisation et de quelques correctifs dans le panneau Ressources
* &amp;lbrack ; Content&amp;rbrack ; Update Fill filter
* &amp;lbrack ;Creative Cloud&amp;rbrack ; Correction du chemin d’accès aux ressources 3D dans Creative Cloud
* &amp;lbrack ; Moteur&amp;rbrack ; Empêcher un crash lors de l&#39;accès aux données de moteur lorsque la tâche a été annulée
* &amp;lbrack ; Export&amp;rbrack ; Add defensive code to check structure&#39;s tree is not null
* &amp;lbrack ;Export&amp;rbrack ; Code défensif pour éviter les crashs dans la génération SBS
* &amp;lbrack ; Export&amp;rbrack ; Active la génération d&#39;utilisations personnalisées, même si elles sont connues par le moteur
* &amp;lbrack ; Export&amp;rbrack ; Fix export presets
* Les Maps normal &amp;lbrack ; Export&amp;rbrack ; sont exportées brutes dans USD
* &amp;lbrack ; Export&amp;rbrack ; Utiliser des libellés de sortie au lieu d&#39;utilisations lors de l&#39;exportation avec un paramètre prédéfini
* &amp;lbrack ; Paramètres exposés&amp;rbrack ; Corriger les paramètres exposés des filtres dynamiques
* &amp;lbrack ; Paramètres exposés&amp;rbrack ; Correction de la mise à jour de paramètre exposé lorsque son nom change
* &amp;lbrack ; Filters&amp;rbrack ; S’assurer que les identifiants de réglage des filtres dynamiques sont identiques entre chaque exécution sur chaque plate-forme
* &amp;lbrack ; Filters&amp;rbrack ; Masquer les utilisations non prises en charge dans la sélection de mappage de mosaïque automatique
* &amp;lbrack ; Layers&amp;rbrack ; La modification de la visibilité des calques recrée toujours des structures
* &amp;lbrack ; Layers&amp;rbrack ; Crash lors de l&#39;aplatissement d&#39;un tampon de Clone sur quelque chose
* &amp;lbrack ; Layers&amp;rbrack ; L&#39;insertion d&#39;un générateur directement sur la pile définit désormais correctement les réglages et le nom du nœud
* &amp;lbrack ; Layers&amp;rbrack ; L&#39;insertion d&#39;un générateur avec Remplir correctement affiche la texture dans le sélecteur
* &amp;lbrack ; Localization&amp;rbrack ; Fix Chinese charset compliance to GB18030
* &amp;lbrack ;Project&amp;rbrack ; Crash lors de l&#39;enregistrement après avoir peint sur un tampon de Clone
* &amp;lbrack ;Project&amp;rbrack ; Vérifiez que les noms de session et de projet sont réellement enregistrés
* &amp;lbrack ;Project&amp;rbrack ; Empêcher un crash lors de l&#39;enregistrement d&#39;un arbre
* &amp;lbrack ;Project&amp;rbrack ; La restauration d&#39;un projet corrompu à partir de la base de données est de retour
* &amp;lbrack ; Actions rapides&amp;rbrack ; Affiche la fenêtre contextuelle de sélection d&#39;image lorsqu&#39;il n&#39;y a aucune image dans la pile
* &amp;lbrack ; Actions rapides&amp;rbrack ; Résoudre les problèmes d&#39;actions rapides ; l&#39;annulation d&#39;une action rapide ne ferme plus le démarrage rapide
* &amp;lbrack ;Quick Actions&amp;rbrack ; Import textures asks pour activer certains canaux et ne doit pas
* &amp;lbrack ; Actions rapides&amp;rbrack ; Empêcher un crash si une action rapide ne parvient pas à se charger
* &amp;lbrack ; Quick Actions&amp;rbrack ; Update quick actions content
* &amp;lbrack ; Rendering&amp;rbrack ; Fix combineNormalAndHeight pour les matériaux ASM
* &amp;lbrack ; Rendu&amp;rbrack ; Correction des utilisations des textures affichables avec Vulkan
* &amp;lbrack ; Rendu&amp;rbrack ; Marquer l&#39;arbre comme sale lorsque la sortie d&#39;utilisation unique a changé
* &amp;lbrack ;Rendering&amp;rbrack ; Utilisez la structure de référence appropriée pour calculer les nœuds de l&#39;arborescence
* &amp;lbrack ; Scripting&amp;rbrack ; Ne pas bloquer si un problème se produit lors d&#39;une exportation
* &amp;lbrack ; Scripting&amp;rbrack ; Sure import_images() renvoie le calque importé
* &amp;lbrack ; Scripting&amp;rbrack ; La définition d&#39;une retouche d&#39;image sur une référence de ressource d&#39;image échoue
* &amp;lbrack ; Scripting&amp;rbrack ; get_filters() ne renvoie pas de filtres dynamiques
* &amp;lbrack ; Thumbnail&amp;rbrack ; Corrige les crashs potentiels lors de la génération de la vignette
* &amp;lbrack ; Thumbnail&amp;rbrack ; Recréez le générateur de vignettes lorsque la mise en page change
* &amp;lbrack ; UI&amp;rbrack ; La modification de l&#39;actif peut définir l&#39;échelle d&#39;height sur la valeur maximale du curseur
* &amp;lbrack ;UI&amp;rbrack ; Le dessin dans une texture met à jour le sélecteur de textures en temps réel
* &amp;lbrack ;UI&amp;rbrack ; L&#39;entrée en mode plein écran sans agrandissement remplit désormais toute la fenêtre
* &amp;lbrack ; UI&amp;rbrack ; Réparer le lien rompu vers le magazine Substance
* &amp;lbrack ; UI&amp;rbrack ; Corriger les marges contextuelles d&#39;exportation
* &amp;lbrack ; UI&amp;rbrack ; Correction de la taille du titre de section
* &amp;lbrack ; UI&amp;rbrack ; Corriger la faute de frappe dans une chaîne
* La boîte de dialogue du fichier &amp;lbrack ; UI&amp;rbrack ; Linux utilise désormais le plug-in GTK
* &amp;lbrack ;UI&amp;rbrack ; Empêcher le crash lors de l’affichage d’un émoji
* &amp;lbrack ;UI&amp;rbrack ; Renommer les fichiers .ssa comme « archive Adobe Substance 3D Sampler » (sans version ni Beta)
* &amp;lbrack ; UI&amp;rbrack ; Restaurer la décélération cliquable lors de l&#39;utilisation de la souris
* &amp;lbrack ; UI&amp;rbrack ; Petits correctifs dans la boîte de dialogue « Créer un nouveau matériau »
