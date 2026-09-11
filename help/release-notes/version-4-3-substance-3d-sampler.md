---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/release-notes/version-4-3substance-3d-sampler.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Sampler version 4.3 pour en savoir plus sur les nouveaux générateurs de textures, le filtre de broderie et l’outil de recadrage de perspective.
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 4.3
user-guide-description: ''
user-guide-title: ''
source-git-commit: 6cc0519fb8c0f74fa805691ec4adb9e449a627d5
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 0%

---


# Version 4.3

<b>Substance 3D Sampler 4.3</b> introduit un nouveau contenu de démarrage, notamment des <b>générateurs de Textures</b>, une nouvelle version du filtre <b>Broderie</b> et un outil <b>Correction de perspective</b>.

*Date de publication : 25 janvier 2024*

## Un nouveau contenu pour les ressources de démarrage

![](../assets/NewStarterContent.png)

Les matériaux inclus dans Sampler ont été mis à jour pour mieux répondre aux besoins des workflows de <b>design industriel</b>, des workflows de <b>mode </b> et des artistes techniques travaillant dans les médias et le divertissement qui auront désormais plus de contrôle sur les aspects techniques de la création de textures.

## Générateur de texture

![](../assets/sa_whats-new-screen_v4-3-0_generators.png)

Les nouveaux générateurs de textures offrent un meilleur contrôle sur la création de matériaux à l&#39;aide de <b>bruits, motifs </b> et<b> options d&#39;usure/salissures</b> paramétriques.  Les images générées peuvent être utilisées dans des masques ou des couches colorées, ce qui facilite plus que jamais la collaboration entre les équipes techniques et créatives sur la conception de matériaux.

![](../assets/sampler4.3-texturegenerators-ezgif.com-video.gif)

Utilisez la nouvelle icône de filtrage pour analyser uniquement les générateurs de textures.

![](../assets/parse-texgen.gif)

## Broderie

![](../assets/Embroideryv3.png)

Le filtre Broderie mis à jour a une meilleure précision de couture et prend en charge jusqu’à 8 couleurs. Les entrées du matériau sont de retour dans la pile de calques ce qui permet l&#39;insertion d&#39;autres métaux dans la pastille.

## Correction de perspective par recadrage

![](../assets/PerspectiveCropTool.png)

Le nouvel outil Recadrage de Perspective vous permet de recadrer des matériaux déformés et de numériser avec quatre points de contrôle pour supprimer les artefacts de perspective et obtenir un élément regroupable.

![](../assets/sampler4.3-perspectivecrop-ezgif.com-video-gif.gif)

## Stylisation

![](../assets/03-8.png)

Le filtre Stylisation vous permet de styliser n’importe quel matériau pour obtenir un aspect pictural.

## Mode fusion dans le filtre Fond

![](../assets/Fill-Blend-mode.gif)

La mise à niveau du filtre Remplissage introduit des modes de Fusion, ce qui vous permet de multiplier la valeur, les maps d&#39;entrée ou les générateurs de texture du remplissage avec les résultats de couche des calques sous-jacents.

## Améliorations apportées au calque d’importation d’image

![](../assets/Import-Layer-improvements.gif)

Vous pouvez ajouter plusieurs images sur un calque d’image d’importation et générer une Map opacity à partir du Canal Alpha d’une image.

## Note de mise à jour

*(Publié Le 25 Janvier 2024)*

<b>Ajouté</b> :

