---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/release-notes/version-4-3substance-3d-sampler.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Sampler version 4.3 pour en savoir plus sur les nouveaux générateurs de texture, le filtre de broderie et l’outil de recadrage de perspective.
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

<b>Substance 3D Sampler 4.3</b> introduit un nouveau contenu de démarrage, notamment des <b>générateurs de texture</b>, une nouvelle version du filtre <b>Broderie</b> et un outil <b>Correction de perspective</b>.

*Date de publication : 25 janvier 2024*

## Un nouveau contenu pour les ressources de démarrage

![](../assets/NewStarterContent.png)

Les matériaux inclus dans Sampler ont été mis à jour pour mieux répondre aux besoins des workflows de <b>design industriel</b>, des <b>workflows de </b> mode et des artistes techniques travaillant dans les médias et le divertissement auront désormais plus de contrôle sur les aspects techniques de la création de textures.

## Générateur de texture

![](../assets/sa_whats-new-screen_v4-3-0_generators.png)

Les nouveaux générateurs de textures offrent un meilleur contrôle sur la création de matériaux à l&#39;aide des options <b>bruits, motifs </b> et<b> usure/salissures</b> paramétriques.  Les images générées peuvent être utilisées dans des masques ou des couches colorées, ce qui facilite plus que jamais la collaboration entre les équipes techniques et créatives sur la conception de matériaux.

![](../assets/sampler4.3-texturegenerators-ezgif.com-video.gif)

Utilisez la nouvelle icône de filtrage pour analyser uniquement les générateurs de textures.

![](../assets/parse-texgen.gif)

## Broderie

![](../assets/Embroideryv3.png)

Le filtre Broderie mis à jour a une meilleure précision de couture et prend en charge jusqu’à 8 couleurs. Les entrées du matériau sont de retour dans l&#39;empilement de couches, ce qui permet l&#39;insertion d&#39;autres métaux dans la pastille.

## Correction de perspective par recadrage

![](../assets/PerspectiveCropTool.png)

Le nouvel outil Recadrage de perspective vous permet de recadrer des matériaux déformés et de numériser avec quatre points de contrôle pour supprimer les artefacts de perspective et obtenir un élément assemblable.

![](../assets/sampler4.3-perspectivecrop-ezgif.com-video-gif.gif)

## Stylisation

![](../assets/03-8.png)

Le filtre Stylisation vous permet de styliser n’importe quelle matière pour obtenir un aspect peint à la main.

## Mode de fusion dans le filtre Fond

![](../assets/Fill-Blend-mode.gif)

La mise à niveau du filtre Remplissage introduit des modes de fusion, qui vous permettent de multiplier la valeur, les cartes d’entrée ou les générateurs de textures du remplissage avec les résultats de couche des calques sous-jacents.

## Améliorations apportées au calque d’importation d’image

![](../assets/Import-Layer-improvements.gif)

Vous pouvez ajouter plusieurs images sur un calque d’image d’importation et générer une carte d’opacité à partir de la couche Alpha d’une image.

## Note de mise à jour

*(Publié Le 25 Janvier 2024)*

<b>Ajouté</b> :

