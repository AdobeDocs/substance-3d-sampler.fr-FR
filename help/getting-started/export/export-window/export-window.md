---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/getting-started/export/export-window.html"
breadcrumb-title: ''
description: Apprenez à utiliser la fenêtre d’exportation de Substance 3D Sampler pour configurer et exporter des matériaux dans différents formats et paramètres prédéfinis.
helpx_creative_field: ""
helpx_description: Sampler > Getting Started > Export > Export Window
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Fenêtre d’exportation
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0f989901713dd30f8f936de2445caf5dc70a9225
workflow-type: tm+mt
source-wordcount: '737'
ht-degree: 0%

---


# Fenêtre d’exportation

Vous pouvez exporter votre ressource à partir du panneau <b>Exporter</b> dans la <b>barre de droite</b>.

Les options d’exportation dépendent du type de fichier exporté.

![Image de la fenêtre d&#39;exportation](../../../assets/6.0_ExportWindowMaterialSettings.png)

Fenêtre d&#39;exportation d&#39;une exportation de matières.

>[!NOTE]
>
> Le panneau Exporter propose également des options pour Envoyer votre ressource vers Substance 3D Designer, Painter ou Stager. Cette opération exportera automatiquement votre ressource avec les paramètres appropriés pour les autres applications Substance 3D.

## Paramètres généraux

Les paramètres suivants sont disponibles pour tous les types de ressources.

* <b>Nom :</b>Ce champ définit le nom de l’actif que vous exportez. Il sera utilisé comme préfixe dans le nom de fichier des fichiers exportés.
* <b>Enregistrer dans :</b>Sélectionnez la destination d’exportation de votre ressource. Vous pouvez également éventuellement créer un sous-dossier à l’emplacement choisi. Si cette option est activée, le sous-dossier portera le nom de votre ressource.

## Paramètres de matière

Lors de l’exportation de matériaux, le panneau Paramètres de matériau de la fenêtre Exporter propose les options suivantes :

* <b>Format</b> : sélectionnez un format de fichier pour votre ressource exportée.
  * <b>SBSAR</b> : exportez votre matière pour l&#39;utiliser dans n&#39;importe quelle application prenant en charge les matières de Substance.
  * <b>SBS</b> : exportez votre matière afin qu&#39;elle puisse être ouverte dans Substance 3D Designer.
  * <b>EXR, JPEG, PNG, TARGA, TIFF</b> : exportez votre matière sous la forme d’une collection de fichiers image.

>[!NOTE]
>
> Le nombre de bits par pixel est forcé à 16 bits pour les canaux Normal et Height. Les autres couches sont exportées en 8/16 bits en fonction de vos matières et des filtres utilisés par votre ressource. Selon le format de fichier, le nombre de bits par pixel peut être modifié, car certains formats de fichiers ne prennent pas en charge le nombre de bits par pixel élevé.

![](../../../assets/export-format.png){width="400px"}

* <b>Paramètre prédéfini </b>(EXR, JPEG, PNG, TARGA, TIFF) : sélectionnez un paramètre prédéfini pour configurer automatiquement l’exportation de fichiers pour une application ou un pipeline donné.
  * L&#39;option <b>Par défaut (workflow du projet)</b> affiche une liste de tous les canaux disponibles de votre ou vos matériaux sans aucun paramètre prédéfini appliqué.
  * Utilisez le bouton <b>Gérer les paramètres prédéfinis </b> à droite du paramètre Paramètres prédéfinis pour modifier les paramètres prédéfinis ou ajouter les vôtres.<b> </b>
  * [Pour plus d’informations sur les paramètres prédéfinis, cliquez ici.](../managing-presets.md)

>[!NOTE]
>
> La sélection des paramètres prédéfinis n’est pas disponible lorsque votre format d’exportation est SBS ou SBSAR. Pour ces formats, le fichier de sortie est déjà configuré pour être utilisable dans tous les produits de Substance et toutes les intégrations de Substance.

* <b>Type de matériau </b>(SBSAR, SBS) : sélectionnez si le matériau exporté se comporte comme un matériau standard, une décalcomanie ou un atlas. Ce paramètre peut changer la façon dont il est traité par d&#39;autres applications qui prennent en charge les fichiers SBSAR et SBS.

![](../../../assets/screenshot-2023-01-24-at-16-32-58.png)

* <b>Compression </b>(SBSAR, SBS) : sélectionnez la méthode de compression du fichier exporté
  * <b>Auto</b> : permet à Sampler de déterminer les paramètres de compression.
  * <b>Idéal</b> : cette option réduit la taille des fichiers, mais peut également allonger les temps de chargement et d’enregistrement pendant le codage ou le décodage du fichier.
  * <b>Aucun</b> : sans compression, les fichiers seront plus volumineux, mais seront chargés et enregistrés plus rapidement.
* <b>Résolution (</b>SBSAR, SBS<b>)</b> : sélectionnez une résolution de sortie pour le matériau.
  * Par défaut, la résolution est basée sur les paramètres globaux de Sampler. Si vous sélectionnez une résolution différente, Sampler recalcule tous vos matériaux avec cette nouvelle résolution. Cela peut affecter l’aspect final de votre ou vos matériaux.

![](../../../assets/SAPR_ResolutionSBSAR.png)

* <b>Résolution </b> (Formats d’image) : indiquez si la résolution de chaque calque doit être exportée indépendamment ou si elle doit remplacer la résolution afin que tous les calques soient exportés à une taille uniforme. Si l’option Tout remplacer est sélectionnée, des options permettant de modifier la résolution de sortie apparaissent.
  * Par défaut, la résolution est basée sur la résolution de sortie de chaque calque. Si vous sélectionnez une résolution différente, Sampler recalcule tous vos matériaux avec cette nouvelle résolution. Cela peut affecter l’aspect final de votre ou vos matériaux.

![](../../../assets/SAPR_ResolutionTextures.png)

* **Modèle de matériau** (tous les formats dans le paramètre prédéfini par défaut) : sélectionnez une norme de nuanceur pour vos textures exportées.
  * La modification du Modèle de matériau aura un impact sur les noms de fichiers des fichiers exportés. Par exemple, OpenPBR utilise « Metalness » au lieu d&#39;ASM qui utilise « Metallic ».

### Informations supplémentaires

L&#39;espace disque disponible sur le lecteur de destination sélectionné est visible au bas de la <b>fenêtre d&#39;exportation</b>.

>[!NOTE]
>
> La <b>Taille physique</b> est définie lors de la création de la matière et ne peut pas être modifiée lors de l&#39;exportation.

### Canaux

![](../../../assets/SAPR_Channelspreview.png)

Sur le côté droit du panneau <b>Paramètres de matière</b>, une liste des couches pouvant être exportées et leur résolution est visible (couches par défaut et couches personnalisées).

Chaque préréglage possède un ensemble différent de canaux à exporter, et le nom des fichiers exportés est basé sur les noms visibles dans la zone <b>Canaux à exporter</b>. Vous pouvez cocher la case en regard de n’importe quel canal pour activer ou désactiver l’exportation pour ce canal.

![](../../../assets/SAPR_Channels_ExportPreset.gif)