* [Assets] Nouveau type d’actif : Générateurs de Textures
* [Fichiers] Nouveaux matériaux inclus dans les fichiers de démarrage
* [Ressources] Nouveau sélecteur de ressources pour les paramètres d’image dans le panneau Propriétés
* [Actifs] Glissez-déposez les générateurs de Textures du panneau Actifs vers les sélecteurs d’images du panneau Propriétés
* [Assets] Glissez-déposez les générateurs de Textures depuis l’explorateur de fichiers du système d’exploitation
* [Ressources] Les filtres peuvent suggérer d’adapter les générateurs via une balise utilisateur sur l’entrée d’image
* [Assets] Les générateurs de Textures peuvent définir quel filtre doit les suggérer via une balise utilisateur
* [Contenu] Nouveau filtre de recadrage de Perspective
* [Contenu] Nouveau filtre de stylisation
* [Contenu] Mode de fusion sur le filtre Fond
* [Contenu] Filtre Broderie mis à jour
* [Content] Filtre de renvoi à la ligne des Peintures mis à jour
* [Contenu] Mise à jour de tous les filtres pour prendre en charge les générateurs de Textures
* [Calques] Possibilité de choisir un canal de sortie du générateur de Textures lors de son ajout à la pile de calques
* [Calques] Possibilité de répertorier et d’appliquer facilement des paramètres prédéfinis sur les générateurs de Textures
* [Calques] Afficher un aperçu du générateur de Textures dans les sélecteurs d’images
* [Calques] Les paramètres du générateur de Textures peuvent être exposés et exportés.
* [Calques] Affectez l’utilisation de la Base color lors de l’importation d’une seule image avec le modèle de création Importation de Texture
* [Calques] Commentaires lors de la tentative de glisser-déposer de fichiers incompatibles dans les sélecteurs d’images du panneau Propriétés
* [Calques] Générer une couche d’opacité à partir du canal Alpha d’une image importée
* [Calques] Le calcul de l’image en Matériau (IA) est plus rapide lors du changement de catégorie
* [Calques] Sélectionnez le calque le plus pertinent après avoir utilisé un modèle de création
* [Calques] Les widgets de position peuvent désormais être modifiés à l’aide d’un curseur dans le groupe Paramètres avancés
* [Exporter] Afficher un pourcentage dans la file d’attente plutôt que des nombres bruts
* [Interopérabilité] Le canal d’opacité est désormais reconnu comme canal Alpha lors de l’envoi vers Painter
* [Application] Nouvelle boîte de dialogue pour afficher et enregistrer les informations sur le matériel
* [Application] Nouvelle préférence pour modifier l’échelle d’height par défaut pour chaque projet
* [Application] Amélioration de l’affichage des ressources obsolètes
* [Scripting] Nouvelles fonctions asset.documentResolution() et asset.setDocumentResolution()
* [Scripting] Nouvelle fonction select\_asset()
* [Scripting] API Python pour les générateurs de Textures
* [Scripting] get\_project\_assets() renvoie désormais les objets 3D
* [UI] La taille des vignettes des actifs peut être modifiée dans le panneau Actifs
* [UI] Mise à jour des icônes d&#39;affichage du viewport

<b>Fixe :</b>

* [vue 2D] Le zoom avec la molette de la souris est bloqué à 244 %.
* crash [Application] au démarrage lors de l’initialisation de l’API graphique
* crash [Application] si le nom du projet contient le caractère #
* [Application] crash possible lors de l’ouverture d’un ancien projet
* [Application] La réouverture du projet en cours peut entraîner un crash
* [Application] Certaines modifications apportées au projet ne sont pas enregistrées et sont perdues sans avertissement lors de la fermeture du projet si elles ne sont pas enregistrées
* [Export] Problèmes d’exportation .sbs/.sbsar lors de l’utilisation de plusieurs fichiers portant le même nom
* [Export] Espace colorimétrique incorrect pour les images en niveaux de gris exportées .sbs/.fichier sbsar
* [Filtres] Problèmes de comportement du mélange d’opacité
* [Calques] Parfois, les fichiers .svg ne sont pas rendus à la bonne résolution
* [Performances] Certaines sauvegardes de projet sur le disque ne sont pas nécessaires
* [Projet] L’importation d’un ancien projet ne charge pas les paramètres prédéfinis associés
* [Scripting] Impossible d’obtenir les paramètres du premier calque inséré
* [UI] La fenêtre contextuelle d’aperçu lors du survol d’une ressource peut apparaître au mauvais emplacement ou à un mauvais écran
* [UI] Les panneaux non ancrés sont visibles et utilisables en haut de l’écran de bienvenue
