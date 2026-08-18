---
breadcrumb-title: ''
description: Apprenez à utiliser les modèles de matériau dans Substance 3D Sampler pour créer rapidement des matériaux complexes et réalistes en appliquant des effets physiques avancés à partir de points de départ simples et prêts à l’emploi.
user-guide-description: ''
user-guide-title: ''
title: Paramètres prédéfinis de création de matériau
source-git-commit: 8777fdda4545110ed765f1d275c35bd11e71903b
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 2%

---


# Paramètres prédéfinis de création de matériau

Les modèles de création de matériaux fournissent des points de départ prédéfinis pour les matériaux de construction dotés d&#39;un comportement physique avancé. Chaque gabarit configure le modèle de matériau, les couches activées et les paramètres par défaut requis pour un type de surface spécifique, ce qui vous permet de créer rapidement des matériaux complexes tout en gardant un contrôle total sur le résultat. Les templates sont disponibles lors de la création d&#39;une nouvelle matière et peuvent être utilisés avec les modèles de matériau OpenPBR et ASM.

![Fenêtre Créer une matière](../../assets/6.0_materialPresets.png)

>[!TIP]
> Vous pouvez en savoir plus sur la création de matériaux avancés qui tirent parti des effets de flou, de la subsurface et des couches de revêtement [ici](../../features-and-workflows/create-advanced-materials/advanced-materials.md).

## Création d&#39;un matériau à partir d&#39;un modèle

Pour créer un matériau à l’aide d’un modèle :

Ouvrez la boîte de dialogue Créer une matière. Sélectionnez un modèle dans les onglets Prédéfini ou Personnalisé. Réglez les paramètres de matière (nom, résolution, modèle de matériau, couches). Cliquez sur Créer pour commencer à travailler avec la matière configurée.

Le modèle sélectionné définit la structure initiale du matériau, notamment les canaux activés et la façon dont ils sont configurés dans la pile de calques.

## Catégories de paramètres prédéfinis

### Modèles prédéfinis

Les gabarits prédéfinis sont des configurations de matériau prêtes à l&#39;emploi conçues pour couvrir les comportements physiques courants en matière. Ils codent les bonnes pratiques et les configurations de canaux recommandées pour chaque cas d’utilisation. Les modèles prédéfinis disponibles sont les suivants :

- Matériau de base Matériel standard à base physique avec les canaux couramment utilisés activés. Utilisez ce modèle pour les matériaux simples ou génériques qui ne nécessitent pas de comportement spécialisé.

- Anisotropie Configure le matériau pour des reflets dépendants de la direction, adaptés aux métaux brossés ou aux surfaces avec des micro-détails orientés.

- Revêtement Ajoute une couche réfléchissante secondaire au-dessus du matériau de base, ce qui permet d’obtenir des effets de vernis ou de couche transparente.

- Fuzz Active les effets de surface doux et diffractables par la lumière, utilisés pour les tissus, les fibres ou les matériaux d’aspect velouté.

- Subsurface Active le transport de lumière sous la surface pour les matériaux tels que la cire, les plastiques ou les surfaces organiques où la lumière pénètre sous la surface.

- Transparent Configure le matériau pour la transmission de la lumière, adapté aux matériaux transparents minces ou de type verre.

Chaque préréglage prédéfini définit automatiquement les canaux requis et les valeurs par défaut, ce qui réduit la configuration manuelle et la complexité technique.

### Paramètres prédéfinis personnalisés

Les paramètres prédéfinis personnalisés vous permettent de réutiliser vos propres configurations de matériau. Tout paramètre prédéfini de matière que vous créez peut être enregistré en tant que modèle personnalisé et s’affiche dans l’onglet Personnalisé. Cela permet une création cohérente de matériaux entre les projets ou les équipes, à l’aide de normes partagées et de configurations de canaux.

## Détails du paramètre prédéfini

Le panneau Détails du paramètre prédéfini affiche et contrôle les paramètres utilisés pour créer le nouveau matériau.

### Nom de la ressource

Définit le nom de l&#39;immobilisation matérielle qui sera créée.

### Résolution

Contrôle la résolution par défaut des textures matériau (Largeur et Height). Cette résolution s’applique à tous les canaux activés lors de la création de la matière.

### Modèle de matériau

Indique le modèle de matériau utilisé par la matière :

OpenPBR pour les workflows physiquement basés modernes et standardisés ASM pour la compatibilité avec les pipelines existants

Le modèle sélectionné s’adapte au modèle de matériau choisi.

### Ajouter un matériau de base

Lorsque cette option est activée, Sampler crée un calque de remplissage de base à l’aide d’un matériau de base compatible avec le modèle sélectionné. Cela fournit un résultat visuel immédiat et un point de départ utilisable. Le matériau de base est adapté aux modèles de matériau OpenPBR et ASM.

### Appliquer les valeurs de vignettes prédéfinies

Lorsque cette option est activée, la matière est initialisée avec les valeurs utilisées pour générer la vignette d&#39;aperçu du modèle, au lieu des valeurs par défaut neutres. Cela permet de démontrer le comportement prévu du modèle et de disposer d’une base visuelle sur laquelle commencer à s’appuyer.

### Modif. liste

Cliquez sur **Modifier la liste** pour personnaliser l&#39;ensemble de canaux avant de créer le matériau. Vous pouvez activer ou désactiver les canaux selon vos besoins, ou enregistrer la configuration en tant que nouveau modèle personnalisé.