---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/generators/embossing.html"
breadcrumb-title: ''
description: Utilisez le générateur d’estampage de Substance 3D Sampler pour créer des motifs estampés et des effets de relief de surface en relief dans les matériaux.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Embossing
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Estampage
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---


# Estampage

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-embossing-18-n-d.png)

Générateurs De **Entrée :**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Estampez du texte ou des motifs sur vos matières.

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Taille de l&#39;estampage** : 0-1\
  Modification de la taille de chaque instance
* **Distance d&#39;estampage** : 0-1\
  Modification du thickness des lignes en relief
* **Sélection de motif** :\
  Sélectionnez le motif à estamper. À partir de là, vous pouvez choisir d’estamper du texte ou un motif personnalisé.
* **Mosaïque de motif X** : 1-64\
  Modification du nombre d’instances sur l’axe X
* **Mosaïque Y** : 1-64\
  Modification du nombre d’instances sur l’axe Y

**Estampage**

* **Utiliser l&#39;estampage de bordure** : activer/désactiver\
  Indique si la bordure du motif choisi doit être estampée
* **Inversion de l&#39;estampage de bordure** : basculer\
  Inverser l’height de l’estampage de bordure
* **Intensité de l’estampage de la bordure** : 0-1\
  Modification de l’intensité de l’effet d’estampage
* **Utiliser le remplissage en relief** : activer/désactiver\
  Indique si le remplissage du motif choisi doit être estampé
* **Inversion du remplissage de l&#39;estampage** : basculer\
  Inverser l’height de l’effet d’estampage de remplissage
* **Intensité de l’estampage du remplissage** : 0-1\
  Modification de l’intensité de l’effet d’estampage

**Motif**

* **Utiliser la couleur** : activer/désactiver\
  Indique si une couleur doit être ajoutée à la zone de relief\
  Lorsque l&#39;option **Utiliser la couleur** est activée, un paramètre **Couleur** supplémentaire apparaît pour ajuster la couleur.
* **Masque De Motif** **Distance** : 0-1\
  Modifiez la taille du masque utilisé pour appliquer de la couleur à la zone gaufrée
* **Contraste du masque de motif** : 0-1\
  Réglez le contraste du masque. La diminution du contraste rend les bords du masque plus flous.
* **Utiliser le motif** : activer/désactiver\
  Activez cette option pour placer le motif en mosaïque, désactivez-la pour n’avoir qu’une seule instance. Lorsque le motif n&#39;est pas juxtaposé, les options **Mosaïque de motif** n&#39;apparaissent pas sous la section **Paramètres de base**.
* **Rotation du motif** : 0-1\
  Faire pivoter le motif
* **Décalage du motif** : 0-1\
  Décale chaque ligne du motif de la ligne précédente.
* **Utiliser la rugosité du motif** : activer/désactiver\
  Activez cette option pour remplacer la rugosité du matériau sous-jacent par une valeur de rugosité personnalisée partout où l’effet d’estampage apparaît.\
  Lorsque cette option est activée, une commande **Rugosité du motif** apparaît pour définir la rugosité.
* **Utiliser un motif métallique** : activer/désactiver\
  Activez cette option pour remplacer les valeurs métalliques du matériau sous-jacent par une valeur métallique personnalisée partout où l’effet d’estampage apparaît.\
  Lorsque cette option est activée, une commande **Motif métallique** apparaît pour définir la rugosité.

**Texte** : cette section apparaît uniquement si **Sélection de motif** sous **Paramètres de base** est définie sur **Texte**

* **Sélection de police** :\
  Sélection d’une police
* **Texte** : champ de texte\
  Saisissez le texte à gaufrer
* **Taille du texte** : 0-1\
  Ajustement de la taille de la police

**Gomme**

* **Gomme normale** : 0-1
* **Occlusion ambiante de la gomme** : 0-1
* **Opacité De La Gomme** : 0-1

**Paramètres avancés**

Ces paramètres vous permettent d’ajuster les valeurs pour l’ensemble du matériau.

* **Luminosité** : 0-1
* **Contraste** : -1 à 1
* **Décalage de teinte**; 0-1
* **Saturation** : 0-1
* **Intensité normale**; 0-1

## Guide d’utilisation

Ajoutez le filtre Estampage en haut de la pile de calques, puis commencez à régler les paramètres.

Les paramètres les plus importants sont généralement **Paramètres de base > Sélection de motif** pour modifier le motif que le filtre utilisera et **Motif > Utiliser une mosaïque de motifs** pour activer et désactiver la mosaïque.
