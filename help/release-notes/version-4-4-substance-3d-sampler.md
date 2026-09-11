---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/release-notes/version-4-4substance-3d-sampler.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Sampler version 4.4 pour en savoir plus sur les workflows génératifs, y compris les fonctionnalités de synthèse de texte en texture et d’image en texture.
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 4.4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 6cc0519fb8c0f74fa805691ec4adb9e449a627d5
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---


# Version 4.4

<b>Substance 3D Sampler 4.4</b> introduit trois nouveaux workflows génératifs en version bêta : Texte en texture, Texte en motif et Image en texture.

<b>Les fonctionnalités d&#39;IA générative sont uniquement disponibles sur la version Adobe</b>, car elle nécessite un compte Adobe. Par conséquent, ces fonctionnalités ne sont <b>pas disponibles sur Steam</b>.

*Date de publication : 23 mai 2024*

## Texte en texture

![](../assets/textToTexture_whatNewPanel.png)

La fonction de texte en texture vous permet d&#39;explorer une nouvelle façon de créer des matériaux avec une <b>invite de texte</b>. Vous pouvez générer une texture en mosaïque à partir d’une description de texte détaillée et continuer à vous appuyer sur les résultats obtenus par le biais de l’option De l’image vers le matériau ou de tout autre filtre Sampler pour en faire un élément unique à votre image.

## Image à texture

![image à texture](../assets/imagetoText_whatNewPanel.png "image à texture")

Grâce à la fonction de transformation d&#39;image en texture, vous pouvez créer des textures carrées en mosaïque à partir de <b>votre propre image de référence</b>, qu&#39;elle soit carrée ou non répétition. Cela vous rapproche des résultats souhaités sans avoir à écrire l’invite parfaite.\
La conversion d’image en texture peut également vous aider à gagner du temps en créant des variantes à partir du contenu que vous avez déjà créé.

## Text-to-pattern

![image d&#39;illustration texte à motif](../assets/patterns_whatNewPanel.png)

La fonction de conversion de texte en motif utilisera votre invite de texte <b></b> pour générer un motif de répétition carrée. Vous pouvez ensuite l’utiliser comme base color avec un filtre Tissu tissé pour créer un matériau de tissu original, l’utiliser comme entrée d’un filtre Motif et bien plus encore !

## Note de mise à jour

*(Publié Le 23 Mai 2024)*

<b>Ajouté</b> :

* [Application] Le cache capture 3D est maintenant stocké dans un sous-dossier séparé
* [IA générative] De l’image à la Texture (bêta)
* [IA générative] Texte en motif (Beta)
* [IA générative] Texte en Texture (Beta)
* [Scripts] Les actifs ont désormais une propriété « ressource ».
* [Scripts] Les calques ont désormais une propriété « output\_utilisations ».

<b>Fixe :</b>

* crash [Application] lors de l’ouverture d’un fichier de projet endommagé
* crash [Application] lorsque le projet contient des ressources corrompues
* crash [Application] lors de la déconnexion d’un moniteur sous Windows
* [Application] Icône d’application incorrecte dans la barre des tâches Windows
* [Application] La corruption du fichier de configuration principal peut entraîner la suppression de fichiers
* [Application] Les panneaux apparaissent devant les fenêtres contextuelles
* [Contenu] Les générateurs de Textures ont des vignettes floues
* [Exporter] La couche d’opacité générée à partir d’une image importée casse lors de l’exportation d’un fichier .sbs/.sbsar
* [Filtres] L’agrandissement peut crash en fonction des calques d’entrée.
* [IA générative] crashs possibles lors de la réception de résultats inattendus du service
* [Scripting] Crash lors du chargement automatique d’un plug-in à partir d’une variable d’environnement
* [Scripts] crash possible lors de l’affectation de l’utilisation de la sortie avec l’API
