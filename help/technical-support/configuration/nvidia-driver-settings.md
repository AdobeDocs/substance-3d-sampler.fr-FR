---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/technical-support/configuration/nvidia-driver-settings.html"
breadcrumb-title: ''
description: Découvrez comment configurer les paramètres du pilote NVIDIA pour Substance 3D Sampler afin d’optimiser les performances du GPU et de résoudre les comportements lents.
helpx_creative_field: ""
helpx_description: Sampler > Technical Support > Configuration > NVIDIA Driver Settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Paramètres du pilote NVIDIA
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---


# Paramètres du pilote NVIDIA

Si vous utilisez un GPU NVIDIA mais que les performances sont médiocres, il existe deux causes courantes :

1. Les pilotes sont manquants ou non à jour
1. Sampler utilise un GPU incorrect

## Mettre à jour les pilotes

Pour mettre à jour vos pilotes NVIDIA :

1. Accédez à la page de téléchargement du pilote NVIDIA - <https://www.nvidia.com/Download/index.aspx?lang=en-us>
1. Sélectionnez votre modèle de GPU et téléchargez les pilotes.
1. Installez les pilotes contenant le fichier téléchargé.

Une fois les derniers pilotes installés, ouvrez Sampler pour voir si les performances se sont améliorées. Si les performances sont lentes, Sampler peut utiliser un GPU incorrect.

## Configuration de Sampler

Pour savoir quel GPU Sampler utilise, procédez comme suit :

![](../../assets/nvidiacontrolpanel.png)

1. Ouvrez le Panneau de configuration NVIDIA. Pour ouvrir le Panneau de configuration NVIDIA, effectuez l’une des opérations suivantes :
   1. Recherche de Panneau de configuration NVIDIA à l’aide du menu Démarrer
   1. Dans la barre d’état système, cliquez avec le bouton droit sur l’icône Force et sélectionnez Panneau de configuration NVIDIA.
1. Dans le panneau de configuration NVIDIA, sélectionnez Gérer les paramètres 3D dans le menu de gauche.
1. Sélectionnez l’onglet Paramètres du programme.
1. Sous Sélectionner un programme à personnaliser, utilisez la liste déroulante pour rechercher Sampler.
1. Si Sampler n’est pas répertorié dans la liste déroulante, utilisez Ajouter.
   1. Recherchez l&#39;emplacement d&#39;installation de Sampler (l&#39;emplacement d&#39;installation par défaut est **C :/Program Files/Adobe/Adobe Substance 3D Sampler**).
   1. Sélectionnez **Adobe Substance 3D Sampler.exe** dans l&#39;emplacement d&#39;installation.
1. Avec Sampler sélectionné, sous « Sélectionner le processeur graphique préféré pour ce programme : » sélectionnez « Processeur NVIDIA hautes performances ».
1. Cliquez sur Appliquer.

Une fois que vous avez suivi ce processus, ouvrez Sampler pour voir si les performances se sont améliorées.
