---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/release-notes/version-3-4.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Sampler version 3.4 pour en savoir plus sur les nouvelles fonctionnalités conçues pour améliorer la vitesse et la qualité des workflows 3D.
helpx_creative_field: ""
helpx_description: Sampler > Release Notes > Version 3.4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 3.4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---


# Version 3.4

**Substance 3D Sampler 3.4.0** introduit une série de nouvelles fonctionnalités conçues pour augmenter la vitesse et la qualité des workflows 3D.

*Date de publication : 6 septembre 2022*

## Principales fonctionnalités

## Paramètres exposés

Modifiez les matériaux paramétriques dans les logiciels prenant en charge les fichiers SBSAR, tels que CLO, UE5, Blender, Photoshop et Illustrator, entre autres.\
Cela est désormais possible grâce à la nouvelle capacité de Sampler à exposer les paramètres des actifs, ce qui vous permet d’accélérer les itérations et de vous débarrasser des va-et-vient entre Sampler et d’autres logiciels.

Exposez les paramètres de votre matériau en cliquant simplement sur une épingle.

Les points de couleur vous aideront à naviguer dans vos paramètres exposés et vos différents panneaux.

## Création Python

Vous pouvez désormais créer des plug-ins et des scripts. Cela vous permet de personnaliser votre interface, de faciliter l’intégration de Sampler dans votre pipeline et de configurer votre workflow global, comme vous le souhaitez.\
Cela pourrait vous permettre, par exemple, de créer un script vous permettant d&#39;automatiser les tâches répétitives comme l&#39;exportation de plusieurs matériaux en un clic.

Découvrez comment créer votre premier plug-in ou script [ici](../scripting-and-development/scripting-and-development.md).

## Propriétés physiques CLO

Vous pouvez maintenant créer des textiles qui se comportent de manière réaliste avec des simulations physiques. Pour ce faire, vous devez saisir les propriétés physiques du tissu, telles que la flexion, le cisaillement et le frottement.\
Avec cette mise à jour, le SBSAR contiendra les informations physiques dans ses métadonnées, qui sont utilisées par CLO pour s&#39;assurer que le matériau réagit de manière réaliste.

## Image vers matériau (optimisé par l’IA)

Image vers matériau (optimisé par l’IA) est désormais disponible sur MacOS et s’exécute en mode natif sur les appareils Apple Silicon.

## Notes de mise à jour

### 3.4.0 Arancini

*(Date de publication : 6 septembre 2022)*

**Ajouté :**

[Paramètres exposés] Nouveau Panneau Paramètres exposés\
[Paramètres exposés] Nouveau bouton au survol des paramètres pour exposer et exposer les paramètres du panneau Propriétés\
[Paramètres exposés] Nouveau menu contextuel par clic droit sur les paramètres pour exposer et exposer les paramètres à partir du panneau Propriétés\
[Paramètres exposés] Les paramètres exposés sont répertoriés dans le Panneau Paramètres exposés\
[Paramètres exposés] Des points et des disques de couleur sont ajoutés à plusieurs endroits pour identifier facilement les paramètres exposés\
[Paramètres exposés] Les étiquettes de paramètres peuvent être modifiées dans le Panneau Paramètres exposés\
[Paramètres exposés] Afficher un avertissement pour les paramètres non exportables\
[Paramètres exposés] Affiche un avertissement si vous déplacez un calque avec des paramètres de fusion exposés à un endroit où ils deviennent masqués\
[Paramètres exposés] Les paramètres exposés sont exportés aux formats SBS et SBSAR\
[Métadonnées] Prise en charge des modèles de métadonnées personnalisés\
[Métadonnées] Nouveau modèle de métadonnées de propriétés physiques CLO\
[Métadonnées] Ajoutez des icônes au survol pour ajouter/supprimer des métadonnées personnalisées\
[API Python] Nouvelle API Python\
[API Python] API pour la création de ressources\
[API Python] API pour la gestion des calques\
[API Python] API pour la gestion des paramètres\
[API Python] API pour la gestion de projets\
[API Python] Un plug-in peut être activé et désactivé\
[API Python] Documentation de l’API Python accessible dans le menu Aide\
[Scripts] Nouvelle section Plug-ins et scripts dans le menu contextuel Préférences\
[Scripts] Création et importation de plug-ins pour personnaliser l’interface de Sampler avec vos propres panneaux\
[Scripts] Les plug-ins font partie de l’interface de Sampler et peuvent être ancrés et déplacés comme les panneaux Sampler standard\
[Scripting] Barre de boutons dédiée aux plug-ins dans la barre d’outils de droite de Sampler\
[Scripts] Créez et importez des scripts pour exécuter une liste de tâches données\
[Scripts] Lancement de scripts Python via le menu Scripts\
[Scripts] Les plug-ins et les scripts peuvent être supprimés, réordonnés et rechargés à partir de la fenêtre Préférences\
[Scripting] Ajout de paramètres de ligne de commande —run-script\
[Journaux] Nouveau panneau Journaux\
[Journaux] Activer le panneau Journaux à partir de la fenêtre Préférences\
[Journaux] Nouvelle barre d’actions pour effacer, copier/coller et exporter les journaux\
[Propriétés] Nouveau bouton au survol des paramètres pour réinitialiser la valeur des paramètres\
[Propriétés] Nouveau menu contextuel par clic droit sur les paramètres pour réinitialiser la valeur du paramètre\
[Contenu] Image vers matériau (optimisé par l’IA) fonctionne désormais sur MacOS\
[Engine] Mettez à jour le moteur de Substance vers la version 8.6.0

**Fixe :**

[Application] L’application peut se bloquer à la fermeture lorsqu’une génération de vignette est en cours\
[Application] L’application peut se bloquer lors de l’utilisation de « Enregistrer sous » à la sortie\
[Application] L’application peut se bloquer lors de l’arrêt de MacOS\
[Application] L’enregistrement avec la boîte de dialogue Couleur ouverte n’enregistre pas ses modifications\
[Export] La convention de dénomination d&#39;utilisation est incorrecte lors de l&#39;exportation\
[Calques] Déposer un matériau sur un filtre peut provoquer un blocage\
[Calques] La mise à jour d’une pile de calques obsolète peut mettre à jour des piles de calques non associées\
[Métadonnées] Les champs vides sont exportés\
[Métadonnées] Lorsqu’il n’existe qu’un seul élément de métadonnées, l’interface utilisateur vous permet d’essayer de le réorganiser\
[Projet] Le calcul ne se termine jamais après la duplication d&#39;une matière\
[Projet] L’actif du projet est dupliqué après l’enregistrement initial du projet\
[Projet] Calculs inutiles lors du changement de ressource\
[Rendu] Certaines piles de calques ne s’affichent pas correctement après avoir supprimé un calque\
[Sécurité] Correctif CVE-2015-20107\
[UI] Les sorties 2D peuvent être floues selon la taille de la fenêtre\
[UI] L’aperçu des ressources peut rester ouvert en haut lorsque l’application perd le focus\
[UI] Les coins arrondis de l’écran de démarrage ont un arrière-plan carré opaque

**Problèmes connus :**

[Sélecteur de couleurs] Le choix d’une couleur sur un deuxième moniteur avec une résolution différente peut ne pas fonctionner\
[Contenu] Le widget Lumière de forme ne fonctionne pas en mode projection sphérique\
[Interopérabilité] Le matériel avec displacement envoyé à Stager perdra les contrôles de displacement
