---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/release-notes/old-versions/version-3-2.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Sampler version 3.2 pour en savoir plus sur le workflow de numérisation de matériau, les nouveaux filtres et les métadonnées personnalisées.
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

**Substance 3D Sampler 3.2** introduit un workflow de numérisation de matériau de bout en bout qui capture et traite la taille physique du matériau, de nouveaux filtres tels que Tissu tissé et Commutateur de couche, ainsi que la possibilité de créer des métadonnées personnalisées.

Date de publication : 25 *janvier 2022*

## Principales fonctionnalités

### Taille physique

Une nouvelle procédure d&#39;analyse de matériau qui capture et traite la taille physique des matériaux est introduite dans cette version.

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

Ajoutez des métadonnées personnalisées à vos matériaux. Toutes les métadonnées personnalisées seront incluses dans le fichier de matériau (SBSAR) afin d’assurer un workflow plus efficace pour le partage de matériaux numériques entre les applications.

![](../../assets/custommetadata.png){width="264px"}

### Commutateur de canal

Avec l’option Permutation de canaux, vous pouvez désormais permuter les canaux des cartes de sortie du matériau.

![](../../assets/screenshot-2022-02-15-at-15-53-00.png){width="300px"}

### Exporter

De nouvelles fonctionnalités d’exportation ont été ajoutées à cette version.

* Définition du paramètre de compression .fichier sbsar

  ![](../../assets/compressionsbsar.png){width="400px"}
* Définition du type de graphe lors de l’exportation d’un fichier .sbs(ar)
* Conserver le ratio physique pour EXR, JPEG, PNG, TARGA, TIFF

  ![](../../assets/screenshot-2022-02-16-at-15-28-09.png){width="400px"}

## Notes de mise à jour

### 3.2.0 Yakitori

*(Publié Le 25 Janvier 2022)*

**Ajouté :**

* [Taille physique] Nouveau panneau Taille physique
* [Taille physique] Ajout d’options de Taille physique à la fenêtre Modèle de création de Matériau
* [Taille physique] Ajouter un outil de mesure de Taille physique
* [Taille physique] Ajouter un outil de mesure automatique de Taille physique
* [Taille physique] Ajout d’un outil de diagnostic de Taille physique
* [Taille physique] Permet de définir la valeur z de la Taille physique
* [Taille physique] Widget déroulant pour définir le niveau de zoom dans la Vue 2D
* [Taille physique] Nouvelle option « Afficher avec rapport physique » dans le menu déroulant du niveau de zoom
* [Taille physique] Nouvelle option « Adapter à la taille physique » dans le menu déroulant du niveau de zoom
* [Taille physique] Afficher la Taille physique dans la Vue 2D
* [Taille physique] Afficher la Taille physique dans le viewport 3D
* [Taille physique] Dans la boîte de dialogue d’importation d’image, affichez la profondeur de taille physique si une map height est importée
* [Taille physique] Afficher la Taille physique dans le menu contextuel de la ressource
* [Taille physique] Définissez l’unité de longueur dans les Préférences
* [Taille physique] textures d&#39;exportation concernant le rapport physique
* [Métadonnées] Possibilité d’ajouter des métadonnées personnalisées à une ressource créée par l’utilisateur
* [Exporter] Exporter des métadonnées personnalisées vers des fichiers .sbs(ar)
* [Exporter] Exportez les métadonnées de description, de catégorie, d’auteur et de balises vers des fichiers .sbs(ar)
* [Exporter] Exportez la Taille physique vers des fichiers .sbs(ar)
* [Export] Définition du paramètre de compression .fichier sbsar
* [Exporter] Exportez la vignette de la ressource vers des fichiers .sbs(ar)
* [Export] Définir le type de graphe lors de l&#39;exportation d&#39;un fichier .sbs(ar)
* [Application] Realtime Moteur 2021 n’est plus disponible
* [Application] La fonction Annuler/Rétablir prend désormais en charge les modifications des curseurs de Répétition (U,V) et d’échelle height
* [Rendu] Générer le cache disque lorsque l’actif créé est enregistré
* [Actifs] Utilisez Ctrl+clic pour activer plusieurs filtres de type d’actif dans le panneau Ressources
* [UI] Possibilité de verrouiller les curseurs de Répétition (U,V)
* [UI] Ajoutez un menu contextuel avec « Copier », « Couper », « Coller », « Copier tout » et « Couper tout » dans les champs de texte
* [UI] Unité de longueur (mètres, pouces, parsecs, ...) prise en charge dans les libellés et les champs de texte
* [UI] L’utilisateur peut définir la précision décimale utilisée pour afficher les nombres
* [UI] Utilisez des unités dans les fenêtres de mesure partout où cela est pertinent
* [Localisation] Le nouveau nom de ressource par défaut est maintenant localisé
* [Contenu] Nouveau générateur de tissu tissé
* [Contenu] Nouveau filtre de changement de canal
* [Contenu] Tous les filtres concernés connaissent désormais la Taille physique
* [Contenu] Nouvelles icônes de finition du bois
* [Contenu] Tous les filtres sont désormais compatibles avec les canaux Adobe Standard Material (ASM)
* [Contenu] Les filtres peuvent désormais avoir une variante « environnement »

