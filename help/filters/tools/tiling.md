---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/tools/tiling.html"
breadcrumb-title: ''
description: Utilisez l’outil Mosaïque de Substance 3D Sampler pour créer des motifs de mosaïque continus à partir de textures pour des surfaces matérielles répétables.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Tiling
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Répétition
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 0%

---


# Répétition

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-tiling-18-n-d.png)

Outils **In:**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Utilisez le **filtre Juxtaposition** pour rendre votre matière juxtaposable. Le filtre **Mosaïque** rend également votre matériau mosaïque, mais chaque filtre fonctionne de manière différente. Si le **filtre Juxtaposition** ne fonctionne pas pour vous, essayez le **filtre Juxtaposition**.

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Afficher la couture** : activer/désactiver\
  Choisir d’afficher ou non la couture
* **Utiliser le masque** : activer/désactiver\
  Si cette option est activée, vous pouvez créer un masque personnalisé pour contrôler l’emplacement des coutures
  * **Masque** : image/pinceau\
    Importez une image à utiliser comme masque ou utilisez le pinceau pour peindre un masque directement dans la **vue 2D**

**Edge**

* **Détecter les contours** : activer/désactiver\
  Indiquez si les bords doivent être détectés en fonction des canaux du matériau pour créer une transition plus organique entre les calques de matériau. Si cette option est activée, les paramètres supplémentaires suivants apparaissent :
  * **Utiliser le seuil par canal** : activer/désactiver\
    Si cette option est activée, des paramètres supplémentaires apparaissent pour ajuster le seuil de chaque couche individuellement.
    * **Couleur de base du seuil** : 0-1
    * **Seuil normal** : 0-1
    * **Height du seuil** : 0-1
  * **Seuil** : 0-1\
    Ajustez la valeur de seuil utilisée pour rechercher la couture.
  * **Flou** : 0-1\
    Atténuation de la zone autour de la couture
  * **Smoothness** : 0-2\
    Ajustez le smoothness de la couture. Cela permet d’éviter les artefacts
  * **Résolution de la grille** : 1-11\
    Ajustez la résolution de la grille sur laquelle la couture est dessinée. Une résolution inférieure peut améliorer les performances, mais diminuer la qualité de la couture
  * **Utiliser la couleur de base** : activer/désactiver\
    Indiquer si les informations de couleur de base sont prises en compte dans la génération de la jointure
  * **Utiliser la normale** : activer/désactiver\
    Indiquer si les informations normales sont prises en compte dans la génération de jointures
  * **Utiliser l&#39;Height** : activer/désactiver\
    Indiquer si les informations d&#39;height sont prises en compte dans la génération de couture
  * **Décalage de coupe** : 0-0,5\
    Ajuster le décalage de la couture sur les axes X et Y

**Paramètres avancés**

* **Transformation** : 0-2\
  Réglez les valeurs de transformation de la matrice. Augmentez les valeurs X et W pour ajuster le degré de chevauchement entre le matériau sous-jacent et celui sous-jacent.
* **Décalage** : 0-1\
  décaler la matière sur les axes X et Y
* **Filtrage** :\
  Sélectionnez la méthode de filtrage à utiliser sur les pixels redimensionnés. Le filtrage bilinéaire applique un flou aux pixels, tandis que le filtrage le plus proche préserve le contour net entre les pixels.
* **Taille d&#39;entrée** : 0-8192\
  Ajustez la taille de l’entrée en pixels sur les axes X et Y.

## Guide d’utilisation

Le filtre **Limites** fonctionne en deux étapes :

1. Il redimensionne et décale votre matière pour générer un chevauchement.
1. Ensuite, il fait varier le bord qui se chevauche pour masquer la couture.

Pour utiliser le **filtre Mosaïque**, vous pouvez donc ajuster ces deux parties du processus afin d&#39;obtenir les meilleurs résultats.

1. Ajoutez le **filtre Limites** en haut de la pile de calques
1. Utilisez les poignées pour transformer le matériau afin qu&#39;il y ait suffisamment de chevauchement pour masquer la couture.
   1. La mise à l’échelle de la matière peut être utile pour créer un chevauchement, mais elle peut également entraîner une perte de détails.
1. Ajustez les paramètres dans la section **Bord** pour ajuster la couture.

Pour certains matériaux, l&#39;utilisation du **filtre Mosaïque** seul entraînera toujours des artefacts ou des problèmes le long de la couture. Dans ce cas, il est conseillé d&#39;utiliser d&#39;autres filtres tels que **Tampon de duplication** pour résoudre les problèmes de couture et de mosaïque.

Il est recommandé de travailler sur le carrelage du matériau dès le début du processus de création de matériau. Dès qu&#39;un élément sans carrelage est ajouté au matériau, il est préférable de s&#39;assurer qu&#39;il est carrelé avant de continuer. Les filtres de Sampler sont conçus de manière à ne pas casser les matériaux de mosaïque. Cela signifie qu’une fois les carreaux de matériau sous-jacents terminés, vous pouvez continuer à travailler avec les filtres et les matériaux inclus dans Sampler, et votre matériau sera toujours en mosaïque.
