---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/release-notes/old-versions/version-3-2.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Sampler version 3.2 pour en savoir plus sur le workflow de numérisation des matériaux, les nouveaux filtres et les métadonnées personnalisées.
helpx_creative_field: ""
helpx_description: Sampler > Release Notes > Old Versions > Version 3.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 3.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '1058'
ht-degree: 0%

---


# Version 3.2

**Substance 3D Sampler 3.2** introduit un flux de travail de numérisation de matière de bout en bout qui capture et traite la taille physique de matière, de nouveaux filtres tels que Tissu tissé et Commutateur de couche, ainsi que la possibilité de créer des métadonnées personnalisées.

Date de publication : 25 *janvier 2022*

## Principales fonctionnalités

### Taille physique

Cette version introduit un nouveau workflow d’analyse des matériaux qui capture et traite la taille physique des matériaux.

Faites correspondre la [taille physique](../../features-and-workflows/end-to-end-physical-size-workflow.md) réelle de vos échantillons/images dans un contexte numérique pour créer des matériaux physiquement précis dans n&#39;importe quel logiciel.

![](../../assets/physicalsize-1.png){width="400px"}

### Tissé

Un tout nouveau générateur est ajouté à cette version. L’outil Tissu tissé vous permet de créer et de concevoir des tissus avec des motifs de tissage personnalisés.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/weavecollection.png){width="390px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/weaveinterface.png){width="400px"}

</td>
</tr>
</table>

### Métadonnées personnalisées

Ajoutez des métadonnées personnalisées à vos matières. Toutes les métadonnées personnalisées seront incluses dans le fichier de matériaux (SBSAR) afin d’assurer un workflow plus efficace pour le partage de matériaux numériques entre les applications.

![](../../assets/custommetadata.png){width="264px"}

### Commutateur de canal

Avec l’option Couches, vous pouvez désormais changer les couches des textures de sortie du matériau.

![](../../assets/screenshot-2022-02-15-at-15-53-00.png){width="300px"}

### Exporter

De nouvelles fonctionnalités d’exportation ont été ajoutées à cette version.

* Définition du paramètre de compression du fichier .sbsar

  ![](../../assets/compressionsbsar.png){width="400px"}
* Définition du type de graphique lors de l’exportation d’un fichier .sbs(ar)
* Conserver le rapport physique pour EXR, JPEG, PNG, TARGA, TIFF

  ![](../../assets/screenshot-2022-02-16-at-15-28-09.png){width="400px"}

## Notes de mise à jour

### 3.2.0 Yakitori

*(Publié Le 25 Janvier 2022)*

**Ajouté :**

* [Taille physique] Nouveau panneau Taille physique
* [Taille physique] Ajout d&#39;options de Taille physique à la fenêtre Modèle de création de matières
* [Taille physique] Ajouter un outil de mesure de Taille physique
* [Taille physique] Ajouter un outil de mesure automatique de Taille physique
* [Taille physique] Ajout d’un outil de diagnostic de Taille physique
* [Taille physique] Permet de définir la valeur z de la Taille physique
* [Taille physique] Widget déroulant pour définir le niveau de zoom dans la vue 2D
* [Taille physique] Nouvelle option « Afficher avec rapport physique » dans le menu déroulant du niveau de zoom
* [Taille physique] Nouvelle option « Adapter à la taille physique » dans le menu déroulant du niveau de zoom
* [Taille physique] Afficher la Taille physique dans la vue 2D
* [Taille physique] Afficher la Taille physique dans la clôture 3D
* [Taille physique] Dans la boîte de dialogue d’importation d’image, affichez la profondeur de taille physique si un mappage d’height est importé
* [Taille physique] Afficher la Taille physique dans le menu contextuel de la ressource
* [Taille physique] Définissez l’unité de longueur dans les Préférences
* [Taille physique] Exportation de textures respectant le rapport physique
* [Métadonnées] Possibilité d’ajouter des métadonnées personnalisées à une ressource créée par l’utilisateur
* [Exporter] Exporter des métadonnées personnalisées vers des fichiers .sbs(ar)
* [Exporter] Exportez les métadonnées de description, de catégorie, d’auteur et de balises vers des fichiers .sbs(ar)
* [Exporter] Exportez la Taille physique vers des fichiers .sbs(ar)
* [Export] Définition du paramètre de compression du fichier .sbsar
* [Exporter] Exportez la vignette de la ressource vers des fichiers .sbs(ar)
* [Exporter] Définition du type de graphique lors de l’exportation d’un fichier .sbs(ar)
* [Application] Realtime Engine 2021 n’est plus disponible
* [Application] La fonction Annuler/Rétablir prend désormais en charge les modifications des curseurs Limites (U,V) et Échelle height
* [Rendu] Générer le cache disque lorsque l’actif créé est enregistré
* [Actifs] Utilisez Ctrl+clic pour activer plusieurs filtres de type d’actif dans le panneau Ressources
* [UI] Possibilité de verrouiller les curseurs de mosaïque (U,V)
* [UI] Ajoutez un menu contextuel avec « Copier », « Couper », « Coller », « Copier tout » et « Couper tout » dans les champs de texte
* [UI] Unité de longueur (mètres, pouces, parsecs, ...) prise en charge dans les libellés et les champs de texte
* [UI] L’utilisateur peut définir la précision décimale utilisée pour afficher les nombres
* [UI] Utilisez des unités dans les fenêtres de mesure partout où cela est pertinent
* [Localisation] Le nouveau nom de ressource par défaut est maintenant localisé
* [Contenu] Nouveau générateur de tissu tissé
* [Contenu] Nouveau filtre de changement de canal
* [Contenu] Tous les filtres concernés connaissent désormais la Taille physique
* [Contenu] Nouvelles icônes de finition du bois
* [Contenu] Tous les filtres sont désormais compatibles avec les canaux ASM (Adobe Standard Materials)
* [Contenu] Les filtres peuvent désormais avoir une variante « environnement »

**Fixe :**

* [Vue 2D] Le canal reste dans la liste lorsqu’il est supprimé
* [Application] Impossible de dupliquer une ressource chargée à partir de l&#39;explorateur de fichiers du système d&#39;exploitation
* [Application] Blocage à la sortie
* [Application] Blocage parfois lorsque vous cliquez sur « Ressources de démarrage » dans le panneau Ressources
* [Application] Blocage lors de la suppression d’un matériau
* [Application] La variable d’environnement « SUBSTANCE\_DISABLE\_SPECIFIC\_FEATURES » est toujours active lorsqu’elle est définie sur « 0 » ou « ».
* [Application] Blocage lors de l’enregistrement d’un projet avec plusieurs matériaux
* [Application] L’importation d’une image peut entraîner un blocage
* [Application] Ressources de démarrage manquantes au premier lancement
* [Export] L’exportation d’une ressource entraîne parfois un blocage
* [Calques] Impossible d’importer des images lorsque le panneau Calques est fermé ou invisible
* [Calques] La modification de la langue entraîne le recalcul de l’actif actuel
* [Calques] La modification de l’utilisation d’une image importée ne met pas à jour la variante de filtre à utiliser
* [Calques] L’effet Image vers matériau (IA) n’est parfois pas calculé lors de l’ajustement des calques situés en dessous
* [Calques] Image vers matériau (AI) est parfois recalculé lorsque cela n’est pas nécessaire
* [Calques] Aucune mise à jour n’est suggérée lorsqu’un filtre personnalisé est mis à jour sur le disque
* [Calques] Le format de pixel de la couche normale est parfois incorrect
* [Calques] Certains calques sont toujours calculés, même lorsqu’ils ne sont pas visibles
* [Calques] Les outils d’affichage 2D peuvent être rompus lors du basculement de la visibilité d’un calque
* [Calques] L’interface utilisateur se fige lors de l’utilisation de Image vers matériau (AI)
* [Calques] Le fait de basculer la visibilité du calque du filtre Transformation rompt l’outil d’affichage 2D et peut entraîner un blocage
* [Calques] Trop de nouveaux calculs lors de la suppression d’un calque de la pile de calques
* [Calques] Lorsqu’un filtre composé contient une entrée/sortie inhabituelle ou personnalisée, Sampler ne la calcule pas
* [Performances] Le panneau Actifs est lent à s’ouvrir
* [Performances] Évitez de recalculer inutilement la pile de calques
* [Performance] Le chargement des ressources du projet prend trop de temps
* [Performance] Le cache de rendu sur le disque ne peut pas être utilisé
* [Performances] Le basculement entre les calques est lent
* [Performance] Le réglage d’un matériau ou d’un filtre est lent
* [Projet] L’enregistrement d’un projet en quittant peut entraîner un blocage
* [Rendu] La suppression d’une image peut supprimer toutes les sorties
* [Rendu] Le temps de rendu affiché dans la clôture est incorrect lors de l’ajustement
* [UI] Impossible de faire défiler verticalement dans la fenêtre contextuelle d’exportation si nécessaire
* [UI] Il est possible d’ouvrir la fenêtre contextuelle d’exportation lorsque rien ne doit être exporté
* [UI] Certaines fenêtres ne défilent pas si leur contenu déborde
* [UI] Les champs de texte ne sont pas sélectionnés lorsque vous cliquez dessus ou ouvrez un menu
* [UI] Le nom du mode de fusion dans le panneau des propriétés est parfois incorrect
* [UI] L’option Enregistrer du menu Fichier est parfois grisée
* [UI] Le champ de texte ne disparaît pas après avoir renommé deux matériaux
* [UI] Erreur de frappe dans la fenêtre contextuelle des préférences

**Problèmes Connus :**

* [Sélecteur de couleurs] Le choix d’une couleur sur un deuxième moniteur avec une résolution différente peut ne pas fonctionner
