---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/adjustments/fill.html"
breadcrumb-title: ''
description: Utilisez le filtre Remplissage de Substance 3D Sampler pour remplir des zones de texture avec des couleurs unies ou des motifs pour les workflows de création de matériaux.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Adjustments > Fill
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Fond
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0f989901713dd30f8f936de2445caf5dc70a9225
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 4%

---


# Fond

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/Fill_Icon_1.png)

**Entrée :** Réglages

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Le **filtre Fond** vous permet de remplacer ou d’ajuster les valeurs de couches spécifiques en fonction d’une valeur sélectionnée.
Dans Sampler 6.0, le filtre Fond adapte ses paramètres en fonction du type de canal auquel il est appliqué. Cela garantit que les commandes disponibles correspondent toujours à la signification physique et au type de données du canal sélectionné, et que le filtre peut être appliqué à n’importe quel mappage, même à partir de workflows personnalisés.

Dans les images ci-dessous, la couche de couleur de base a été remplacée.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/fillnobc.png.img.png){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/fillbc.png){width="200px"}

</td>
</tr>
</table>

</td>
</tr>
</table>

## Paramètres

<b>Appliqué à...</b>

La liste déroulante Appliqué à... détermine le canal sur lequel porte le filtre Remplissage.
**Seuls les canaux actuellement activés dans les paramètres de canal du matériau apparaissent dans cette liste.** Si le canal à remplir n’est pas disponible :

* Ouvrez le panneau des paramètres de canal (tout en bas de la barre de navigation de gauche)
* Cliquez sur « Modifier la liste »
* Activer le canal souhaité
* Réapplication ou mise à jour du filtre Fond

Une fois activé, le canal devient disponible dans la liste déroulante Appliqué à...

<b>Paramètres de base</b>

Les paramètres du filtre de remplissage **changent dynamiquement en fonction du type de canal** sélectionné dans Appliqué à... Il existe quatre jeux de paramètres, chacun correspondant à un type de mappage spécifique.

### Paramètres de table des couleurs

Ce paramètre est utilisé lorsque le filtre Fond est appliqué aux couches de couleur.

#### Exemples de canaux :

* Couleur de base
* Couleur du revêtement
* Couleur du sous-sol...

#### Paramètres disponibles

* Couleur
Sélectionne la couleur de RGB utilisée pour remplir la couche.
* Valeur personnalisée
Basculez pour ouvrir le mappage personnalisé. Sélectionnez une image pour remplacer la couche sélectionnée ou peignez directement dans la **vue 2D**.
* Graine aléatoire
Modifie la randomisation utilisée lorsque les variations de procédure sont activées.
* Mode de fusion
Détermine la manière dont le remplissage se fond dans les calques inférieurs (par exemple : Copier, Ajouter, Multiplier).
* Opacité
Réglez l’opacité des informations de la nouvelle couche par rapport aux informations de la couche existante. En d’autres termes, cette option contrôle l’opacité du masque utilisé pour appliquer le nouveau fond de couche.

Ce mode est généralement utilisé pour initialiser ou remplacer les informations de couleur.

### Paramètres de mappage des niveaux de gris

Ce paramètre est utilisé lorsque le filtre Fond est appliqué à des couches de niveaux de gris scalaires.

#### Exemples de canaux :

* Rugosité spéculaire
* Métallique de base
* Opacité
* Height...

#### Paramètres disponibles

* Value
Définit une seule valeur de niveaux de gris pour la couche.
* Graine aléatoire
Modifie la randomisation utilisée lorsque les variations de procédure sont activées.
* Valeur personnalisée
Basculez pour ouvrir le mappage personnalisé. Sélectionnez une image pour remplacer la couche sélectionnée ou peignez directement dans la **vue 2D**.
* Mode de fusion
Copier, Ajouter (Densité linéaire - Éclaircir), Soustraire, Multiplier, Ajouter sub, Max (Éclaircir), Min (Obscurcir), Basculer, Diviser, Incruster, Superposition, Superposition, Superposition, Lumière tamisée.
Sélectionnez le mode de fusion pour fusionner l’entrée personnalisée avec les calques sous-jacents.
* Opacité
Réglez l’opacité des informations de la nouvelle couche par rapport aux informations de la couche existante. En d’autres termes, cette option contrôle l’opacité du masque utilisé pour appliquer le nouveau fond de couche.

Ce mode est utile pour définir des propriétés physiques uniformes, comme une valeur de rugosité ou d’opacité constante.

#### Paramètres de mappage normaux

Utilisé lorsque le filtre Fond est appliqué aux canaux **normaux**.

##### Exemples de canaux :

* Normale
* Coat normal

##### Paramètres disponibles

* Graine aléatoire
Modifie la randomisation utilisée lorsque les variations de procédure sont activées.
* Valeur personnalisée
Basculez pour ouvrir le mappage personnalisé. Sélectionnez une image pour remplacer la couche sélectionnée ou peignez directement dans la **vue 2D**.
* Opacité
Réglez l’opacité des informations de la nouvelle couche par rapport aux informations de la couche existante. En d’autres termes, cette option contrôle l’opacité du masque utilisé pour appliquer le nouveau fond de couche.

Ce mode est principalement utilisé pour réinitialiser ou neutraliser les informations normales, ou pour établir une ligne de base propre avant d&#39;ajouter des détails normaux.

### Paramètres de valeur uniforme

Ce paramètre est utilisé pour les couches reposant sur une seule valeur physique uniforme et non sur une texture plaquée.

#### Exemples de canaux

* Specular...

#### Paramètres disponibles

* Graine aléatoire
Modifie la randomisation utilisée lorsque les variations de procédure sont activées.
* Value
Définit la valeur constante appliquée à la couche.
* Mode de fusion
Entre Normal et Produit

Ce mode est particulièrement utile lorsque vous travaillez avec des comportements de matériau avancés introduits par le biais de modèles, où certaines propriétés sont contrôlées par des valeurs scalaires plutôt que par des cartes.

## Cas d’utilisation typiques

Le filtre Fond est couramment utilisé pour :

* Initialisation des couches lors de la création d’un matériau à partir de zéro
* Remplacer les valeurs de couche existantes
* Définir des propriétés physiques uniformes (par exemple, rugosité ou métallisation fixe)
* Neutraliser les couches comme Normal avant de reconstruire les détails
* Ajustez rapidement les propriétés avancées telles que la fluidité, la translucidité ou les valeurs de revêtement

Le filtre Remplissage s’adaptant automatiquement au canal sélectionné, il fournit un flux de production cohérent et prévisible pour tous les types de matériau.
