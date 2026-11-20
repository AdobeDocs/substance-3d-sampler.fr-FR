---
title: déformation de peinture
description: Apprenez à utiliser le filtre Déformation de Peinture de Substance 3D Sampler pour maîtriser avec précision la déformation de votre matériau.
source-git-commit: f281c7ec254de74381b2565f835cc32e4de643d2
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 2%
---

# Déformation de peinture

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top">Outils <img src="../../assets/Filters/S_WarpPaint_18_N_D.png" alt=""/><br><strong>In:</strong></td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le filtre <strong>Déformation de Peinture</strong> est un outil puissant conçu pour corriger les distorsions géométriques dans les numérisations basées sur l’image. Elle est particulièrement utile pour les matériaux à motifs linéaires (tels que les tissus de velours côtelé, les planches de bois ou les briques), où les lignes naturelles ne sont pas parfaitement droites ou alignées avec les axes. En définissant manuellement le flux du motif, vous pouvez « redresser » le matériau pour obtenir des cartes de répétition homogènes et de qualité professionnelle.<br></td>
  </tr>
</table>

## Alignement des motifs de Matériau

Vous pouvez ajouter le filtre Déformation de Peinture manuellement à votre Pile de calques, mais le workflow le plus efficace pour les numérisations consiste à utiliser l’action rapide dédiée.

### Utilisation de l’action rapide

1. Ouvrez l&#39;onglet **Action rapide**.
1. Sélectionnez **Aligner les motifs de Matériau en peignant**.

* Sampler ajoutera automatiquement trois calques à votre pile : **Égaliser**, **Déformation de Peinture horizontale** et **Déformation de Peinture verticale**.

1. Dans la **Pile de calques**, identifiez la direction que suit votre motif.

* *Exemple :* pour le velours côtelé avec côtes verticales, conservez la **déformation de Peinture verticale** et désactivez ou supprimez la version horizontale.

### Peinture des repères de déformation

Une fois le filtre sélectionné, vous devez définir le tracé « tordu » actuel du motif afin que Sampler sache comment le redresser.

1. Accédez au panneau **Propriétés** du filtre Déformation de Peinture.

1. Recherchez la propriété **Entrée d&#39;image** et cliquez sur l&#39;icône **Pinceau** en regard pour passer en mode peinture.

1. Ajustez la **taille du pinceau** à l&#39;aide des widgets ou des raccourcis de l&#39;interface utilisateur.

1. Peinture le long des lignes de votre matériau :

   >[!TIP]
   >
   > Maintenez la touche **Maj** enfoncée tout en cliquant pour créer des segments parfaitement droits entre les points.

1. Tracez plusieurs lignes sur la largeur ou l’height de la texture pour fournir suffisamment de données à l’algorithme.

1. Dans le panneau **Propriétés**, basculez le paramètre **Redresser** sur **Activé**. Sampler va déformer l’image afin que les lignes peintes soient parfaitement parallèles à l’axe choisi.

## Référence des paramètres

| Nom | Description | Plage/Options | Par défaut |
| --- | --- | --- | --- |
| **Direction** | Détermine l’axe sur lequel la déformation s’alignera. | Vertical, Horizontal | Vertical |
| **Redresser** | Active ou désactive l’effet de déformation en fonction du masque peint. | Activer/désactiver | Désactivé |
| **Afficher l&#39;entrée** | Incrustation d’assistant affichant des repères pour améliorer la précision de la peinture. | Activer/désactiver | Désactivé |
| **Déformation Lisse** | Contrôle le retrait et le smoothness de la déformation entre les repères peints. | 0.0 - 1.0 | 0.5 |

## Conseils et bonnes pratiques

* **Utiliser Afficher l&#39;entrée :** activez le bouton **Afficher l&#39;entrée** pendant la peinture. Cela fournit une incrustation de grille qui permet de voir plus facilement où l’analyse d’origine s’écarte d’une grille parfaite.
* **Ne pas sur-Peinture :** vous n&#39;avez pas besoin de tracer chaque ligne d&#39;un motif. Habituellement, 3 à 5 lignes bien placées à travers la texture sont suffisantes pour que l&#39;algorithme calcule la déformation nécessaire.
* **Combiner avec la Répétition :** utilisez la déformation de Peinture avant d’appliquer le filtre **Répétition**. Un motif redressé est nettement plus facile à carreler sans seams visibles ou lignes « brisées » sur les bords.
* **Égaliser en premier :** comme illustré dans l’action rapide, placer un filtre **Égaliser** avant la déformation de Peinture permet de supprimer les dégradés d’éclairage, ce qui facilite la visualisation des détails du motif que vous tentez d’aligner.

## Articles connexes

* [Égaliser](../adjustments/equalize.md)
* [Répétition](tiling.md)
* [Actions rapides](../../features-and-workflows/quick-actions.md)
* [Bonnes pratiques d&#39;analyse](../../pipeline-and-integrations/hp-z-captis-support/scanning-best-practices.md)
