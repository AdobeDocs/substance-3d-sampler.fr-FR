---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/release-notes/version-4-4substance-3d-sampler.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Sampler version 4.4 pour en savoir plus sur les workflows génératifs, y compris les fonctionnalités de conversion de texte en texture et d’image en texture.
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

<b>Substance 3D Sampler 4.4</b> introduit trois nouveaux workflows génératifs en tant que version Beta : texte-texture, texte-motif et image-texture.

<b>Les fonctionnalités d&#39;IA générative sont uniquement disponibles sur la version Adobe</b>, car elle nécessite un compte Adobe. Par conséquent, ces fonctionnalités ne sont <b>pas disponibles sur Steam</b>.

*Date de publication : 23 mai 2024*

## Text-to-texture

![](../assets/textToTexture_whatNewPanel.png)

La conversion de texte en texture vous permet d&#39;explorer une nouvelle façon de créer des matériaux avec une <b>invite de texte</b>. Vous pouvez générer une texture juxtaposée à partir d’une description de texte détaillée et continuer à vous appuyer sur les résultats obtenus par l’intermédiaire du filtre Image à matière ou de n’importe quel filtre Sampler pour personnaliser les textures.

## Image-à-texture

![image à texture](../assets/imagetoText_whatNewPanel.png "image à texture")

Avec la fonction de transformation d&#39;image en texture, vous pouvez créer des textures carrées à partir de <b>votre propre image de référence</b>, qu&#39;elle soit carrée ou non carrée. Cela vous rapproche des résultats souhaités sans avoir à écrire l’invite parfaite.\
La conversion d’image en texture peut également vous aider à gagner du temps en créant des variantes à partir du contenu que vous avez déjà créé.

## Text-to-pattern

![image d&#39;illustration texte à motif](../assets/patterns_whatNewPanel.png)

La fonctionnalité Texte à motif utilisera votre <b> invite de texte</b> pour générer un motif de carreaux. Vous pouvez ensuite l’utiliser comme couleur de base avec un filtre Tissu tissé pour créer un tissu original, l’utiliser comme entrée d’un filtre Motif et plus encore !

## Note de mise à jour

*(Publié Le 23 Mai 2024)*

<b>Ajouté</b> :

* [Application] Le cache capture 3D est maintenant stocké dans un sous-dossier séparé
* [IA générative] Image en texture (Beta)
* [IA générative] Texte en motif (Beta)
* [IA générative] Texte en texture (Beta)
* [Scripts] Les actifs ont désormais une propriété « ressource ».
* [Scripts] Les calques ont désormais une propriété « output\_utilisations ».

<b>Fixe :</b>

* [Application] Blocage lors de l’ouverture d’un fichier de projet corrompu
* [Application] Blocage lorsque le projet contient des ressources corrompues
* [Application] Blocage lors de la déconnexion d’un moniteur sous Windows
* [Application] Icône d’application incorrecte dans la barre des tâches Windows
* [Application] La corruption du fichier de configuration principal peut entraîner la suppression de fichiers
* [Application] Les panneaux apparaissent devant les fenêtres contextuelles
* [Contenu] Les générateurs de texture ont des vignettes floues
* [Exporter] La couche d’opacité générée à partir d’une image importée casse lors de l’exportation d’un fichier .sbs/.sbsar
* [Filtres] L’agrandissement peut se bloquer en fonction des calques d’entrée.
* [IA générative] Blocages possibles lors de la réception de résultats inattendus du service
* [Scripts] Blocage lors du chargement automatique d’un plug-in à partir d’une variable d’environnement
* [Scripts] Blocage possible lors de l’affectation de l’utilisation de la sortie avec l’API
