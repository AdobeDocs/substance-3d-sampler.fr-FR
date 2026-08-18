---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/3d-capture/cross-polarising-for-3d-capturesubstance-3d-sampler.html"
breadcrumb-title: ''
description: Apprenez à utiliser les techniques de polarisation croisée dans Substance 3D Sampler pour réduire les reflets et améliorer la qualité de la Capture 3D.
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Polarisation croisée pour capture 3D
user-guide-description: ''
user-guide-title: ''
source-git-commit: 6cc0519fb8c0f74fa805691ec4adb9e449a627d5
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---


# Polarisation croisée pour capture 3D

>[!WARNING]
>
> La prise en charge de capture 3D a été supprimée à partir de la version 5.1 de Sampler.

## Polarisation Croisée

Dans ce guide de l’utilisateur, nous allons apprendre à gérer les objets réfléchissants et les problèmes qu’ils provoquent, et à utiliser la polarisation de la lumière pour résoudre ce problème.

Vous préférez en savoir plus sur ce sujet dans un tutoriel vidéo ? Cliquez [ici](https://youtu.be/VWsbP56MDk0?si=Hdp7vblJB6L1RPxK "Tutoriel sur la polarisation croisée").

![](../assets/polarized-lens-3d-capture.png)

Lorsque la lumière atteint une surface, elle se reflète généralement de manière diffuse, rebondissant uniformément, donnant à la surface son aspect coloré. Mais selon la rugosité de la surface, une partie de la lumière peut être réfléchie directement vers votre œil ou votre appareil photo. Ce <b>reflet de specular</b> change en fonction de votre angle de vue.

La photogrammétrie fonctionne en alignant les motifs visuels et les éléments entre les photos. Elle part du principe que l’aspect d’un objet ne changera pas entre chaque photo consécutive. Donc, la réflexion au specular est un effet indésirable ici. Un objet de boîtier léger peut avoir juste un revêtement réfléchissant, mais les objets qui sont en métal peuvent être beaucoup plus délicats et nécessitent plus d&#39;efforts pour être résolus. Nous aborderons le cas léger dans ce guide de l’utilisateur. Il nous suffit de capturer une couleur de base parfaite, préservée des hautes lumières du specular. Il est facile de rajouter la réflectivité en 3D une fois capturée.

Pour résoudre ce problème, nous pouvons filtrer nos réflexions de specular à l&#39;aide d&#39;une méthode appelée <b>polarisation croisée</b>. Lorsque la lumière est polarisée, toutes les ondes sont orientées dans la même direction. Si vous le polarisez à nouveau, dans une direction perpendiculaire, il est complètement bloqué, ce qui le rend invisible.

La polarisation affecte principalement la lumière du specular, car il s’agit de rayons lumineux focalisés, qui se déplacent dans une direction spécifique, par opposition à la lumière diffuse dispersée que nous voulons conserver.

Vous pouvez polariser la lumière à l’aide d’un filtre polarisant, une feuille transparente spéciale qui filtre les ondes. Ils se présentent sous de nombreuses formes, nous utiliserons des filtres en verre à vis pour vos objectifs, ainsi que des feuilles de film polarisantes de style bricolage

L&#39;idée de base est de <b>ajouter un filtre à votre lumière</b> et à <b>votre objectif</b>, et de les configurer pour qu&#39;ils soient <b>perpendiculaires les uns aux autres</b>. Cela signifie que vous devrez affiner l’orientation des filtres en les faisant pivoter. Une fois configurés, les reflets de specular de cette lumière deviennent invisibles. C’est assez spécial à voir. Déformer vos filtres peut soudainement éliminer complètement tous les reflets d’une lumière polarisée.

![](../assets/polarizing-before-after-3d-capture.png)

Un filtre polarisant pour votre objectif doit être acheté, car vous voulez un optique optimal, tout en permettant des photos nettes et claires. Les différents objectifs ont des tailles de filetage différentes pour visser les filtres, alors assurez-vous d’en choisir un qui convient à votre objectif, ou plusieurs tailles pour plusieurs objectifs si vous faites des essais.

La polarisation de vos lumières est moins coûteuse et plus simple :<b> feuilles de film polarisantes</b> sont relativement peu coûteuses. Vous pouvez utiliser une feuille entière ou en découper des morceaux. Il est conseillé de couper des morceaux circulaires couvrant toute la lumière, car il est plus facile de les faire pivoter. Certaines lumières sont meilleures pour cela, elles peuvent avoir un petit porte-filtre, ou des aimants pour maintenir les feuilles en place. Sinon, le ruban adhésif fonctionne toujours !

Assurez-vous d&#39;<b>ajouter le polariseur après tous les diffuseurs</b>, car la diffusion de la lumière annule toute polarisation.

La plupart des flashes en anneau moins chers se vissent dans votre fente de filtre et peuvent ne plus vous permettre de fixer un filtre d&#39;objectif. Ils n’ont aucun moyen d’attacher des filtres de polarisation à la lumière du flash elle-même. Vous devrez donc créer les vôtres. Seuls les modèles haut de gamme le prennent en charge correctement.

<b>Les polariseurs rotatifs et correspondants dans votre configuration doivent être effectués en permanence</b>. Votre filtre d’objectif doit être entièrement perpendiculaire à toutes vos lumières. Pour ce faire, la seule façon est de regarder l’écran de votre appareil photo et de régler les choses. J’aime commencer par coller une seule feuille sur mon flash, puis ajuster le filtre de mon objectif pour bloquer les reflets du flash. Pour ce faire, il suffit de prendre une photo ou de faire chauffer le flash à sec. C&#39;est un peu compliqué, vous pouvez marquer la bonne orientation sur votre filtre d&#39;objectif avec un marqueur, puis essayer de ne plus toucher l&#39;objectif et le filtre flash.

Le réglage de la polarisation des lumières vidéo est différent, mais plus facile. Vous devrez constamment régler les lumières lorsque vous les déplacez ou lorsque vous réglez l’height de l’appareil photo. Il vous suffit de <b>faire pivoter la feuille jusqu&#39;à ce qu&#39;elle apparaisse parfaitement sur l&#39;écran de votre appareil photo</b>.

<b>Chaque source lumineuse qui apparaît dans les reflets doit être polarisée</b>. Vous devrez donc peut-être fermer les fenêtres ou éteindre les écrans.

Lorsque vous êtes correctement configuré, vous devriez être en mesure de capturer un objet comme s’il était complètement mat, sans reflets ni éclairage. Tout comme le fait de voir votre filet avec seulement la texture de couleur de base appliquée, il vous permet de capturer des objets réfléchissants difficiles.

Découvrez maintenant en détail [comment traiter votre Capture 3D à l&#39;aide de Substance 3D Sampler](processing-advanced-3d-captures.md) !
