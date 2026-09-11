---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/3d-capture/editing-3d-captured-meshes.html"
breadcrumb-title: ''
description: Apprenez à modifier des maillages 3D capturés dans Substance 3D Sampler pour affiner la géométrie, résoudre des problèmes et optimiser la qualité des maillages.
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

Vous préférez visionner ce tutoriel en vidéo ? Vous le trouverez [ici.](https://youtu.be/6_EZEAR0Uy8?si=6AaCUHD6nnWZyKUE "Capture 3D avancée - Tutoriel vidéo sur le post-traitement Maillage")

![](../assets/post-processing-3d-capture.png)

Une fois que vous avez terminé le processus de Capture 3D et ajouté un maillage à votre projet Sampler, vous pouvez le modifier. Il peut s’agir de modifications apportées au maillage ou au matériau. Les filtres Maillage sont nouveaux depuis Sampler 4.0. Les filtres de matériau utilisent tous les filtres habituels de Sampler.

Lorsque vous modifiez un objet 3D capturé dans Sampler, <b>vous pouvez effectuer une pile mixte du Maillage et des Filtres de matériau</b>, qui s’appliquent automatiquement à la partie correcte de vos données. La liste de filtres rapides ne fait pas de distinction entre les deux types.

## filtres de maillage

Examinons d’abord les filtres de maillage. Il y en a deux dans Sampler : <b>Transforme de maillage</b> et <b>post-traitement de maillage</b>.

Le <b>transforme de Maillage</b> est un filtre simple qui vous permet de <b>translater</b>, de <b>faire pivoter</b> et de <b>redimensionner</b> votre maillage. Le plus souvent, vous pouvez retourner un objet ou ajuster son échelle. Toute numérisation est livrée avec un transforme pré-appliqué.

Le <b>post-traitement de Maillage</b> est identique à l&#39;étape de post-traitement à la fin de la boîte de dialogue Capture 3D, mais dans un filtre dynamique. Il vous permet de <b>réengrener</b> , <b>réutiliser</b> et <b>refaire</b> vos textures. Ce filtre est conçu pour <b>optimiser vos maillages en réduisant le tricount, en améliorant les UV et en réduisant la texture d&#39;échelle</b>. L’un des meilleurs résultats de son utilisation est l’amélioration de la disposition des UV. Par défaut, les sorties Capture 3D originales ont des UV très fragmentés, généralement les nouveaux UV automatiques sont une amélioration.

Il ne s’agit pas d’un filtre rapide. Chaque fois que vous modifiez un paramètre, le maillage est traité. Il est préférable de faire preuve d’un peu de patience.

## Filtres de matériau

Les filtres de matériau sont beaucoup plus variés. Tout ce que vous pouvez utiliser sur des matériaux normaux peut être utilisé sur le matériau du maillage capture 3D, mais gardez à l’esprit que les résultats peuvent ne pas toujours fonctionner, car de nombreux filtres sont destinés à des matériaux de répétition uniformes.

Les filtres les plus utiles sont généralement les réglages comme le <b>contraste</b> lumineux, la <b>saturation de teinte</b>, ainsi que certains des filtres les plus avancés pour la modification des couches. Comme nous n’avons pas pu capturer la rugosité de notre objet, nous allons utiliser des filtres pour le faire réapparaître.

Vous pouvez utiliser un <b>filtre Saturation de teinte</b> pour que les couleurs correspondent davantage aux vraies couleurs de votre objet. Il existe de meilleures façons d’obtenir la précision des couleurs, mais elles sont beaucoup plus complexes que ce filtre rapide.

Vous pouvez ensuite restaurer les reflets qui existaient dans votre objet. Nous pouvons utiliser le <b>filtre Remplacement de couleur</b> ici. Le Remplacement de couleur vous permet de prélever une couleur sur votre texture et de modifier toutes les zones contenant cette couleur.

Par défaut, tout est coloré dans la couleur que vous avez sélectionnée. Toutefois, si vous activez la <b>segmentation avancée</b>, puis la définissez sur <b>Masquer à partir de la couleur de base</b> et <b>Remplacer</b> dans <b>Rugosité</b>, vous pouvez rendre toute la rugosité de la zone de la couleur sélectionnée beaucoup plus brillante. Jouer avec la variation de luminosité et la plage de masque peut aider à affiner le masque.

Enfin, vous voudrez peut-être récupérer un peu de détails de la couleur de base dans la rugosité. Le <b>filtre de changement de canal</b> me permet de mélanger et de fusionner des détails entre différents canaux. Vous pouvez définir l&#39;<b>entrée sur Basecolo</b>r, la <b>sortie sur Rugosité</b>, puis jouer avec le mode Fusion et l&#39;opacité pour obtenir quelque chose d&#39;intéressant et de suffisamment proche de la réalité.

Enfin, pour mieux contrôler la rugosité finale, vous pouvez utiliser un filtre Contraste de luminosité et le définir de manière à modifier la couche de rugosité. Ensuite, vous modifiez les valeurs pour rendre la rugosité un peu plus pointue.

Chaque objet est différent et, selon votre jeu de données, des réglages spécifiques peuvent être nécessaires. Vous pouvez même utiliser l&#39;<b>outil Tampon de Clone</b> pour effacer les parties de votre texture que vous souhaitez supprimer, comme les repères d&#39;aide à la capture. Gardez à l&#39;esprit que tout filtre de matériau qui utilise des emplacements spécifiques sur votre texture dépendra de la disposition de votre UV. Le traitement du maillage avant tout filtre de matériau doit donc être effectué.

Une fois que vous êtes satisfait de votre objet et de vos textures, vous pouvez <b>exporter </b>votre résultat à l’aide de la boîte de dialogue <b>Partager > Exporter sous</b>. Les paramètres généraux vous permettent de choisir le nom et le chemin, les paramètres de Maillage vous permettent de choisir le format de Maillage 3D et les paramètres de matériau vous permettent de configurer le matériau du maillage. Vous pouvez désactiver l’option maillage ou matériau pour exporter un seul fichier individuellement. Une fois exporté, votre maillage peut être utilisé dans d’autres applications 3D.