**Fixe :**

* [vue 2D] Le canal reste dans la liste lorsqu’il est supprimé
* [Application] Impossible de dupliquer une ressource chargée à partir de l&#39;explorateur de fichiers du système d&#39;exploitation
* crash [Application] à la sortie
* [Application] Crash parfois lorsque vous cliquez sur « Ressources de démarrage » dans le panneau Ressources
* crash [Application] lors de la suppression d’un matériau
* [Application] La variable d’environnement « SUBSTANCE\_DISABLE\_SPECIFIC\_FEATURES » est toujours active lorsqu’elle est définie sur « 0 » ou « ».
* [Application] Blocage lors de l’enregistrement d’un projet comportant plusieurs matériaux
* [Application] L’importation d’une image peut entraîner un crash
* [Application] Ressources de démarrage manquantes au premier lancement
* [Exporter] L’exportation d’une ressource entraîne parfois un crash
* [Calques] Impossible d’importer des images lorsque le panneau Calques est fermé ou invisible
* [Calques] La modification de la langue entraîne le recalcul de l’actif actuel
* [Calques] La modification de l’utilisation d’une image importée ne met pas à jour la variante de filtre à utiliser
* [Calques] L’option Image vers Matériau (IA) n’est parfois pas calculée lors de l’ajustement des calques situés en dessous
* [Calques] L’option Image vers Matériau (IA) est parfois recalculée lorsque cela n’est pas nécessaire
* [Calques] Aucune mise à jour n’est suggérée lorsqu’un filtre personnalisé est mis à jour sur le disque
* [Calques] Le format de pixel de la couche normale est parfois incorrect
* [Calques] Certains calques sont toujours calculés, même lorsqu’ils ne sont pas visibles
* [Calques] Les outils Vue 2D peuvent être rompus lors du basculement de la visibilité d’un calque
* [Calques] L’interface utilisateur se bloque lors de l’utilisation de l’option Image vers Matériau (AI)
* [Calques] Le fait de basculer la visibilité du calque de Transforme casse l’outil Vue 2D et peut entraîner un crash
* [Calques] Trop de nouveaux calculs lors de la suppression d’un calque de la pile de calques
* [Calques] Lorsqu’un filtre composé contient une entrée/sortie inhabituelle ou personnalisée, Sampler ne la calcule pas
* [Performances] Le panneau Actifs est lent à s’ouvrir
* [Performances] Évitez de recalculer inutilement la pile de calques
* [Performance] Le chargement des ressources du projet prend trop de temps
* [Performance] Le cache de rendu sur le disque ne peut pas être utilisé
* [Performances] Le basculement entre les calques est lent
* [Performances] L’ajustement d’un matériau est lent
* [Projet] L’enregistrement d’un projet en quittant peut entraîner un crash
* [Rendu] La suppression d’une image peut supprimer toutes les sorties
* [Rendu] L’heure de rendu affichée dans le viewport est incorrecte lors des ajustements
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
