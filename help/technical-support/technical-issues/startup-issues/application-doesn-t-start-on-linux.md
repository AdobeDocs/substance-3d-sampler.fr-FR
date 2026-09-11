---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/technical-support/technical-issues/startup-issues/application-doesn-t-start-on-linux.html"
breadcrumb-title: ''
description: Découvrez comment résoudre les problèmes de démarrage de Substance 3D Sampler sous Linux afin de résoudre les problèmes de lancement d’application et les messages d’erreur.
helpx_creative_field: ""
helpx_description: Sampler > Technical Support > Technical Issues > Startup issues > Application doesnt start on Linux
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: L'application ne démarre pas sous Linux
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '108'
ht-degree: 0%

---


# L&#39;application ne démarre pas sous Linux

L&#39;application ne peut pas démarrer sous Linux avec le message d&#39;erreur suivant dans un terminal :

```
error while loading shared libraries: libicui18n.so.50
```


Cela signifie que l&#39;ICU de bibliothèque ([Composants internationaux pour Unicode](http://site.icu-project.org/)) est manquante ou que la version installée est trop récente. L’application nécessite la version 50.

Pour résoudre ce problème, installez la version 50 à partir du gestionnaire de modules ou [téléchargez manuellement](http://mirror.centos.org/centos/7/os/x86_64/Packages/libicu-50.2-4.el7_7.x86_64.rpm) la version manquante lors de l&#39;installation dans **/usr/lib64**.
