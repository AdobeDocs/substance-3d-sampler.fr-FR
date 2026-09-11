---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/tools/delight-ai-powered.html"
breadcrumb-title: ''
description: Utilisez le filtre Delight optimisé par l’IA dans Substance 3D Sampler pour supprimer les informations d’éclairage des images et créer des matériaux de base neutres.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Delight (AI Powered)
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Delight (optimisé par l’IA)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---


# Delight (optimisé par l’IA)

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-lightgeneric-18-n-d.png)

Outils **In:**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

L’outil Delighter vous permet de supprimer les informations d’éclairage du canal de base color. Ceci est important lors de la conversion d’images en matériaux, car les matériaux ne doivent généralement pas inclure d’informations d’éclairage. Un matériau est un ensemble d&#39;informations qui explique comment la lumière doit réagir avec une surface. Ainsi, si des informations de lumière sont déjà bakées dans un canal qui ne devrait pas contenir d&#39;informations de lumière, cela peut empêcher le matériau de représenter la surface de manière réaliste.

*Exemple d **image avant et après traitement par le filtre**&#x200B;Delight (optimisé par l’IA)**. Notez que les tons foncés et les tons clairs ont été supprimés, seule la base color est conservée.*

![](../../assets/120-0-comparison.png)

Les images ci-dessous montrent un matériau avant et après traitement par un filtre **Delight (optimisé par l&#39;IA)**.

![](../../assets/3d-2d-filters-cropped-0043-delighter-in.jpg)

Dans l&#39;image ci-dessus, le matériau comprend encore une quantité importante d&#39;informations d&#39;éclairage dans le canal de base color. Les ombres sombres entre les briques ne doivent pas être présentes dans la couche de base color.

![](../../assets/3d-2d-filters-cropped-0042-delight-out.jpg)

Après la passe de ravissement, les ombres ont été supprimées pour créer un canal de base color plus précis physiquement. Bien que les résultats de cet exemple puissent ne pas sembler perceptibles, le fait de ravir des images est une étape importante de la conversion des images en matériaux.

Dans les images sources, la lumière provient de sources statiques, mais les matériaux doivent être capables de gérer la lumière provenant de n’importe quel angle. Par exemple : si une image source avec une lumière dirigée de haut en bas est convertie en matériau sans passer par une étape de ravissement, elle peut être affichée dans un espace 3D où la lumière brille de bas en haut. Le matériau sera rapidement déplacé, car il semble convertir simultanément les ombres de plusieurs lumières lorsqu&#39;il n&#39;y a qu&#39;une seule source de lumière.

</td>
</tr>
</table>

## Paramètres

Le delighter n&#39;a pas de paramètres - il fonctionne automatiquement.

## Guide d’utilisation

Comment l’utiliser ?

Ajoutez le **filtre Delighter** en haut de la pile de calques.

### Quand l’utiliser ?

Lors de l&#39;utilisation de **Image vers Matériau (B2M)**, une fois que vous avez extrait tous les canaux de vos images et rendu le matériau juxtaposable, utilisez le filtre Délice pour supprimer les informations d&#39;éclairage de la couleur de base. **Le filtre Image vers Matériau (optimisé par l&#39;IA)** comprend une passe de ravissement. Vous n&#39;avez donc pas besoin d&#39;utiliser le filtre **Delighter (optimisé par l&#39;IA)** avec lui.
