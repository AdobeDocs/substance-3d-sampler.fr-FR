---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/tools/auto-tiling.html"
breadcrumb-title: ''
description: Utilisez l’outil Mosaïque automatique de Substance 3D Sampler pour créer automatiquement des motifs de mosaïque homogènes à partir de textures à l’aide de la technologie d’IA.
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mosaïque automatique
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 0%

---


# Limites automatiques

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-tiling-18-n-d.png)

Outils **In:**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Le <b>filtre Mosaïque automatique</b> recherche les structures répétitives dans votre matériau et les utilise pour créer un matériau de mosaïque. Contrairement au <b>filtre Créer un carreau</b> ou au <b>filtre Carrelage</b>, le <b>carrelage automatique</b> se concentre sur l&#39;isolation de la plus petite zone de matière qui peut être réalisée sur le carreau.

<b>Le carrelage automatique </b> est particulièrement utile pour les textiles.

</td>
</tr>
</table>

>[!NOTE]
>
> Pour que le filtre Limites automatiques fonctionne, un minimum de 3x3 répétitions est requis dans l’image ou le matériau source.

## Tutoriel sur le filtre Mosaïque automatique

## À propos de la mosaïque automatique

Lorsque vous l&#39;ajoutez à votre pile de calques, <b>Mosaïque automatique</b> tente de trouver automatiquement des motifs répétitifs et de générer un matériau de mosaïque. Si cela ne fonctionne pas, vous pouvez utiliser le bouton <b>Paramètres avancés</b> pour ajuster manuellement le processus.

Si vous envisagez de créer un matériau de mosaïque à partir d&#39;une image, il est préférable d&#39;utiliser d&#39;abord le <b>filtre Mosaïque automatique</b>, puis le <b>filtre Image vers matériau</b>.

La <b>juxtaposition automatique</b> s&#39;exécute entièrement sur votre appareil, aucun contenu n&#39;est envoyé vers le cloud.

## Paramètres

Contrairement à la plupart des filtres, la <b>juxtaposition automatique</b> n&#39;a pas de paramètres. À la place, il existe un bouton <b>Paramètres avancés </b>, qui vous guidera tout au long du processus de configuration du filtre. Vous n’avez pas besoin d’effectuer de réglages manuels à chaque étape. Vous pouvez aller vers l’avant ou vers l’arrière en sélectionnant une étape en haut de la fenêtre.

Ce processus comprend les étapes suivantes :

1. <b>Introduction</b> : explique le fonctionnement du filtre. Utilisez la case à cocher pour masquer cet écran à l’avenir.
1. <b>Sélection du mappage</b> : sélectionnez le canal que le filtre doit utiliser. Il est recommandé d’utiliser la couche présentant le motif répétitif le plus visible. Il s’agit généralement de la couche de couleur de base ou de la couche Height, mais d’autres couches peuvent être utiles en fonction de votre matière.
1. <b>Exemples de paramètres</b> : modifiez le matériau d&#39;entrée afin d&#39;obtenir les meilleurs résultats. Cela inclut le choix d’une résolution et la rotation ou la déformation de l’entrée. Si votre motif est très petit, il peut être utile de sélectionner une résolution plus élevée pour s’assurer qu’il est visible. Toutefois, pour les motifs plus volumineux, une résolution plus faible peut fournir des résultats meilleurs et plus rapides.
1. <b>Taille du motif</b> : à cette étape, le filtre recherche le plus petit motif possible. Vous pouvez choisir entre une détection automatique plus grande ou plus petite, ou sélectionner une taille personnalisée pour spécifier votre propre taille. Pour obtenir de meilleurs résultats, sélectionnez la plus petite taille pour laquelle le motif est répété une fois par boîte.\
   Si les cases sont toutes de forme irrégulière et ne semblent pas correspondre au motif, utilisez la taille personnalisée pour essayer d’obtenir des résultats plus réguliers.
1. <b>Détection de motif</b> : positionnez les points de sorte que chaque point se trouve au même emplacement dans le motif. Par exemple, dans un motif à damier noir et blanc, vous pouvez souhaiter que les points soient au centre des carrés noirs.
1. <b>Zone d&#39;intérêt</b> : sélectionnez la zone du matériau à utiliser pour créer le motif final. L’utilisation d’une zone plus grande permet de réduire la quantité de répétition visible, mais l’inclusion de zones avec des artefacts ou des différences d’éclairage visibles peut augmenter la quantité de répétition visible.
1. <b>Suppression de couture</b> : ajustez les paramètres pour minimiser la visibilité des coutures. Le paramètre <b>Couper le smoothness </b> contrôle la fluidité de la ligne de la couture, tandis que le paramètre <b>Largeur de fusion </b> brouille la couture entre les carreaux.

Une fois toutes les étapes effectuées, utilisez <b>Appliquer</b> pour confirmer vos choix. Le filtre <b>Limites automatiques</b> traitera le matériau pour générer un résultat final.
