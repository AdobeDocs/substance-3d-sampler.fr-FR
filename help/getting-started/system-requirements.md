---
helpx_url: 'https://helpx.adobe.com/substance-3d-sampler/getting-started/system-requirements.html'
breadcrumb-title: ''
description: Vérifiez la configuration requise pour Substance 3D Sampler pour vous assurer que votre matériel et vos logiciels sont compatibles.
helpx_creative_field: ''
helpx_description: Sampler > Getting Started > System requirements
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Configuration requise
user-guide-description: ''
user-guide-title: ''
source-git-commit: cd61972eaf1567863dc8c3549a1c90c84ffee825
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 1%

---


# Systèmes pris en charge

Vous trouverez ci-dessous une liste du matériel et des systèmes pris en charge par l’application :

>[!WARNING]
>
> Les pilotes Nvidia suivants sont connus pour provoquer une instabilité lors de l’exécution de Sampler :
>
> * 610.47
>
> Nous vous recommandons d’éviter d’utiliser ces versions : idéalement, utilisez une version plus récente ou, si aucune version plus récente n’est disponible, utilisez la version précédente.

## Windows

|  | Minimum | Recommandé | Optimale |
| --- | --- | --- | --- |
| **SE** | Windows 11 64 bits version 23H2 | Windows 11 64 bits version 24H1 | Windows 11 64 bits version 24H2 |
| **CPU** | Intel Core i5 AMD Ryzen 5 | Intel Core i7 AMD Ryzen 7 | Intel Core i9 AMD Ryzen 9 |
| **GPU** | NVIDIA GeForce RTX 2060 Super NVIDIA Quadro RTX 4000 AMD Radeon RX 5700 XT AMD Radeon Pro W5700 | NVIDIA GeForce RTX 3080 NVIDIA Quadro A4000 AMD Radeon RX 6800 XT AMD Radeon Pro W7700 | NVIDIA GeForce RTX 4090 NVIDIA Quadro RTX 5000 Ada Generation AMD Radeon RX 7900 XTX AMD Radeon Pro W7800 |
| **VRAM** | 8 Go | 16 Go | 24 Go |
| **RAM** | 16 Go | 32 Go | 64 Go |
| **Stockage** | Disque SSD avec 30 Go d’espace disponible | Disque SSD avec 50 Go d’espace disponible | Disque SSD avec 70 Go d’espace disponible |

### macOS

|  | Minimum | Recommandé | Optimale |
| --- | --- | --- | --- |
| **SE** | macOS 13 Ventura | macOS 14 Sonoma | macOS 26 Tahoe |
| **CPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **GPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **RAM** | 24 Go | 32 Go | 64 Go |
| **Stockage** | Disque SSD avec 30 Go d’espace disponible | Disque SSD avec 50 Go d’espace disponible | Disque SSD avec 70 Go d’espace disponible |

### Linux

| Grands comptes | Vapeur |
| --- | --- |
| RHEL 8 <br>RHEL 9 | Ubuntu 22.04 |

>[!NOTE]
>
> Si votre système répond à la configuration requise ci-dessus, mais que les performances restent médiocres, il est possible que Sampler n’utilise pas le bon GPU.
>
> Si vous utilisez un GPU NVIDIA, [modifiez le GPU que Sampler utilise en suivant les instructions de cette page](../technical-support/configuration/nvidia-driver-settings.md).

## Recommandations générales

* Pour travailler dans des conditions confortables, nous vous recommandons un moniteur avec une résolution supérieure à 1 mégaPixel et plus large que 1280 pixels.
* De nombreuses applications de Substance dépendent d’OpenSSL 1.1.1 pour la compatibilité RHEL8/9. Pour les systèmes dotés de nouvelles versions d’OpenSSL, vous devez les fournir manuellement.

## Configurations non prises en charge

**Windows**

* Les ordinateurs virtuels ne sont pas pris en charge.
* Windows Server n&#39;est pas pris en charge.

**Mac**

* Seules les configurations Apple officielles sont prises en charge.
* Les eGPU ne sont actuellement pas pris en charge et peuvent présenter des problèmes de stabilité.

**Linux**

* Les pilotes Mesa sous Linux ne sont pas pris en charge.

**Toute plateforme**

* Les GPU intégrés ne sont pas pris en charge sur les processeurs x86-64 (Intel, AMD).
* L’utilisation de Sampler en association avec un logiciel tiers qui intercepte les appels Sampler aux pilotes graphiques n’est pas prise en charge. Ces logiciels comprennent :
  * Injecteurs de post-traitement tels que les nuanciers qui appliquent un étalonnage des couleurs, des effets de caméra, ...
  * Incrustations à l’écran telles que les réticules personnalisés, les métriques de performance GPU, les habillages pour la diffusion vidéo...

## Versions minimales du pilote GPU

Vous trouverez ci-dessous une liste des versions minimales du pilote GPU requises pour que l’application s’exécute sans problème. Cette liste est susceptible d’être modifiée à mesure que de nouvelles versions sont publiées.

Pour télécharger de nouveaux pilotes, voir : [Le GPU a des pilotes obsolètes](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/technical-support/technical-issues/gpu-issues/gpu-has-outdated-drivers).

| SE | NVIDIA | AMD | Intel |
| --- | --- | --- | --- |
| **Windows** | GeForce 551.86 Quadro/RTX 538.33 | Radeon 23.8.1 Radeon Pro / FirePro 24.q2 | 31.0.1015590 |
| **Linux** | 525.116.04 ou version ultérieure *ou* 535.54.03 ou version ultérieure | Radeon 23.20 Pro 23.Q3 | Non pris en charge |

>[!NOTE]
>
> Sur **Mac OS**, le pilote GPU est fourni par le système d&#39;exploitation lui-même. Effectuez une mise à jour vers la dernière version de votre système d’exploitation pour accéder au pilote le plus récent.

## Langues

L’interface du logiciel est disponible dans les langues suivantes :

* English
* Deutsch
* Français
* 日本語
* Coréen
* 中文
* Italien
* Portugais
* Espagnol
