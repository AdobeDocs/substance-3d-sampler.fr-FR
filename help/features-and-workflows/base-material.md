---
breadcrumb-title: ''
description: Découvrez comment utiliser le Matériau de base dans Sampler, un excellent point de départ pour une édition efficace des matériaux.
title: Utiliser comme bitmap
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0f989901713dd30f8f936de2445caf5dc70a9225
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 4%

---


# Matériau de base

Le **Matériau de base** est un calque de matériau de base conçu pour vous offrir un point de départ rapide et flexible lors de la création de matériaux dans Sampler. Il expose un ensemble complet de paramètres qui s&#39;adaptent automatiquement au **modèle de matériau** utilisé par votre matériau (OpenPBR ou ASM), ce qui vous permet de construire n&#39;importe quoi, des surfaces simples aux matériaux complexes et physiquement riches.
Que vous partiez d&#39;un paramètre prédéfini ou que vous fabriquiez un matériau à partir de zéro, le Matériau de base vous assure de toujours partir d&#39;une **base claire, prévisible et modifiable**.

## Sensibilisation aux modèles de matériau (ASM OpenPBR)

Le Matériau de base est **sensible au modèle de matériau**.
Cela signifie que ses propriétés disponibles et ses valeurs par défaut changent selon que votre matériau est créé à l&#39;aide de :

* OpenPBR
* ASM (Adobe Standard Material)

Bien que les deux versions aient le même objectif, elles exposent **différents groupes de paramètres et comportements**, correspondant au modèle de matériau sous-jacent :

### OpenPBR

Les groupes de paramètres comprennent :

* Base
* Spéculaire
* Transmission
* Subsurface
* Revêtement
* Fibres
* Émission
* Film mince
* Géométrie
* Divers

Ces paramètres s’alignent sur la représentation physique unifiée de l’OpenPBR et sont conçus pour une interopérabilité dans l’ensemble de l’écosystème 3D.

### MATÉRIAU DE BASE ASM

Les groupes de paramètres comprennent :

* Surface
* Absorption
* Graphique de dispersion
* Translucidité
* Revêtement
* Éclat
* Émission
* Géométrie

Cette disposition reflète le modèle d’ombrage ASM et assure la continuité avec les workflows ASM existants.

>[!NOTE]
>
>Le Matériau de base s&#39;adapte toujours au modèle de matériau du matériau sur lequel il est appliqué. Un Matériau de base appliqué à un matériau OpenPBR n&#39;exposera pas les paramètres ASM, et vice versa.

## Valeurs uniformes et mappages personnalisés

Pour chaque paramètre exposé, le Matériau de base propose deux méthodes de travail :

### Valeurs uniformes (par défaut)

Par défaut, les paramètres utilisent des valeurs uniformes (curseurs ou sélecteurs de couleurs).
Cela vous permet de définir rapidement l’aspect global de votre matière sans aucune entrée de texture.

Des valeurs uniformes sont idéales pour :

* Blocage des matériaux
* Création de surfaces propres et simples
* Définition d’un point de départ visuel

### Mappages personnalisés

Si vous disposez déjà de cartes de texture, vous pouvez **remplacer n&#39;importe quelle valeur uniforme** en activant son **entrée de carte personnalisée**.

* Activer/désactiver l&#39;option de mappage personnalisé pour le paramètre
* Branchez votre texture existante
* La carte remplace complètement la valeur uniforme

## Préréglages

Le Matériau de base comprend un ensemble de **paramètres prédéfinis**, visibles sous forme de vignettes en haut du panneau Propriétés.
Les paramètres prédéfinis fournissent :

* Valeurs de Matériau de base préconfigurées
* Un moyen rapide de commencer à partir d&#39;une configuration visuellement significative
* Points de départ lisibles et cohérents pour les types de surface courants

La sélection d’un paramètre prédéfini ne verrouille pas le matériau. Tous les paramètres restent entièrement modifiables.

## « Appliquer des valeurs prédéfinies » lors de la création d’un matériau

Lors de la création d’une matière, vous pouvez choisir d’appliquer des valeurs prédéfinies à partir du panneau Créer une matière.
Ce que cela fait

* Remplace les valeurs par défaut du Matériau de base par les valeurs représentées par la vignette du paramètre prédéfini sélectionné
* Vous offre un point de départ visuel immédiat, au lieu des valeurs par défaut neutres
* Permet de réduire l’effet de « page vierge » au début d’un nouveau matériau

Ce qu&#39;il ne fait pas

* Il n’ancre ni ne fige les valeurs
* Cela n’empêche pas d’autres modifications
* Elle n’ajoute pas automatiquement de textures

On peut y voir le choix du point de départ, et non une limitation de l&#39;endroit où l&#39;on peut aller.

## Activation Des Canaux : Une Étape Critique

Pour qu&#39;un paramètre de Matériau de base ait un effet visible, la couche correspondante doit être activée dans les paramètres de couche de votre matériau.

### Meilleures pratiques

Avant de modifier un paramètre, vérifiez que son canal est activé
Activez uniquement les canaux dont vous avez besoin pour que votre matériau reste propre et efficace