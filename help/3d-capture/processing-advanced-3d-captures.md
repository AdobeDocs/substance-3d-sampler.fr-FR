---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/3d-capture/processing-advanced-3d-captures.html"
breadcrumb-title: ''
description: Découvrez comment traiter des captures 3D avancées dans Substance 3D Sampler pour optimiser la géométrie, les textures et la qualité de la matière.
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Traitement des captures 3D avancées
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '1339'
ht-degree: 0%

---


# Traitement des captures 3D avancées

>[!WARNING]
>
> La prise en charge de capture 3D a été supprimée à partir de la version 5.1 de Sampler.

## Traitement des captures 3D avancées dans Substance 3D Sampler

Dans ce guide de l’utilisateur, nous examinons dans la profondeur le traitement de vos jeux de données capture 3D dans Substance 3D Sampler.

Vous préférez visionner ce tutoriel en vidéo ? Vous le trouverez [ici](https://youtu.be/vJQ756Up55Y?si=GiAnajXRGkb5gyTH "Capture 3D avancée - Tutoriel sur le traitement de capture").

![](../assets/cloud-points-3d-capture.png)

Lors de la Capture 3D ou de la photogrammétrie, la plupart des efforts sont consacrés à la prise de bonnes photos, étapes abordées dans les articles précédents du guide de l’utilisateur. Gardez également à l’esprit que nous avons conçu et ciblé l’expérience de Capture 3D pour les objets jusqu’à la taille humaine. Vous risquez de rencontrer des problèmes lorsque vous utilisez un très grand ensemble de données (c’est-à-dire supérieur à 6 Giga pixels, soit 500 photos de 12 mégapixels).

## Démarrage du processus capture 3D

Pour commencer à utiliser Sampler, vous devez créer un <b>nouveau projet</b>. Vous remarquerez la nouvelle section Objets 3D dans la fenêtre Projets. Cliquez sur le signe + en regard de cela, puis sélectionnez « <b>Nouvel objet 3D</b> » pour commencer le processus de capture 3D dans une nouvelle fenêtre dédiée.

![](../assets/new-capture-3d-capture.png)

Sélectionnez toutes vos photos dans l’explorateur et faites-les glisser dans la fenêtre capture 3D. Après un certain temps de chargement, vos photos sont présentées dans une liste et une galerie, avec les propriétés de la sélection à droite.

La liste des groupes de photos sur la gauche est basée sur l’appareil photo et l’objectif utilisés pour les photos. Si vous mélangez des photos à partir de plusieurs appareils, tels qu&#39;un téléphone portable, un appareil photo reflex numérique ou un drone, vous obtiendrez <b>des groupes distincts</b> ici.

Lorsque le groupe est sélectionné, vous obtenez un aperçu de ses propriétés. Parfois, la <b>Distance focale</b> et la <b>taille du capteur</b> sont absentes ; il est possible de les remplir <b>manuellement</b> si nous connaissons les chiffres. Ces informations peuvent aider à améliorer un peu le traitement.

## Génération de masques

L&#39;option la plus importante se trouve sous la section <b>Masque</b>. Comme les photos ont été prises sur une platine, l&#39;arrière-plan n&#39;a pas beaucoup changé, mais l&#39;objet a changé. Cela peut entraîner l’échec complet du processus d’alignement. En plus de cela, l&#39;arrière-plan ne contient aucune information significative. Pour résoudre ce problème, vous devrez masquer le sujet de chaque photo.

Le moyen le plus simple est d&#39;utiliser la génération automatique de lots. Sélectionnez <b>Générer</b>, puis <b>Nouveau lot</b> et attendez que Sampler ait créé les masques. Cela utilise la technologie « Sélectionner un sujet » d’Adobe Sensei, tout comme dans Photoshop. Avec 72 photos, ce processus prend un peu de temps, il est donc préférable d&#39;être patient.

![](../assets/generate-mask-3d-capture.png)

Vous pouvez vérifier un masque individuel en <b>sélectionnant une photo</b> et en cliquant sur l&#39;<b>icône en forme d&#39;œil</b> en bas à droite, à côté du tracé du masque. Cela montre un aperçu en niveaux de gris du masque. Si le masquage automatique fait une erreur et conserve des parties de l’arrière-plan, ne vous inquiétez pas, quelques masques incorrects ne posent pas de problème.

La majorité des masques doivent avoir votre sujet. C&#39;est pourquoi il est essentiel de prendre vos photos sur un <b>arrière-plan uniforme et uni</b>. Le masquage automatique fonctionne beaucoup plus facilement. Si la plupart de vos masques ne sont pas corrects, vous pouvez soit les corriger tous manuellement, soit retoucher vos photos avec un arrière-plan plus adapté.

Vous pouvez réessayer un jeu de données plusieurs fois et éviter de générer à nouveau vos masques à chaque fois, car Sampler les supprime une fois l’application fermée. Vos masques sont mis en cache dans Documents\Adobe\Adobe Substance 3D Sampler\3DCapture\p1. Si vous effectuez plusieurs ressources dans une session, vous obtiendrez des dossiers appelés p2, p3, etc. Il est conseillé de <b>copier les masques mis en cache dans un emplacement sûr avec votre jeu de données</b>, afin de gagner du temps si vous devez revoir ce jeu de données.

## Alignement

Lorsque les masques sont corrects, vous êtes prêt à passer à l’alignement. Appuyez sur le <b>bouton bleu d&#39;envoi</b> en haut à droite. Vous aurez deux options : <b>Précision</b> et <b>Commande de photos</b>.

* La <b>précision</b> peut améliorer l&#39;alignement. Il est préférable de commencer à faible, si vous obtenez des photos en échec, réessayez avec une valeur élevée.
* L&#39;<b>ordre des photos</b> est lié à l&#39;ordre dans lequel vous avez pris vos photos. Si vous vous êtes promené autour d’un objet et que vous avez filmé en spirale, vous pouvez utiliser la séquence pour gagner du temps. Toutefois, l’option la plus sûre est généralement celle par défaut, même si l’alignement peut prendre un peu plus de temps.

Cliquez sur <b>Traiter</b> et attendez la fin de l&#39;alignement. Cela peut prendre plusieurs minutes, alors il est préférable d&#39;être patient à nouveau. Une fois l’opération terminée, un nuage de points représentant votre objet s’affiche, chaque photo étant représentée par un appareil photo flottant autour de lui. Un triangle d&#39;avertissement orange en haut à gauche signifie que certaines photos n&#39;ont <b>pas pu s&#39;aligner</b>. Réessayez avec une précision de haute qualité et une commande par défaut si ce n’est pas déjà fait. Certaines photos peuvent ne pas s’aligner, ce qui signifie qu’il n’y a pas assez de chevauchement ou de détails dans les photos. Vous devrez peut-être revoir votre processus de photographie pour résoudre ce problème, ou vous pouvez simplement les ignorer s&#39;il ne s&#39;agit que de quelques photos.

En examinant vos données de nuage de points, vous pouvez voir <b>des points parasites flotter autour de votre objet</b> qui ne sont pas censés en faire partie. Cela est généralement dû à un mauvais masquage. Dans ce cas, quelques mauvais masques ont provoqué la capture de particules de dust. Vous pouvez <b>les recadrer</b> à l&#39;aide de l&#39;icône en forme d&#39;œil à droite, en regard de Zone d&#39;intérêt. Il vous suffit de <b>déplacer les poignées carrées</b> qui semblent mieux s&#39;ajuster autour de votre objet. Tous les points en dehors de cette zone, en gris foncé, ne seront pas inclus dans votre modèle 3D final. Vous pouvez également utiliser ce cadre de sélection pour <b>faire pivoter au préalable et mieux aligner votre modèle.</b>

Les nuages de points ont parfois des points plus denses que les autres. Cela ne pose pas de problème, car moins de points signifie que la surface aura moins de petits détails géométriques. Elle provient d’un manque de détails et de contraste dans certaines parties de l’objet, tandis que d’autres ont plus de détails.

## Détails géométriques

Il ne reste qu’un seul paramètre avant de créer notre filet. Sous Détails de la géométrie (geometry details), vous pouvez sélectionner le niveau de détail de géométrie initial.

* <b>Brut</b> est le <b>mème non décimé</b>h, il n&#39;est pas vraiment recommandé de l&#39;utiliser, sauf si vous êtes sûr d&#39;en avoir besoin.
* <b>Les </b> sont des <b>maillages décimés</b>. Choisissez des options inférieures pour obtenir un résultat de test plus rapidement, des options supérieures pour obtenir plus de détails au détriment d&#39;un traitement plus lent.

Appuyez sur <b>Envoyer pour commencer le traitement du maillage</b>. Ce processus peut prendre un certain temps, plus long que les étapes précédentes.

## Aperçu et post-traitement

Une fois votre maillage terminé, la dernière fenêtre nous permet de prévisualiser et de post-traiter notre maillage avant de l’ajouter à notre projet Sampler. Ce mode comporte quelques boutons en bas pour voir votre filet avec une <b>texture</b>, un <b>solide ombré</b>, de la <b>structure filaire</b> et un <b>matériau anti-UV</b>. Les paramètres de post-traitement sur le côté vous permettent de générer une nouvelle version de votre filet. Cela signifie un filet réassemblé, avec de nouveaux UV automatiques, et une texture cuite à partir du filet d’origine. Les commandes principales vous permettent de définir un nombre de visages cible et d’activer/désactiver la cuisson normale, height et AO. Il existe de nombreux paramètres avancés à modifier, mais les valeurs par défaut fonctionnent généralement correctement.

Vous pouvez également effectuer cette étape de traitement du filet par la suite, une fois le filet ajouté à Sampler. Une fois que vous l’avez ajouté à Sampler, vous pouvez lui donner un nom ; il apparaît désormais dans votre liste de projets.

Vous pouvez modifier le maillage et les textures, mais vous pouvez déjà exporter votre résultat à l&#39;aide de l&#39;<b>option Partager</b> Boîte de dialogue > <b>Exporter sous</b>. Les <b>paramètres généraux</b> vous permettent de choisir le nom et le chemin, les <b>paramètres de filet</b> vous permettent de choisir le format de filet 3D et les <b>paramètres de matière</b> vous permettent de configurer le matériau du filet. Vous pouvez désactiver le maillage ou la matière pour n’exporter qu’une seule d’entre elles individuellement. Une fois exporté, votre filet est prêt à être utilisé dans d’autres applications 3D.

Découvrez maintenant comment [modifier davantage vos maillages 3D capturés dans Sampler](editing-3d-captured-meshes.md).
