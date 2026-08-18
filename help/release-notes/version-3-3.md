---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/release-notes/version-3-3.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Sampler version 3.3 pour en savoir plus sur les nouveaux outils, le contenu et les fonctionnalités de création de matériel.
helpx_creative_field: ""
helpx_description: Sampler > Release Notes > Version 3.3
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 3.3
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '1108'
ht-degree: 0%

---


# Version 3.3

**Substance 3D Sampler 3.3.0** introduit une série de nouveaux outils, contenus et fonctionnalités permettant de créer et de modifier plus facilement des matériaux et des éclairages de l&#39;environnement.

*Date de publication : 17 mai 2022*

## Principales fonctionnalités

## Remplissage d’après le contenu

L’outil Remplissage d’après le contenu est une technologie répandue dans Adobe Photoshop. Elle permet de supprimer les détails d’une image tout en préservant l’intégrité de la zone environnante.

Substance 3D Sampler utilise désormais la même technologie, ce qui vous permet de nettoyer les matériaux PBR et les éclairages de l’environnement. Sur les matériaux PBR, le remplissage d’après le contenu est appliqué sur tous les canaux. Il n’est pas nécessaire de traiter chaque canal séparément.

L’outil Remplissage d’après le contenu peut aider à supprimer les éléments de grande taille afin d’éviter les répétitions lors du mosaïque d’un matériau ou les petites imperfections sur votre tissu numérisé.

Lorsque vous capturez des panoramas à 360 degrés, il se peut que vous n’ayez pas le contrôle de tous les éléments de la scène. Par conséquent, vous devez supprimer de petits objets sur le sol, des peintures sur un mur ou une personne debout en arrière-plan. L’outil Remplissage d’après le contenu simplifie désormais les choses.

## Création IBL

### Projection sphérique

La modification des éclairages de l’environnement et des images 360 peut s’avérer difficile lorsqu’ils sont affichés sous forme d’images normales. Tous les éléments sont déformés, ce qui les rend presque impossibles à modifier. Avec la nouvelle projection sphérique, vous pouvez naviguer à 360° et effectuer des modifications avec des outils dédiés tels que Nadir patch, Remplissage d’après le contenu et tous les éclairages procéduraux sans distorsion. Il est désormais plus facile, par exemple, de modifier ou de nettoyer les lignes droites, de retirer le trépied de l’appareil photo et de placer parfaitement les éclairages des lignes.

