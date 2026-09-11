---
breadcrumb-title: ''
description: Découvrez les paramètres prédéfinis de matériau, comment appliquer un paramètre prédéfini à votre matériau et comment créer et gérer des paramètres prédéfinis personnalisés.
title: Paramètres prédéfinis de matériau
user-guide-description: ''
user-guide-title: ''
source-git-commit: 6fe7ff5c975480f2e8852dd8b443c6650bd883ea
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 4%

---


# Paramètres prédéfinis de matériau

Les modèles de création de matériaux fournissent des points de départ prédéfinis pour la création de matériaux avec un comportement physique avancé. Chaque gabarit configure le modèle de matériau, les couches activées et les paramètres par défaut requis pour un type de surface spécifique, ce qui vous permet de créer rapidement des matériaux complexes tout en gardant un contrôle total sur le résultat.
Les modèles sont disponibles lors de la création d&#39;un nouveau matériau et peuvent être utilisés avec les modèles de matériau OpenPBR et ASM.

![Fenêtre Créer un matériau](../../assets/6.0_materialPresets.png)

## Création d’un matériau à partir d’un modèle

Pour créer un matériau à l’aide d’un modèle :

Ouvrez la boîte de dialogue Créer un matériau.
Sélectionnez un modèle dans les onglets Prédéfini ou Personnalisé.
Réglez les paramètres de matériau (nom, résolution, modèle de matériau, couches).
Cliquez sur Créer pour commencer à travailler avec le matériau configuré.

Le modèle sélectionné définit la structure initiale du matériau, notamment les canaux activés et la façon dont ils sont configurés dans la Pile de calques.

## Catégories de paramètres prédéfinis

### Modèles prédéfinis

Les modèles prédéfinis sont des configurations de matériau prêtes à l’emploi conçues pour couvrir les comportements de matériau physique courants. Ils codent les bonnes pratiques et les configurations de canaux recommandées pour chaque cas d’utilisation.
Les modèles prédéfinis disponibles sont les suivants :

* Matériau de base
Matériau physique standard avec canaux couramment utilisés activé. Utilisez ce modèle pour les matériaux simples ou génériques qui ne nécessitent pas de comportement particulier.

* Anisotropie
Configure le matériau pour les reflets dépendants de la direction, adaptés aux métaux brossés ou aux surfaces avec des micro-détails orientés.

* Revêtement
Ajoute une couche réfléchissante secondaire au-dessus du matériau de base, ce qui permet d’obtenir des effets de vernis ou de pelage transparent.

* Fibres
Active les effets de surface doux et diffractés par la lumière, utilisés pour les tissus, les fibres ou les matériaux d’aspect velouté.

* Subsurface
Active le transport lumineux souterrain pour les matériaux tels que la cire, les plastiques ou les surfaces organiques où la lumière pénètre sous la surface.

* Transparent
Configure le matériau pour la transmission de la lumière, adapté aux matériaux transparents minces ou de type verre.


Chaque préréglage prédéfini définit automatiquement les canaux requis et les valeurs par défaut, ce qui réduit la configuration manuelle et la complexité technique.

### Paramètres prédéfinis personnalisés

Les paramètres prédéfinis personnalisés vous permettent de réutiliser vos propres configurations de matériau.
Tout paramètre prédéfini de matériau que vous créez peut être enregistré comme modèle personnalisé et apparaîtra dans l’onglet Personnalisé. Cela permet une création de matériau cohérente entre les projets ou les équipes, à l’aide de normes partagées et de configurations de canaux.

## Détails du paramètre prédéfini

Le panneau Détails du paramètre prédéfini affiche et contrôle les paramètres utilisés pour créer le nouveau matériau.

### Nom de la ressource

Définit le nom de l’actif de matériau qui sera créé.

### Résolution

Contrôle la résolution par défaut des cartes de matériau (Largeur et Height). Cette résolution s’applique à tous les canaux activés lors de la création du matériau.

### Modèle de matériau

Spécifie le modèle de matériau utilisé par le matériau :

OpenPBR pour des workflows physiques modernes et standardisés
ASM pour la compatibilité avec les pipelines existants

Le modèle sélectionné s’adapte au modèle de matériau choisi.

### Ajouter un matériau de base

Lorsque cette option est activée, Sampler crée un calque de remplissage de base en utilisant un matériau de base compatible avec le modèle sélectionné. Cela fournit un résultat visuel immédiat et un point de départ utilisable. Le matériau de base est adapté aux modèles de matériau OpenPBR et ASM.

### Appliquer les valeurs de vignettes prédéfinies

Lorsque cette option est activée, le matériau est initialisé avec les valeurs utilisées pour générer la vignette d’aperçu du modèle, au lieu des valeurs par défaut neutres. Cela permet de démontrer le comportement prévu du modèle et de disposer d’une base visuelle sur laquelle commencer à s’appuyer.

### Modif. liste

Cliquez sur **Modifier la liste** pour personnaliser l&#39;ensemble de canaux avant de créer le matériau. Vous pouvez activer ou désactiver les canaux selon vos besoins, ou enregistrer la configuration en tant que nouveau modèle personnalisé.

