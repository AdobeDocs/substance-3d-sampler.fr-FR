---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/interface/panels/share-panel.html"
breadcrumb-title: ''
description: Apprenez à utiliser le panneau Exportation de Substance 3D Sampler pour exporter des matériaux sous forme de fichiers ou les envoyer directement à d’autres applications.
helpx_creative_field: ""
helpx_description: Sampler > Interface > Panels > Export panel
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Panneau Exporter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0f989901713dd30f8f936de2445caf5dc70a9225
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 3%

---


# Panneau Exporter

Le <b>panneau Exporter</b> vous permet d&#39;exporter vos actifs sous forme de fichiers généraux ou d&#39;envoyer des actifs directement à d&#39;autres applications.

## Envoyer à...

Les options Envoyer vers... vous permettent d’envoyer directement votre fichier à d’autres applications installées sur votre système. Cela est généralement beaucoup plus rapide que l’importation et l’exportation de ressources.

Actuellement, Sampler prend en charge l’envoi à :

* **Substance 3D Painter** : importez des matériaux et des environnements que vous pouvez utiliser lors de la texturation de vos actifs.
* **Substance 3D Stager** : importe les éclairages de l’environnement pour changer l’ambiance de votre scène. Disponible uniquement avec les éclairages de l’environnement, désactivé pour les matériaux.

Les matériaux sont toujours envoyés comme SBSAR, les environnements comme EXR.

## Exporter

Cliquez sur **Exporter sous...** pour exporter la ressource sur laquelle vous travaillez actuellement. Choisissez de modifier les paramètres généraux ou les paramètres de matière dans le menu de gauche.

### Paramètres généraux

Lorsque les paramètres généraux sont sélectionnés, vous pouvez modifier le nom de la matière et l’emplacement d’enregistrement. Vous pouvez également choisir de créer ou non un sous-dossier pour le matériau. Cela peut être utile lors de l’exportation dans un format d’image qui crée plusieurs fichiers.

### Paramètres de matériau

Lorsque les paramètres de matière sont sélectionnés, vous pouvez modifier différents paramètres pour contrôler la manière dont la matière sera exportée :

| Paramètre | Description |
| --- | --- |
| Format | Choisissez d’exporter l’image sous forme de fichier SBS, SBSAR ou sous forme de collection d’images dans un format d’image spécifique |
| Paramètre prédéfini | Sélectionnez un paramètre prédéfini pour organiser automatiquement votre exportation pour une application spécifique. [Plus d&#39;informations sur les paramètres prédéfinis sont disponibles ici](../../getting-started/export/default-presets/default-presets.md). Les paramètres prédéfinis ne sont disponibles que lorsqu’un format d’image est sélectionné. |
| Compression | Choisir si la compression privilégie la vitesse ou l&#39;efficacité <br> <ul> <li> **Auto** : permet à Sampler de choisir. <li> **Idéal** : optimisez l’efficacité de la compression pour les fichiers de petite taille. <li> **Aucune** : l’absence de compression signifie une ouverture et une fermeture plus rapides des fichiers exportés, mais des fichiers plus volumineux. </ul> |
| Résolution | Modifiez la résolution de votre exportation. Cette option s&#39;affiche différemment en fonction du format sélectionné <br> <ul> <li> **SBSAR/SBS** : sélectionnez une largeur et un height par défaut pour le matériau. Elles peuvent être mises à jour ultérieurement. <li> **Format d&#39;image** : choisissez entre **Sortie des calques** qui exporte chaque mappage à la taille définie par la pile de calques, ou **Remplacer tout** qui vous permet de spécifier une largeur et un height pour l&#39;exportation. |
| Modèle de matériau | Indiquez si vous souhaitez exporter en tant que matériau Adobe Standard ou en tant que matériau OpenPBR. L’option à sélectionner doit dépendre des autres applications que vous utilisez dans votre pipeline. Différents canaux seront disponibles en fonction du Modèle de matériau. |
| Canaux | Activez/désactivez les canaux à exporter dans le cadre de votre ressource. |

>[!NOTE]
>
> Pour plus d&#39;informations sur les options de la boîte de dialogue Exporter et d&#39;autres informations telles que les formats de fichiers, consultez l&#39;[article Export](../../getting-started/export/export.md) et son [sous-article sur la fenêtre d&#39;exportation](../../getting-started/export/export-window/export-window.md).

Une fois que vous êtes satisfait des paramètres d&#39;exportation, cliquez sur **Exporter**. Votre exportation apparaîtra dans la file d’attente d’exportation qui affiche une liste des exportations récentes. Cliquez sur l’icône de dossier d’une exportation pour ouvrir l’emplacement de fichier de cette exportation.
