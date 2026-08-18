---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/getting-started/activation-and-licenses.html"
breadcrumb-title: ''
description: Découvrez comment activer et gérer les licences pour que Substance 3D Sampler puisse commencer à utiliser l’application et accéder à toutes les fonctionnalités.
helpx_creative_field: ""
helpx_description: Sampler > Getting Started > Activation and licenses
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Activation et licences
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 1%

---


# Activation et licences

Cette page contient des informations sur l’activation et la gestion de vos licences afin que vous puissiez commencer à utiliser Sampler.

## Processus d’activation par type d’application

Le processus d’activation dépend de l’endroit où vous avez acheté ou accédé à Sampler :

| Type d’application | Processus d’activation |
| --- | --- |
| Application pour poste de travail Creative Cloud | Voir la page dédiée dans la [documentation HelpX](https://helpx.adobe.com/fr/support/substance-3d-sampler.html).En cas de problème, la [documentation du Creative Cloud](https://helpx.adobe.com/fr/creative-cloud/user-guide.html) peut fournir des réponses supplémentaires. |
| Vapeur | Lancez le produit directement à partir de la bibliothèque Steam. |
| Substance 3D autonome | Voir le processus d’activation décrit ci-dessous. |

## Étapes d’activation

### Assistant d’activation

![](../assets/activation-wizard.png){width="350px"}

Trois choix s&#39;offrent à vous :

* **Évaluer ce produit** : les versions d&#39;évaluation héritées ne sont plus disponibles. Vous pouvez à la place commencer une version d&#39;essai de 30 jours pour chaque application Substance 3D [ici](https://www.adobe.com/creativecloud/3d-augmented-reality.html) ou avec Creative Cloud Desktop. Chaque version d’essai est indépendante des autres applications Substance 3D, vous pouvez donc les tester une par une ou toutes à la fois.
* **Activer à l&#39;aide d&#39;un fichier de licence** : activez le produit avec un fichier de licence (**\*.key**) téléchargé à partir de la page de votre compte sur le [site web Substance 3D](https://store.substance3d.com/user) avant le 30 septembre 2022.
* **Activer à l&#39;aide de votre compte** : les comptes Substance hérités ne peuvent plus être utilisés pour l&#39;activation. [Plus d&#39;informations sur les comptes de Substance de données sont disponibles ici](https://helpx.adobe.com/fr/substance-3d/unlisted/faq-end-of-life-accounts.html).

>[!WARNING]
>
> Pour installer le fichier de licence avec l’Assistant d’activation, assurez-vous d’exécuter Sampler en tant qu’administrateur et de désactiver temporairement votre antivirus.

### Activation manuelle

Il est possible d&#39;activer manuellement Sampler en plaçant le fichier **license.key** dans le dossier suivant :

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> <col/> </colgroup><tbody><tr><th>Plateforme</th><th>Version</th><th colspan="2">Chemin</th></tr><tr><td rowspan="4"><strong>Windows</strong></td><td rowspan="2"><strong>3.0</strong> ou version plus récente</td><td colspan="1">Données de l’application (local)</td><td colspan="1">C:\Users\[nom d’utilisateur]\AppData\Local\Adobe\Adobe Substance 3D Sampler</td></tr><tr><td colspan="1">Données d’application (itinérance)</td><td colspan="1">C:\Users\[nom d’utilisateur]\AppData\Roaming\Adobe\Adobe Substance 3D Sampler</td></tr><tr><td rowspan="2">Ancien système</td><td colspan="1">Données de l’application (local)</td><td colspan="1">C:\Users\[nom d’utilisateur]\AppData\Local\Allegorithmic\Substance Alchemist</td></tr><tr><td colspan="1">Données d’application (itinérance)</td><td colspan="1">C:\Users\[nom d’utilisateur]\AppData\Roaming\Allegorithmic\Substance Alchemist</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>3.0</strong> ou version plus récente</td><td colspan="2">/Users/[nom d’utilisateur]/Library/Application Support/Adobe/Adobe Substance 3D Sampler</td></tr><tr><td colspan="1">Ancien système</td><td colspan="2">/Users/[nom d’utilisateur]/Library/Application Support/Allegorithmic/Substance Alchemist</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>3.0</strong> ou version plus récente</td><td colspan="2">/home/[nom d’utilisateur]/.local/share/Adobe/Adobe Substance 3D Sampler</td></tr><tr><td>Ancien système</td><td colspan="2">/home/[nom d’utilisateur]/.local/share/Allegorithmic/Substance Alchemist</td></tr></tbody></table>

>[!NOTE]
>
> Certains des répertoires dans les chemins mentionnés ci-dessus peuvent être masqués par défaut. Saisissez le chemin manuellement dans l’explorateur de fichiers ou affichez les fichiers masqués pour les afficher.

>[!NOTE]
>
> Assurez-vous que le fichier s&#39;appelle **license.key**, sinon l&#39;application ne pourra pas le trouver.

### Variable d’environnement

Vous pouvez remplacer l&#39;emplacement que Sampler recherche pour le fichier **license.key** par une [variable d&#39;environnement](../pipeline-and-integrations/environment-variables.md).