* [Assets] Nouveau type d’actif : Générateurs de textures
* [Ressources] Nouvelles matières incluses dans les ressources de démarrage
* [Ressources] Nouveau sélecteur de ressources pour les paramètres d’image dans le panneau Propriétés
* [Actifs] Faites glisser les générateurs de texture du panneau Actifs vers les sélecteurs d’image du panneau Propriétés.
* [Actifs] Glissez-déposez des générateurs de texture à partir de l’explorateur de fichiers du système d’exploitation
* [Ressources] Les filtres peuvent suggérer d’adapter les générateurs via une balise utilisateur sur l’entrée d’image
* [Assets] Les générateurs de textures peuvent définir quel filtre doit les suggérer via une balise utilisateur
* [Contenu] Nouveau filtre Correction de perspective par recadrage
* [Contenu] Nouveau filtre de stylisation
* [Contenu] Mode de fusion sur le filtre Fond
* [Contenu] Filtre Broderie mis à jour
* [Content] Mise à jour du filtre d’habillage de peinture
* [Content] Mise à jour de tous les filtres pour prendre en charge les générateurs de texture
* [Calques] Possibilité de choisir un canal de sortie du générateur de textures lors de son ajout à la pile de calques
* [Calques] Possibilité de répertorier et d’appliquer facilement des paramètres prédéfinis sur les générateurs de textures
* [Calques] Afficher un aperçu du générateur de textures dans les sélecteurs d’images
* [Calques] Les paramètres du générateur de textures peuvent être exposés et exportés.
* [Calques] Affectez la couleur de base utilisée lors de l’importation d’une seule image avec le modèle de création Importation de texture
* [Calques] Commentaires lors de la tentative de glisser-déposer de fichiers incompatibles dans les sélecteurs d’images du panneau Propriétés
* [Calques] Génération d’une couche d’opacité à partir de la couche alpha d’une image importée
* [Calques] Le calcul de l’image en matériau (IA) est plus rapide lors du changement de catégorie
* [Calques] Sélectionnez le calque le plus pertinent après avoir utilisé un modèle de création
* [Calques] Les widgets de position peuvent désormais être modifiés à l’aide d’un curseur dans le groupe Paramètres avancés
* [Exporter] Afficher un pourcentage dans la file d’attente plutôt que des nombres bruts
* [Interopérabilité] La couche d’opacité est désormais reconnue en tant que couche alpha lors de l’envoi vers Painter
* [Application] Nouvelle boîte de dialogue pour afficher et enregistrer les informations sur le matériel
* [Application] Nouvelle préférence pour modifier l’échelle d’height par défaut pour chaque projet
* [Application] Amélioration de l’affichage des ressources obsolètes
* [Scripting] Nouvelles fonctions asset.documentResolution() et asset.setDocumentResolution()
* [Scripting] Nouvelle fonction select\_asset()
* [Scripting] API Python pour les générateurs de textures
* [Scripting] get\_project\_assets() renvoie désormais les objets 3D
* [UI] La taille des vignettes des actifs peut être modifiée dans le panneau Actifs
* [UI] Mise à jour des icônes d&#39;affichage de la fenêtre d&#39;affichage

<b>Fixe :</b>

* [Vue 2D] Le zoom avec la molette de la souris est bloqué à 244 %
* [Application] Blocage au démarrage lors de l’initialisation de l’API graphique
* [Application] Blocage si le nom du projet contient le caractère #
* [Application] Blocage possible lors de l’ouverture d’un ancien projet
* [Application] La réouverture du projet actuel peut entraîner un blocage
* [Application] Certaines modifications apportées au projet ne sont pas enregistrées et sont perdues sans avertissement lors de la fermeture du projet si elles ne sont pas enregistrées
* [Export] Problèmes d’exportation .sbs/.sbsar lors de l’utilisation de plusieurs fichiers portant le même nom
* [Exportation] Espace colorimétrique incorrect pour le fichier .sbs/.sbsar des images en niveaux de gris exportées
* [Filtres] Problèmes de comportement du mélange d’opacité
* [Calques] Parfois, les fichiers .svg ne sont pas rendus à la bonne résolution
* [Performances] Certaines sauvegardes de projet sur le disque ne sont pas nécessaires
* [Projet] L’importation d’un ancien projet ne charge pas les paramètres prédéfinis associés
* [Scripting] Impossible d’obtenir les paramètres du premier calque inséré
* [UI] La fenêtre contextuelle d’aperçu lors du survol d’une ressource peut apparaître au mauvais emplacement ou à un mauvais écran
* [UI] Les panneaux non ancrés sont visibles et utilisables en haut de l’écran de bienvenue
