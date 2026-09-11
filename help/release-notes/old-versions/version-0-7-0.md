---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/release-notes/old-versions/version-0-7-0.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Sampler version 0.7.0 pour en savoir plus sur les mises à jour, les améliorations et les correctifs de bogues.
helpx_creative_field: ""
helpx_description: Sampler > Release Notes > Old Versions > Version 0.7.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 0.7.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---


# Version 0.7.0

Date de publication : **2019/06/13**

Ajouté :

* [Filtres] Accédez rapidement à vos filtres en appuyant sur la barre d’espace
* [Filtres] Nouveau panneau dédié pour gérer, parcourir et importer vos filtres
* [Métadonnées] Cliquez avec le bouton droit de la souris sur un matériau pour afficher ses métadonnées
* [Métadonnées] Cliquez avec le bouton droit de la souris sur un matériau pour afficher son emplacement sur le disque
* [Curseurs] Animez les curseurs lorsque vous les survolez en appuyant sur Ctrl
* [Curseurs] Arrêtez et redémarrez l’animation de vos curseurs en appuyant sur P
* [Export] L&#39;exportation SBSAR suit les directives de Substance Source
* [Licence] Activer la Substance Alchemist à l’aide d’une variable d’environnement
* [UX] La boîte de dialogue Fichier mémorise le dernier chemin de fichier sélectionné
* [UX] La boîte de dialogue Dossier mémorise le dernier chemin de dossier sélectionné
* [UI] Interface utilisateur du panneau Ressources de mise à jour
* [UI] Mettre à jour l&#39;interface utilisateur de la barre de recherche
* [UI] L’icône Créer un nouveau matériau est mise à jour
* [Aide] Les URL sont mises à jour vers le domaine [substance3d.com](http://substance3d.com)
* [Maillage] Un maillage en tissu est maintenant disponible
* [Contenu] Nouveau filtre de corrosion
* [Contenu] Nouveau filtre d’oxydation
* [Contenu] Nouveau filtre de mousse
* [Contenu] Nouveau filtre de Dust
* [Contenu] Nouveau filtre de motif de mur de briques
* [Contenu] Nouveau filtre de motif de mur de pierre
* [Contenu] Nouveau filtre de finition du bois
* [Contenu] Nouveau filtre de finition métallique
* [Contenu] Nouveau filtre de Snow
* [Contenu] Nouveau filtre aléatoire
* [Contenu] Vous pouvez désormais importer vos textures directement dans le filtre de Matériau de base

Fixe :

* Corriger un crash lors de l’enregistrement de la pile de calques
* Possibilité d’ajouter une valeur supérieure à 1 dans le curseur de rotation de l’environnement
* Ne perdez pas les paramètres de fusion lorsqu’un calque de fusion est transformé d’avant en arrière d’un calque de fusion à un calque de matériau
* Correction des doublons lors de la génération de variations de la même pile de calques plusieurs fois
* Lors de la réouverture d’un matériau, Alchemist mémorise les plages modifiées (min et max) de vos curseurs

Problèmes connus :

* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Le basculement rapide de visibilité d’une scène Delighter n’est pas recommandé
* L’importation d’environnement personnalisée peut devenir noire
* Les images Tif ne s’affichent pas dans le panneau Propriétés du calque d’importation d’image
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Le filtre Normal à l’height peut effectuer un crash sur MacOS
