---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/filters/tools/height-to-normal.html"
breadcrumb-title: ''
description: Utilisez l’outil Height à la normale de Substance 3D Sampler pour convertir les calques d’height en calques de normales pour les workflows de création de matériaux.
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Height to Normal
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Height à la normale
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---


# Height à la normale

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-heighttonormal-18-n-d.png)

Outils **In:**

</td>
<td width="58.30%" style="border: 0;" valign="top">

## Description

Générez des données de couche Normal en fonction de la couche height.

Dans les images ci-dessous, vous pouvez voir le filtre **Height à la normale** en action.

![](../../assets/h2n-in.jpg)

Dans l&#39;image ci-dessus, il n&#39;y a pas de données normales du matériau. Seule la carte d&#39;height est disponible et affichée dans la **vue 2D**.

![](../../assets/h2n-out.jpg)

Avec le filtre **Height à la normale**, les données normales sont générées à partir de la carte d&#39;height affichée dans l&#39;image supérieure. La lumière rebondit de manière plus réaliste sur le matériau dans la deuxième image grâce à la carte de normales générée.

</td>
</tr>
</table>

## Paramètres

**Paramètres de base**

* **Utiliser les unités mondiales** : activer/désactiver\
  Indiquez si les paramètres sont mesurés à l’aide d’unités réelles ou non. Cela modifie les paramètres disponibles.
  * **Si l&#39;option Utiliser les unités universelles est activée :**
    * **Taille de la surface (cm)** : 0-500\
      Définir la taille de l’espace UV en unités universelles
    * **Profondeur Height (cm)** : 0-10\
      Définissez la distance représentée par la carte d’height. Si la courbe d&#39;height représente une petite distance, une grande différence dans les valeurs de courbe d&#39;height peut avoir un faible impact sur l&#39;angle normal. Si la courbe d&#39;height représente une grande distance, une petite différence dans les valeurs de courbe d&#39;height peut représenter un grand angle sur la courbe de normales.
  * **Si Utiliser les unités universelles est désactivé :**
    * **Intensité** : 0-3\
      Réglage de la pente des angles normaux
* **Combiner la normale inférieure** : 0-1\
  Ajoutez le mappage normal existant aux résultats de ce filtre.

**Masquer**

* **Masque personnalisé** : activer/désactiver\
  Activez ou désactivez l’utilisation d’un masque personnalisé. Si cette option est activée, les paramètres suivants apparaissent :
  * **Masque** : image/pinceau\
    Sélectionnez une image à utiliser comme masque ou utilisez le pinceau pour peindre un masque personnalisé directement dans la vue 2D
  * **Masque personnalisé - Flou** : 0-1\
    Flouter le masque
  * **Masque personnalisé - Inverser** : activer/désactiver\
    Inverser le masque