Consultez le nouveau tutoriel pour [créer des éclairages de l&#39;environnement](https://www.youtube.com/watch?v=cfW9IyoTXQ8) à l&#39;aide de ce nouveau mode.

### Curseur d’exposition

Dans la vue 2D, vous pouvez modifier temporairement l’exposition pour mieux voir les détails ou les objets des parties sous-exposées ou surexposées de l’environnement que vous modifiez.

### Paramètres de la visionneuse dédiée

Les paramètres du visualiseur sont persistants par type de ressource (matériau ou éclairage de l’environnement). Vous pouvez définir le maillage, les textures par défaut ou le champ de vision de la caméra pour chaque type de ressource afin de faciliter le basculement entre eux pour fonctionner dans le bon contexte.

## Widgets améliorés

### Tampon de duplication

Avec cette mise à jour Tampon de duplication, vous pouvez peindre plusieurs contours de tampon avec différentes sources dans un seul calque et accéder à l’historique des tampons dans la pile de calques. En outre, vous pouvez désormais voir le résultat du tampon directement dans l’aperçu du pinceau avant de peindre. Cela facilite le nettoyage des matériaux et évite beaucoup de va-et-vient entre les vues.

### Recadrage et transformation

Cette mise à jour introduit de nouveaux raccourcis pour la manipulation des widgets Recadrer et Transformer.

### Barre d’outils Pinceau

La nouvelle interface utilisateur, similaire aux produits Adobes les plus récents tels que Fresco, vous permet de déplacer la barre d’outils n’importe où dans la vue 2D, affichée verticalement ou horizontalement. Lorsque vous peignez, passez du pinceau à la gomme avec la touche E et utilisez les nouvelles options de mosaïque pour mieux contrôler ce que vous peignez.

## Image vers matériau (optimisé par l’IA)

### Conserver la mosaïque

Image vers matériau (optimisé par l’IA) bénéficie d’une nouvelle option : elle permet désormais de préserver la mosaïque de votre image en mosaïque, ce qui réduit le temps nécessaire pour ajouter une mosaïque au matériau par la suite.

## Interopérabilité

Envoi de matériaux à Stager

Il était déjà possible d’envoyer des éclairages d’environnement à Stager. Vous pouvez désormais envoyer vos matières vers Stager en un clic, comme vous le feriez avec Designer et Painter. Grâce à cette fonctionnalité, vous n’avez plus besoin de publier vos matériaux et de les charger dans Stager en tant que fichiers individuels (nécessite Stager version 1.2.0 avec le nouveau gestionnaire de matériaux).

## Notes de mise à jour

### 3.3.0 Courgettes

*(Publié Le 17 Mai 2022)*

**Ajouté :**

* [Contenu] Nouveau filtre Remplissage d’après le contenu (Windows et Mac)
* [Contenu] L’outil Remplissage d’après le contenu fonctionne sur les images, les matériaux PBR et les éclairages de l’environnement
* [Contenu] Ajout du paramètre « Conserver les limites » à Image vers matériau (optimisé par l’IA)
* [Contenu] Le filtre Transformation de perspective peut afficher une grille entre ses quatre points
* [Interopérabilité] Envoi de matériel à Adobe Substance 3D Stager
* [Outils] Centrez la transformation en appuyant sur Ctrl lors du redimensionnement de l’outil Transformation ou Recadrage
* [Outils] Verrouillez le rapport L/H en appuyant sur Maj lors du redimensionnement de l’outil Transformation ou Recadrage
* [Outils] Le curseur de tampon de duplication offre un aperçu de ce qui sera tamponné
* [Outils] Affichez l’aperçu du contenu d’origine dans le curseur Gomme lors de l’utilisation du tampon de duplication
* [Outils] La touche Ctrl + Clic crée un nouveau tampon dans le calque Tampon de duplication
* [Outils] Les tampons dupliqués successifs sont désormais regroupés dans un seul calque
* [Outils] Réorganisation de l’interface utilisateur de la barre d’outils Pinceau
* [Outils] La position de la barre d’outils Pinceau est persistante pendant une session
* [Outils] Nouvelles options de mosaïque de pinceaux par axe
* [Outils] Masquer/afficher l’incrustation sur la vue 2D lors de la peinture
* [Outils] Nouveau raccourci, touche X, pour basculer entre les outils Pinceau et Gomme
* [Outils] Nouveau raccourci : « [ » « ] » pour modifier l’épaisseur du pinceau
* [Outils] Nouveau raccourci, touche « E », pour activer/désactiver la Gomme
* [Vue 2D] Nouveau mode de Projection sphérique lors de la création de l’éclairage de l’environnement
* [Vue 2D] L’outil Pinceau est pris en charge avec le mode projection sphérique
* [Vue 2D] L’outil Position est pris en charge avec le mode projection sphérique
* [Vue 2D] La fonction Annuler/Rétablir est prise en charge avec le mode projection sphérique
* [Vue 2D] En Projection sphérique, définissez la position par défaut pour regarder le centre de l&#39;environnement
* [Vue 2D] Nouveau contrôle d&#39;exposition
* [UI] Dans le panneau Propriétés, l’ajustement de l’image affiche la source du contenu (Image ou depuis un calque)
* [UI] Amélioration de l’arrière-plan déroulant des sorties de calque/matériau
* [UI] Nouvelle position des informations de résolution dans la vue 2D
* [UI] Nouvelle info-bulle avec raccourcis des commandes de navigation de la vue 3D
* [UI] Nouvelle info-bulle avec options de pinceau
* [UI] Nouvelle info-bulle avec raccourcis des commandes de navigation de projection
* [Filtres composés] Les filtres composés gèrent les variations qui fonctionnent sur les images, les matériaux PBR et les éclairages de l’environnement
* [Filtres composés] L’ordre des ajustements correspond à l’ordre de liste des nœuds dans le filtre composé
* [Filtres composés] Les modifications de différents nœuds avec le même groupe seront fusionnées dans un seul groupe dans le panneau Propriétés
* [Application] Disposer de paramètres de visionneuse dédiés par type de ressource

**Fixe :**

* [Application] L’application peut se bloquer lors du passage à la vue 2D
* [Application] Correction d’un blocage possible lors de l’exportation multiple
* [Application] Homogénéisation des valeurs par défaut des couches avec Substance 3D Designer
* [Application] Le chargement d’un projet ne déclenche pas le recalcul de la matière
* [Application] Mise à jour de l’URL de la documentation d’importation de textures
* [Contenu] Lors de l’utilisation d’un filtre composé, il demande à être mis à jour lorsqu’il ne le devrait pas, lors du rechargement
* [Contenu] Les détails de la carte d’height disparaissent lors de l’utilisation du mélange d’opacité
* [UI] Dans la boîte de dialogue Couleur, il est possible de sortir de la plage en utilisant les champs de texte du curseur
* [UI] La liste d&#39;utilisation a une barre de défilement verticale inutile

**Problèmes Connus :**

* [Sélecteur de couleurs] Le choix d’une couleur sur un deuxième moniteur avec une résolution différente peut ne pas fonctionner
* [Contenu] Le widget Lumière de forme ne fonctionne pas en mode projection sphérique
* [Interopérabilité] Le matériel avec displacement envoyé à Stager perdra les contrôles de displacement
