---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/3d-capture/editing-3d-captured-meshes.html"
breadcrumb-title: ''
description: Apprenez à modifier des maillages capturés 3D dans Substance 3D Sampler pour affiner la géométrie, résoudre des problèmes et optimiser la qualité du maillage.
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Modification de maillages capturés 3D
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---


# Modification de maillages capturés 3D

>[!WARNING]
>
> La prise en charge de capture 3D a été supprimée à partir de la version 5.1 de Sampler.

## Modification de maillages capturés 3D

Dans ce guide de l’utilisateur, nous allons passer en revue certaines techniques de modification et de post-traitement des objets capturés en 3D dans Substance 3D Sampler.

Vous préférez visionner ce tutoriel en vidéo ? Vous le trouverez [ici.](https://youtu.be/6_EZEAR0Uy8?si=6AaCUHD6nnWZyKUE "Capture 3D avancée - Tutoriel vidéo sur le post-traitement du maillage")

![](../assets/post-processing-3d-capture.png)

Une fois que vous avez terminé le processus de Capture 3D et ajouté un filet à votre projet Sampler, vous pouvez le modifier. Il peut s&#39;agir de modifications apportées au maillage ou à la matière. Les filtres de filet sont nouveaux depuis Sampler 4.0. Les filtres Matériau utilisent tous les filtres familiers qui se trouvaient dans Sampler auparavant.

Lorsque vous modifiez un objet 3D capturé dans Sampler, <b>vous pouvez empiler les filtres Filet et Matière de manière mixte</b>, ils s’appliquent automatiquement à la partie correcte de vos données. La liste de filtres rapides ne fait pas de distinction entre les deux types.

## Filtres Filet

Examinons d’abord les filtres de filet. Il y en a deux dans Sampler : <b>transformation de maillage</b> et <b>post-traitement de maillage</b>.

<b>La transformation de filet</b> est un filtre simple qui vous permet de <b>traduire</b>, de <b>faire pivoter</b> et de <b>mettre à l’échelle</b> votre filet. Le plus souvent, vous pouvez retourner un objet ou ajuster son échelle. Toute analyse est livrée avec une transformation pré-appliquée.

<b>Le post-traitement de maillage</b> est identique à l&#39;étape de post-traitement à l&#39;issue de la boîte de dialogue Capture 3D, mais dans un filtre dynamique. Il vous permet de <b>rémailler</b> , <b>réuv</b> et <b>redessiner</b> vos textures. Ce filtre est conçu pour <b>optimiser vos maillages en réduisant le tricount, en améliorant les UV et en réduisant la texture</b>. L&#39;un des meilleurs résultats de son utilisation est l&#39;amélioration de la disposition UV. Par défaut, les sorties Capture 3D originales ont des UV très fragmentés, généralement les nouveaux UV automatiques sont une amélioration.

Il ne s’agit pas d’un filtre rapide. Chaque fois que vous modifiez un paramètre, le maillage est traité. Il est préférable de faire preuve d’un peu de patience.

## Filtres de matériau

Les filtres Matériau sont beaucoup plus variés : tout ce que vous pouvez utiliser sur des matériaux normaux peut être utilisé sur le matériau du filet de capture 3D, mais gardez à l’esprit que les résultats peuvent ne pas toujours fonctionner, car de nombreux filtres sont destinés aux matériaux de mosaïque uniforme.

Les filtres les plus utiles sont généralement les réglages comme le <b>contraste</b> lumineux, la <b>saturation de teinte</b>, ainsi que certains des filtres les plus avancés pour la modification des couches. Comme nous n’avons pas pu capturer la rugosité de notre objet, nous allons utiliser des filtres pour le faire réapparaître.

Vous pouvez utiliser un <b>filtre Saturation de teinte</b> pour que les couleurs correspondent davantage aux vraies couleurs de votre objet. Il existe de meilleures façons d’obtenir la précision des couleurs, mais elles sont beaucoup plus complexes que ce filtre rapide.

Vous pouvez ensuite restaurer les reflets qui existaient dans votre objet. Nous pouvons utiliser le <b>filtre Remplacement de couleur</b> ici. Le remplacement de couleur vous permet de prélever une couleur sur votre texture et de modifier toutes les zones contenant cette couleur.

Par défaut, tout est coloré dans la couleur que vous avez sélectionnée, mais si vous activez la <b>Segmentation avancée</b>, puis la définissez sur <b>Masquer à partir de la couleur de base</b> et <b>Remplacer</b> dans <b>Rugosité</b>, vous pouvez rendre toute la rugosité de la zone de couleur sélectionnée beaucoup plus brillante. Jouer avec la variation de luminosité et la plage de masque peut aider à affiner le masque.

Enfin, il peut être utile de récupérer quelques détails de la couleur de base dans la zone de cassure. Le <b>filtre de changement de canal</b> me permet de mélanger et de fusionner des détails entre différents canaux. Vous pouvez définir l&#39;<b>entrée sur Basecolo</b>r, la <b>sortie sur Rugosité</b>, puis jouer avec le mode de fusion et l&#39;opacité pour obtenir quelque chose d&#39;intéressant et de suffisamment proche de la réalité.

Enfin, pour mieux contrôler la rugosité finale, vous pouvez utiliser un filtre Contraste de luminosité et le définir de manière à modifier la couche de rugosité. Ensuite, vous ajustez les valeurs pour rendre la rugosité un peu plus dure.

Chaque objet est différent et, selon votre jeu de données, des réglages spécifiques peuvent être nécessaires. Vous pouvez même utiliser l&#39;<b>outil Tampon de duplication</b> pour effacer les parties de votre texture que vous souhaitez supprimer, comme les repères d&#39;aide à la capture. Gardez simplement à l’esprit que tout filtre Matériau qui utilise des emplacements spécifiques sur votre texture dépendra de votre disposition UV, de même que le traitement du filet avant tout filtre Matériau.

Une fois que vous êtes satisfait de votre objet et de vos textures, vous pouvez <b>exporter </b>votre résultat à l’aide de la boîte de dialogue <b>Partager > Exporter sous</b>. Les paramètres généraux vous permettent de choisir le nom et le chemin, les paramètres de maillage vous permettent de choisir le format de maillage 3D et les paramètres de matière vous permettent de configurer le matériau du maillage. Vous pouvez désactiver le maillage ou la matière pour n’exporter qu’une seule d’entre elles individuellement. Une fois exporté, votre filet est prêt à être utilisé dans d’autres applications 3D.
