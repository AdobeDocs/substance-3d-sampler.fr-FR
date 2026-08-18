---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/technical-support/configuration/retrieving-the-installation-path.html"
breadcrumb-title: ''
description: Découvrez comment récupérer le chemin d’installation de Substance 3D Sampler sur différentes plateformes à des fins de script et de configuration.
helpx_creative_field: ""
helpx_description: Sampler > Technical Support > Configuration > Retrieving the installation path
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Récupération du chemin d’installation
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 6%

---


# Récupération du chemin d’installation

Cette page regroupe des informations sur la façon de récupérer le chemin d’installation de l’application en fonction de la version et de la plate-forme.

## Windows

### Application pour poste de travail Creative Cloud

1. Ouvrez l&#39;éditeur de registre Windows (**regedit**).
1. Accédez à la clé de registre : ** HKEY\_LOCAL\_MACHINE\Software\Microsoft\Windows\CurrentVersion\App Paths\**
1. Ouvrez la sous-clé nommée **Adobe Substance 3D Sampler.exe**
1. La valeur de la clé contient le chemin d’accès à l’exécutable de l’application sur lequel elle est installée

>[!NOTE]
>
> Cette clé de registre n’est disponible qu’à partir de la version 3.\
> Pour les anciennes versions, le chemin d&#39;installation peut être récupéré à partir des associations de fichiers dans **HKEY\_CURRENT\_USER\Software\Microsoft\Windows\CurrentVersion\ Explorer\FileExts**.

### Substance 3D Standalone

1. Ouvrez l&#39;éditeur de registre Windows (**regedit**).
1. Accédez à la clé de registre : **HKEY\_LOCAL\_MACHINE\ SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall**
1. Recherchez la sous-clé correspondant à l’AppID de la version de votre application (voir le tableau ci-dessous).
1. La valeur de la clé contient le chemin d’accès à l’emplacement d’installation de l’application

| Version | AppId |
| --- | --- |
| **1.x (2019.x) à 2.x** | {B3506E85-E98F-4D48-A010-BE4DEE27D108} |
| **3.x (ou plus récent)** | {ED4A4ABC-9B7D-44B8-984A-C8A994B69CFD} |

### Vapeur

L’application est installée dans le sous-dossier **steamapps/common/** du dossier d’installation de Steam.

## Mac

Sous Mac, l’application est installée dans les emplacements suivants :

| Version | Chemin |
| --- | --- |
| **3.x ou version plus récente** | **/Applications/Adobe Substance 3D Sampler.app** |
| **Hérité** | **/Applications/Substance Alchemist.app** |

## Linux

Sous Linux, le package rpm est installé dans le chemin suivant :

| Version | Chemin |
| --- | --- |
| **3.x ou version plus récente** | **/opt/Adobe/Adobe\_Substance\_3D\_Sampler** |
| **Hérité** | **/opt/Allegorithmic/Substance\_Alchemist** |
