---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/interface/panels/layers-panel.html"
breadcrumb-title: ''
description: Apprenez à utiliser le panneau Calques de Substance 3D Sampler pour gérer les calques de filtre et créer des piles de matériaux complexes.
helpx_creative_field: ""
helpx_description: Sampler > Interface > Panels > Layers panel
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Panneau Calques
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0f989901713dd30f8f936de2445caf5dc70a9225
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 2%

---


# Panneau Calques

<table>
<tr style="border: 0;">
<td style="border: 0; width: 70%" valign="top">

Le **panneau Calques** contient la pile de calques et les raccourcis pour gérer vos calques. Le **panneau Calques** fonctionne en étroite collaboration avec le **panneau Propriétés** : sélectionnez un calque dans le **panneau Calques** pour voir ses propriétés dans le **panneau Propriétés**.

Le **panneau Calques** se compose de trois sections principales :

1. La section Outils contient des boutons que vous pouvez utiliser pour
   1. Afficher/Masquer la résolution des calques
   1. Changer la stratégie de résolution des calques
   1. Ajouter un calque
   1. Ajouter un matériau de base
   1. Importer un filtre personnalisé
   1. Supprimer un calque
1. Le **sélecteur de mode de fusion** vous permet d&#39;ajuster la façon dont un calque se fond avec les calques situés en dessous. Le **sélecteur de mode de fusion** est uniquement disponible lorsqu&#39;un calque Matériau est sélectionné : les filtres n&#39;utilisent pas de modes de fusion.
1. La **pile de calques** contient tous les calques qui composent votre ressource.

</td>
<td style="border: 0;" valign="top">

