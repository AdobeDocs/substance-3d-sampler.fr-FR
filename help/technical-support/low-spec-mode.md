---
title: Mode de spécification basse
description: Découvrez le mode de spécification basse, activé par Sampler lorsque le matériel ne présente pas la configuration minimale requise.
hold: true
source-git-commit: 59761aab02bff266047813f1714e3f53ddcb805c
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%
---

# Mode de spécification basse

![](../assets/v6.1/6_1-Checked.png)

Si votre matériel ne respecte pas la [configuration minimale requise](../getting-started/system-requirements.md) de Sampler, Sampler se lance automatiquement en mode Faible spécification, qui se comporte comme le [mode Performances](performance-mode.md) sans possibilité de modifier les paramètres.

## Limitations du mode Faible spécification

Le mode Spécifications basses active automatiquement le **mode Performances** avec toutes les fonctionnalités désactivées et une résolution d&#39;aperçu maximale de 2048 × 2048.

Le mode de spécification basse désactive :

* **Displacement**
* **Tons foncés**
* **Traçage de chemin**

En outre, le mode Spécifications basses empêche les exportations supérieures à 2 048 px × 2 048 px.

![](../assets/low-spec-mode-export-message.png)

*Ce message apparaît dans la **fenêtre d&#39;exportation**en **mode de spécification faible**pour fournir des informations supplémentaires.*

## Comment savoir si le mode Faibles spécifications est activé ?

Lorsque vous lancez Sampler, si la configuration matérielle n’est pas conforme à la configuration minimale requise, une fenêtre s’affiche indiquant les configurations non conformes et vous donnant la possibilité de poursuivre le lancement de Sampler.

L’image ci-dessous montre un exemple d’ordinateur avec moins de 8 Go de VRAM.

![](../assets/low-device-specs-popup.png)

Si vous choisissez de **lancer quand même**, Sampler se lancera en **mode de spécification faible**. Si vous avez coché la case dans le message ci-dessus pour ne pas afficher et lancer malgré tout, vous verrez toujours la bannière suivante lors des lancements suivants.

![](../assets/low-spec-mode-banner.png)

Enfin, bien que le **mode de spécification basse** soit activé, il n&#39;est pas possible de désactiver le mode Performances ou d&#39;ajuster les paramètres du mode Performances.

![](../assets/performance-mode-locked.png)
