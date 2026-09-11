---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/3d-capture/camera-settingsfocussubstance-3d-sampler.html"
breadcrumb-title: ''
description: Découvrez comment configurer les paramètres de mise au point de caméra dans Substance 3D Sampler pour une qualité Capture 3D et une netteté d’image optimales.
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Focus sur les paramètres de caméra
user-guide-description: ''
user-guide-title: ''
source-git-commit: 6cc0519fb8c0f74fa805691ec4adb9e449a627d5
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---


# Focus sur les paramètres de caméra

>[!WARNING]
>
> La prise en charge de capture 3D a été supprimée à partir de la version 5.1 de Sampler.

## Paramètres de caméra - Focus

<b>Ouverture</b> étant le paramètre de caméra le plus complexe, nous l&#39;expliquerons dans la profondeur de ce guide de l&#39;utilisateur.

Vous préférez regarder ce guide sous forme de tutoriel vidéo ? Vous le trouverez [ici](https://youtu.be/kFZ71ZWuap0?si=MDuvyO9w96rFpsQ9 "ouverture et mise au point pour le tutoriel vidéo Capture 3D").

![](../assets/focus-manually-3d-capture.png)

## Mise au point d’un objectif

Par défaut, le système de mise au point automatique de votre caméra contrôle cette opération, en définissant la mise au point automatiquement. C&#39;est logique lorsque vous photographiez des personnes, de grands environnements ou tout ce qui est dynamique, mais pour notre sujet contrôlé et statique, cela peut même causer des problèmes ; la mise au point automatique peut faire des erreurs et gâcher une photo, même entre deux prises de vue.

Chaque reflex numérique peut passer de la mise au point automatique à une mise au point <b>manuelle</b> complète. Cela signifie que vous contrôlez entièrement la mise au point, en tournant la bague de mise au point sur l&#39;objectif. De cette façon, vous êtes sûr que la mise au point ne passera pas d’un plan à l’autre. Si vous lisez le mode d’emploi de la caméra, il y aura probablement des réglages pour vous aider, comme « focus peaking », où un effet coloré est dessiné sur l’écran de la caméra. Cela permet de voir quelle partie de l’image est mise au point. Il peut même y avoir un zoom-agrandisseur, où l’affichage montre une petite partie de la vue actuelle agrandie, ce qui vous permet d’obtenir une mise au point parfaite en pixels. Cet agrandisseur est particulièrement important pour vous aider à vous concentrer.

L&#39;utilisation de la mise au point manuelle vous aidera à voir et à mieux comprendre ce qui se passe avec votre <b> ouverture</b> et votre <b>mise au point</b>. L&#39;inconvénient est que vous devez <b>réajuster votre mise au point chaque fois que votre caméra ou votre sujet bouge</b>. Il est facile d’oublier et de gâcher une photo. Il est donc préférable de prendre l’habitude de vérifier.

## Choix de la valeur d’ouverture

L&#39;<b>Ouverture</b> est délicate, car elle affecte la <b>mise au point</b> et la <b>netteté</b>. Nous ne voulons pas que des parties de notre sujet ne soient pas nettes, cela pose des problèmes pour le processus de photogrammétrie. Cela signifie qu&#39;une ouverture importante, généralement entre f1,8 et f3,5 pour les objectifs standards, sera un problème. D&#39;un autre côté, si l&#39;on recherche la plus petite ouverture possible, f/32 n&#39;est pas non plus génial, les choses sont également moins nettes de ce côté, et la quantité de lumière qui entre est minuscule, ce qui entraîne des problèmes de sous-éclairage.

Bien que la profondeur de champ s’élargisse avec des ouvertures plus petites, elle s’adapte également en fonction de la distance focale. Cela signifie que vous aurez plus de profondeur de champ de près, et beaucoup moins, jusqu’à la netteté complète, plus loin. Cela peut être problématique pour les petits objets, si vous voulez qu’ils prennent la plus grande partie de la photo.

Quelle est donc la bonne valeur ouverture ? En règle générale, déterminez la plage d’ouverture la plus nette pour votre objectif et commencez par cette valeur. C&#39;est probablement<b> F8 ou f11, jusqu&#39;à f16</b>.  Vérifiez si <b>tout est net</b>. Si ce n&#39;est pas le cas, réduisez étape par étape jusqu&#39;à ce que f20 environ soit actif. Si votre objet n’est toujours pas entièrement net, essayez de vous éloigner un peu plus de lui. Même une distance de 10 à 15 cm peut faire une différence pour les petits objets.

Gardez également à l’esprit que le choix de l’objectif peut faire une différence. Les objectifs en kit par défaut fournis avec une caméra ne sont généralement pas de la meilleure qualité, et il peut être intéressant d&#39;investir dans un objectif de meilleure qualité. Les objectifs macro peuvent être utiles, en particulier pour les gros plans, car ils permettent de faire la mise au point beaucoup plus près de l&#39;objectif.

## Mise au point entre crochets

Il y a une astuce spéciale que vous pouvez faire, pour obtenir une netteté parfaite lorsque tout le reste échoue. Le <b>bracketing de mise au point</b> signifie que vous prenez <b>plusieurs photos</b>, à <b>différentes distances de mise au point</b>, et que vous les associez dans Photoshop. Il nécessite <b>beaucoup de travail supplémentaire</b>, en particulier avec les séries en boucle complète. Il ne doit donc être utilisé qu&#39;en dernier recours.

Si vous avez au moins deux photos avec une mise au point différente, chargez-les dans différents calques.

![](../assets/focus-differences-3d-capture.png)

Sélectionnez tous les calques, puis accédez à <b>Modifier</b> > <b>Alignement automatique des calques</b>. Appuyez sur OK avec les paramètres par défaut. Photoshop tente d’aligner parfaitement tous les calques sélectionnés sur un pixel

Accédez ensuite à <b>Modifier</b> > <b>Calques de Fusion automatique</b>. Ici encore, choisissez OK avec tous les paramètres par défaut. Photoshop va fusionner les parties les plus nettes de vos calques.

Si tout s&#39;est bien passé, vous avez maintenant une photo parfaitement nette. Pour gagner du temps, il est judicieux de transformer certaines de ces étapes en actions enregistrées.

Maintenant que vous avez appris tout ce qu&#39;il y a à savoir sur l&#39;Ouverture et la mise au point pour le processus de Capture 3D, découvrez [comment créer une configuration d&#39;éclairage idéale](3d-capture-lighting-substance-3d-sampler.md).