![Animation du panneau Calques d&#39;aucun calque vers une pile complète qui crée un matériau](../../assets/Layers-panel-gen.png.img.png)

</td>
</tr>
</table>

## La pile de calques

La pile de calques est l’ensemble des matériaux, filtres et autres ressources qui composent votre matériau actuel. Comme dans Photoshop et Substance 3D Painter, la pile de calques fonctionne du calque inférieur au calque supérieur. Cela signifie que chaque calque peut affecter les calques situés en dessous.

Il existe plusieurs façons de gérer la pile de calques :

| Actions | Comment |
| --- | --- |
| Ajouter un calque | Faites glisser une ressource du panneau **Ressources** dans la clôture pour l&#39;ajouter en haut de la pile de calques. Faites glisser une ressource du panneau **Ressources** dans la pile de calques pour l&#39;ajouter à un emplacement spécifique dans la pile de calques. Utilisez le bouton **Ajouter un calque** de la section Outils pour sélectionner un filtre dans une liste. |
| Déplacer un calque | Faites glisser un calque dans la pile de calques pour le déplacer. Lors du déplacement d’un calque, une barre s’affiche pour indiquer l’emplacement du calque. |
| Supprimer un calque | Cliquez sur un calque pour le sélectionner et appuyez sur **Suppr** ou utilisez le bouton **Supprimer un calque** dans la section Outils. |
| Activer/désactiver la visibilité | Passez le curseur de la souris sur un calque pour voir le bouton à bascule **Visibilité** sur le côté droit du calque. Lorsque la visibilité d’un calque est désactivée, elle n’est pas calculée. |
| Afficher les propriétés du calque | Cliquez sur un calque pour ouvrir ses propriétés dans le panneau **Propriétés**. |
| Afficher/Masquer la résolution | Cliquez sur le bouton en haut à gauche du **panneau Calques**. |
| Changer la résolution de tous les calques | Cliquez sur la flèche à côté du bouton « Afficher/Masquer la résolution », sélectionnez la stratégie pour tous les calques de la pile. |
| Permutation d’une résolution de calque | Cliquez sur un calque pour ouvrir ses propriétés, cliquez sur la résolution dans le **panneau Propriétés**, sélectionnez la stratégie de résolution que le calque utilisera. |

## Types de calques

Il existe trois types de calque :

* Matériaux
* Filtres
* Images

### Calques Matériau

Un calque Matériau contient des informations dans plusieurs couches et peut être fusionné avec les calques situés en dessous. Les calques Matériau apparaissent légèrement différemment selon qu’ils se trouvent au bas de la pile ou non. Par exemple, l’image ci-dessous montre un matériau rocheux déposé deux fois dans la pile de calques. Notez que le calque inférieur n’a pas d’icône pour contrôler le mélange, contrairement au calque supérieur.

![Calques de matériau dans la pile de calques, le calque supérieur a une option de fusion.](../../assets/Material-Layer.png)

Les règles générales applicables aux calques Matériau sont les suivantes :

* Un calque Matériau utilise toujours la résolution du document.
* Un calque Matériau au bas de la pile n&#39;a rien avec lequel fusionner. Le **sélecteur de mode de fusion** n&#39;est donc pas disponible.
* Un calque Matériau qui n&#39;est pas au bas de la pile peut se fondre avec les calques sous-jacents. Vous pouvez donc utiliser le **sélecteur de mode de fusion** pour modifier le mode de fusion. En outre, une icône de **fusion** apparaît en regard de l&#39;icône de **calque**. Sélectionnez l&#39;icône de fusion **fusionner** pour ajuster les paramètres de fusion du calque en fonction du mode de fusion sélectionné.

### Calques de filtre

![Propriétés du filtre Teinte/saturation lors du réglage des calques sous-jacents.](../../assets/HueSaturation_LayerFilter.gif)

Les filtres effectuent des opérations sur les calques situés en dessous d’eux pour créer des effets spécifiques. Par exemple, dans l&#39;image au-dessus du **filtre Teinte/Saturation**, vous pouvez régler la teinte, la saturation et la luminosité des calques sous-jacents.

Certains filtres peuvent utiliser un ou plusieurs autres calques comme entrées. Par exemple :

* Le **filtre d&#39;Atlas scatter** peut prendre une matière comme entrée.
* Le **filtre d&#39;Atlas scatter** mettra en dispersion des instances à partir du matériau d&#39;atlas d&#39;entrée en fonction des paramètres **Atlas scatter**.

Faites glisser un matériau sur un emplacement d’entrée de calques pour l’utiliser comme entrée.

Un calque de filtre utilise la stratégie de résolution par défaut définie dans les préférences. Vous pouvez modifier la résolution utilisée par le filtre dans le panneau des propriétés.

![Changer la résolution d&#39;un calque de filtre](../../assets/SwitchLayerResolution.gif)

### Calques d’image

Les calques d’image utilisent leur propre résolution et se trouvent principalement dans le workflow Image vers matériau. Comme pour les calques Matériau, vous pouvez créer un calque d&#39;image en faisant glisser une image à partir du **panneau Actifs**.

Vous pouvez faire glisser une image depuis l’explorateur de fichiers de votre système dans Sampler. S’il y a déjà des calques dans votre pile de calques, le calque d’image sera ajouté en haut de la pile. S’il n’y a pas de calques dans la pile de calques, une boîte de dialogue apparaît dans laquelle vous pouvez choisir le traitement de l’image :

* **Image en matériau** vous permet d&#39;utiliser l&#39;IA pour convertir une image en matériau.
* **Multiangle vers matériau** vous permet d&#39;utiliser plusieurs images avec différentes conditions d&#39;éclairage pour créer un matériau.
* **L&#39;importation de texture** vous permet d&#39;utiliser des images importées comme couches de texture pour créer un matériau.
* **Utiliser comme bitmap** importe l&#39;image en tant que calque bitmap simple.

Vous pouvez également faire glisser plusieurs images sélectionnées dans la pile de calques à la fois pour les importer toutes en tant que calque unique. Cela peut être utile pour les filtres multi-images tels que la **fusion HDR** et le **Multiangle vers matériau**. Sélectionnez le calque contenant plusieurs images pour modifier les données de couche pour chaque image.
