---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/scripting-and-development/manage-installed-plugins-and-scripts.html"
breadcrumb-title: ''
description: Découvrez comment gérer les plug-ins et les scripts installés dans Substance 3D Sampler pour installer, modifier et supprimer des extensions personnalisées.
helpx_creative_field: ""
helpx_description: Sampler > Scripting and Development > Manage installed plugins and scripts
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gestion des plug-ins et des scripts installés
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---


# Gestion des plug-ins et des scripts installés

Pour installer, modifier ou supprimer des plug-ins, utilisez Édition > Préférences, puis sélectionnez Plug-ins et scripts.

![](../assets/preferences-86.png)

Dans le panneau Plug-ins et scripts, vous pouvez activer le panneau Journal qui affiche la sortie des plug-ins. Cela peut être utile pour le dépannage et le débogage. Une fois activé, vous pouvez ouvrir le panneau Journal à partir de la barre de droite dans l’interface principale de Sampler. Le panneau Journal peut être ancré comme les autres panneaux Sampler.

## Modules externes et scripts

La principale différence entre les plug-ins et les scripts réside dans le fait que les plug-ins incluent des éléments d’interface utilisateur où les scripts n’en incluent pas. Les plug-ins nécessitent au moins un fichier PY et un fichier QML. Le fichier XML définit les éléments de l’interface utilisateur, tandis que le fichier PY définit le comportement du plug-in. Les scripts, en revanche, se composent uniquement d’un fichier PY.

Les éléments de l’interface utilisateur d’un plug-in signifient que le comportement du plug-in peut être modifié à l’aide de paramètres. Par exemple, le module externe d’enregistrement automatique comporte des commandes qui permettent de modifier le temps entre les enregistrements automatiques. Les plug-ins font partie de l’interface de Sampler et peuvent être ancrés et déplacés comme les panneaux Sampler standard.

Les scripts ne permettent pas ce niveau de flexibilité, mais effectuent plutôt une tâche donnée. Par exemple, le script Tout exporter se comportera toujours de la même manière lorsqu’il sera appelé. Les scripts sont accessibles à partir de la barre de menus supérieure. Le menu Script n’est disponible qu’une fois les scripts ajoutés à Sampler.

## Gérer les plug-ins

Par défaut, la seule option disponible est « Ajouter un module ». Un explorateur de fichiers s’ouvre, dans lequel vous pouvez sélectionner un fichier PY à charger.

![](../assets/manageplugins.png)

>[!NOTE]
>
> Les plug-ins nécessitent un fichier PY et un fichier QML pour fonctionner. Lorsque vous sélectionnez un fichier PY à importer, Sampler recherche un fichier QML dans le dossier. Si aucun fichier XML n’est trouvé, le chargement du plug-in échouera.

Une fois qu’un plug-in est installé, quelques options deviennent disponibles :

* Vous pouvez réorganiser les plug-ins en faisant glisser la poignée à gauche du plug-in.
* Activez ou désactivez les plug-ins à l’aide du commutateur à bascule.
* Utilisez le bouton de menu à droite de chaque plug-in pour recharger, supprimer ou ouvrir l’emplacement du dossier du plug-in.

Les plug-ins installés apparaissent initialement dans la barre de droite de l’interface principale de Sampler. À partir de là, vous pouvez ouvrir, ancrer et déplacer le panneau des plug-ins tout comme les panneaux Sampler standard.

## Gérer les scripts

Les scripts peuvent être gérés de la même manière que les plug-ins.

![](../assets/managescripts.png)

Une fois qu’un script est installé, quelques options deviennent disponibles :

* Réorganisez les scripts à l’aide de la poignée située à gauche du script.
* Activez ou désactivez le script à l’aide du bouton bascule.
* Utilisez le bouton de menu à droite de chaque script pour supprimer le script ou ouvrez l’emplacement du dossier du script.
* Une fois importés, les scripts sont copiés dans **%\AppData\Roaming\Adobe\Adobe Substance 3D Sampler\scripts**
* Pour modifier le script, vous devez modifier celui copié par Sampler
