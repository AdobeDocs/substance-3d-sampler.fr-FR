---
title: Remplissage d’après le contenu
description: Apprenez à utiliser le filtre Remplissage d’après le contenu de Substance 3D Sampler pour résoudre les problèmes de répétition de motifs ou pour supprimer les dirts ou la saleté indésirables.
source-git-commit: f281c7ec254de74381b2565f835cc32e4de643d2
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 1%
---

# Remplissage d’après le contenu

<table>
  <tr>
    <td>Outils <img src="../../assets/Filters/S_ContentAwareFill_18_N_D.png" alt=""/><br><strong>In:</strong></td>
    <td>Description<br>Le remplissage d'après le contenu permet de supprimer facilement des éléments tels que le dirt, le texte ou d'autres objets indésirables de vos matériaux.<br>Dans l'exemple du sol de la forêt ci-dessous, le bâton se distingue dans le motif répétitif. L’outil Remplissage d’après le contenu nous permet de supprimer la brindille, ce qui rend la répétition un peu moins visible. <br><br><img src="../../assets/content-aware-fill-before.png" alt=""/><br><em>Avant suppression</em><br><br><img src="../../assets/content-aware-fill-after.png" alt=""/><br><em>Après suppression</em></td>
  </tr>
</table>

## Paramètres

* **Sélection de canaux :** sélectionnez les canaux sur lesquels exécuter le filtre. Par défaut, cette option est définie sur toutes les couches. Cependant, vous pouvez également choisir de l’exécuter uniquement sur les couches Height ou Base color.
* **Miroir :** pour les matériaux ou les motifs symétriques, ce paramètre guide le remplissage d&#39;après le contenu pour incorporer le contenu en miroir sur l&#39;ensemble du matériau.
* **Échelle :** pour les motifs géométriques tels que les carreaux ou les briques, ce paramètre peut aider à conserver la structure du motif.

### Paramètres techniques

* **Masque personnalisé :** appliquez un masque à l&#39;aide d&#39;une texture ou utilisez le pinceau pour appliquer votre propre peinture dans le **Viewport 2D**.
* **Rechercher le facteur de recadrage :** recadrez la zone échantillon utilisée par le filtre. Par défaut, la zone d&#39;échantillonnage couvre toute la texture, à l&#39;exception de la zone masquée. L&#39;augmentation du **facteur de recadrage de recherche** réduit la zone d&#39;échantillonnage, ce qui peut aider à limiter les échantillons aux pixels plus proches de la zone masquée.

### Paramètres de remplissage

* **Adaptation des couleurs :** ajustez le degré d&#39;adaptation du remplissage aux couleurs environnantes. Ce paramètre peut être utile pour les matériaux qui
* **Adaptation de la rotation :** pour les motifs pour lesquels la rotation des éléments est importante, tels que les pétales d&#39;une fleur ou les rayons d&#39;une roue, ce paramètre peut aider à créer des résultats plus cohérents.