---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/generators/surface-relief.html"
breadcrumb-title: ''
description: Utilisez le générateur de Reliefs de surface de Substance 3D Sampler pour créer des motifs de surface en relief et reliefs dans les matériaux.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Surface Relief
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Relief de surface
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---


# Relief de surface

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-surfacerelief-18-n-d.png)

Générateurs De **Entrée :**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Utilisez le filtre Relief de surface pour ajouter du bruit à votre matière. Cela peut aider à séparer les grandes formes ou ajouter un intérêt visuel.

</td>
</tr>
</table>

## Paramètres

<b>Paramètres de base</b>

* <b>Générateur aléatoire</b> :\
  Valeur de départ aléatoire sur laquelle sont basés tous les autres paramètres aléatoires de ce filtre.
* <b>Intensité</b> : 0-1\
  Modification de l’amplitude du bruit
* <b>Intensité du flou</b> : 0-1\
  Intensité du flou appliqué au bruit
* <b>Imperfection De La Surface </b> : Générateur D’Images/De Pinceaux/De Textures\
  Utilisez une image ou un générateur de texture à utiliser comme imperfection de surface.

<b>Paramètres de bruit</b>

* <b>Clamp</b> : 0-1\
  Limitation du bruit à une certaine plage
* <b>Contraste</b> : 0-1\
  Modifier le contraste du bruit
* <b>Inverser</b> : activer/désactiver\
  Inverser la courbe d&#39;height du bruit

<b>Transformation</b>

* <b>Mosaïque</b> : 1-16\
  Contrairement aux <b>paramètres de base > échelle</b>, la fonctionnalité <b>Mosaïque</b> gère le nombre d&#39;instances du bruit.
* <b>Miroir</b> :\
  Symétrie du bruit sur un axe ou les deux
* <b>Décalage</b> :\
  Repositionnement du bruit sur les axes X et Y
* <b>Rotation</b> :\
  Faites pivoter le bruit. L’angle de rotation s’accroche pour vous assurer que la juxtaposition est toujours possible.

<b>Masquer</b>

* <b>Utiliser un masque personnalisé</b> : activer/désactiver\
  Activez cette option pour afficher les commandes de masque personnalisées :
  * <b>Masque</b> : générateur d&#39;image/pinceau/texture\
    Importez une image à utiliser comme masque ou utilisez le pinceau pour peindre directement dans la <b>vue 2D</b>
  * <b>Masque personnalisé - Flou</b> : 0-1\
    Flouter le masque
  * <b>Masque personnalisé - Inverser</b> : activer/désactiver

<b>Paramètres avancés</b>

* <b>Intensité de l&#39;Height</b> : 0-1\
  Contrôle du mélange de la courbe de hauteur du bruit avec la courbe de hauteur des matériaux sous-jacents
* <b>Height - Remplacer la base</b> : basculer\
  Activer/désactiver le remplacement de l’height de base
* <b>Intensité normale</b> : 0-1\
  Régler l&#39;intensité de la courbe de transfert normale du bruit
* <b>Normal - Remplacer la base</b> : activer/désactiver\
  Indique si le mappage normal de base doit être remplacé ou non
* <b>Direction normale</b> :\
  Modifier les axes à utiliser pour la génération normale
* <b>Normal - Direction de la rotation</b>
* <b>Occlusion ambiante - Intensité</b>
* <b>Occlusion ambiante - Rayon</b>
