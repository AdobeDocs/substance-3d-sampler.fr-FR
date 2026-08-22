---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/pipeline-and-integrations/hp-z-captis-support/faq-hp-z-captis-support-in-sampler.html"
breadcrumb-title: ''
description: Consultez les questions fréquemment posées sur la prise en charge de HP Z Captis dans Substance 3D Sampler pour obtenir des réponses sur l’intégration et l’utilisation du matériel.
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: FAQ sur la prise en charge de HP Z Captis dans Sampler
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '1547'
ht-degree: 0%

---


# Questions les plus fréquemment posées

## Exemples de matériaux

+++Quels sont les cas d’utilisation couverts par Captis ?
La solution couvre des cas d&#39;utilisation intersectoriels (Automobile, Vêtement, Conception de produits, Média et divertissement, Architecture...). Le mode Studio permet la capture sur ordinateur (reproductible, efficace et simple), tandis que le mode Explorateur permet la capture mobile «flexible, mobile, s&#39;adaptant à chaque situation).

+++

+++Quels types de matériaux peuvent être numérisés et capturés avec Captis ?
Tous les types de matériaux peuvent être numérisés et capturés, sauf avec plusieurs couches de revêtement transparentes (les peintures automobiles sont exclues du champ d’application de Captis). Certains matériaux spécifiques peuvent nécessiter un traitement supplémentaire dans Sampler pour optimiser les résultats. Veuillez noter que les algorithmes de traitement seront continuellement optimisés au fil du temps.

+++

+++Quelles sont les restrictions sur la taille ou la forme de l&#39;échantillon de matériau - les échantillons doivent-ils être plats ?
Captis peut numériser une grande variété d’échantillons de matière, de taille ou de forme. Il est livré avec des aimants pour aplatir les échantillons sur le plateau d&#39;échantillonnage. Il existe plusieurs modes pour capturer un échantillon de matière avec Captis :

* Mode Studio : avec la base studio sur votre bureau, en studio ou en usine, Captis prendra des échantillons jusqu&#39;à 30cm x 30cm - avec rétroéclairage pour l&#39;opacité. La profondeur du plateau d&#39;échantillonnage est de 1,8 CM.

* Mode Explorateur : vous pouvez utiliser l’anneau de l’explorateur sur le terrain, sur le plateau ou dans des environnements uniques et activer la capture flexible pour les échantillons de plus de 30 cm x 30 cm. Limitation actuelle : veuillez noter que le mode Explorateur est toujours une version antérieure et n’est pas encore optimisé (à partir de la version du 29 juillet 2024).

+++

## Logiciel

+++L’appareil HP Z Captis nécessite-t-il un abonnement ou une licence logicielle pour être utilisé ?
L’appareil Captis nécessite une licence Substance 3D Sampler Enterprise, Teams ou University active, disponible dans la collection Substance 3D dans les mêmes conditions d’utilisation que tout abonnement Substance 3D.

Le périphérique (HP Z Captis) et la licence (Substance 3D Sampler) sont vendus séparément.

+++

+++Quel est le niveau d’intégration existant avec la suite de Substances d’Adobe ?
Le périphérique HP Z Captis est entièrement contrôlé et exploité par Adobe Substance 3D Sampler : vous pouvez prévisualiser et lancer la capture à partir de Substance 3D Sampler. Une fois la capture terminée, il charge automatiquement les canaux PBR en tant que calque et crée un matériau 3D. Vous pouvez continuer à traiter vos matières avec tous les outils et filtres disponibles dans Sampler.

Une fois que votre matériel capturé est dans Substance 3D Sampler, vous pouvez l’exporter vers n’importe quelle application de la suite Substance 3D (Substance 3D Designer, Painter, Stager) et vers n’importe quelle application tierce prenant en charge les Substances, notamment 3DS Max, Maya, Blender, Unreal Engine, CLO, Browzwear, VRED, Rhino, Cinema4D et bien d’autres (voir la liste complète ici : <https://www.adobe.com/fr/products/substance3d/plugins.html>).

+++

+++Quelles sont les spécifications recommandées pour l’utilisation de Substance 3D Sampler avec Captis ?
Les spécifications matérielles de Sampler sont disponibles [ici](system-requirements-to-use-hp-z-captis.md).

+++

+++Le workflow HP Z Captis est-il disponible sous Windows et Mac ?
À compter de la version du 20 février 2025, le workflow Sampler avec HP Z Captis est disponible uniquement sous Windows.

+++

+++Où puis-je trouver la version du workflow Substance 3D Sampler avec HP Z Captis ?
À partir de la version du 20 février 2025, vous pouvez accéder au workflow Adobe Substance 3D Sampler avec Captis dans le cadre des versions régulières de Substance 3D Sampler, téléchargées à partir de l’application de bureau Creative Cloud. Il n’est plus nécessaire de les télécharger à partir de la version préliminaire d’Adobe.

+++

+++Qu’est-ce qui n’est pas encore disponible ?
*Limitations en août 2025 (version de Sampler 5.1.0) :*

* Le workflow Sampler avec HP Z Captis est disponible sur Windows uniquement pour le moment.

* Les cinq textures exportées aujourd’hui sont les suivantes : Couleur de base, Rugosité, Normal, Height et Opacité.

* Le mode Explorateur est encore une version antérieure et n’est pas encore optimisé.

* Les mosaïques sont réalisées dans une pile de calques Sampler à l’aide des filtres de mosaïque actuels.

+++

+++Quels canaux PBR sont disponibles ?
Depuis la version du 7 août 2025, les cinq mappages exportés sont les suivants : Couleur de base, Rugosité, Normal, Height et Opacité. Le pipeline de traitement actuel ne gère pas encore le mappage de métallisation.

+++

+++La création de mosaïques est-elle automatique ?
La juxtaposition est effectuée dans la pile de calques Sampler à l’aide des filtres de juxtaposition actuels.

Le filtre Mosaïque automatique peut être utilisé pour mosaïquer automatiquement des matériaux avec une structure répétitive définie ou de petits motifs, avec un minimum de 3 motifs dans chaque direction. Pour en savoir plus sur ce filtre, consultez la [section dédiée de la documentation](../../filters/tools/auto-tiling.md).

+++

+++Quels formats les matériaux numérisés peuvent-ils être exportés ?
HP Z Captis est géré en mode natif par Adobe Substance 3D Sampler. HP Z Captis capture 64 images brutes (qui peuvent être récupérées dans votre dossier local) et cartes PBR (qui sont traitées à partir des images brutes capturées et qui sont chargées automatiquement dans Substance 3D Sampler). Substance 3D Sampler crée un matériau 3D basé sur les canaux PBR qui sont automatiquement chargés dans la pile de calques Sampler après la capture.

Depuis Adobe Substance 3D Sampler, vous pouvez exporter vos documents numériques dans n’importe quel format d’exportation disponible dans Substance 3D Sampler : sous forme de fichiers de Substance de données (fichiers .SBS et .SBSAR) ou de textures bitmap, notamment .PNG, .JPG, .TIFF.. (consultez les détails sur la page Web de la documentation Sampler : [https://helpx.adobe.com/fr/substance-3d-sampler/getting-started/export.html](../../getting-started/export/export.md)).

+++

+++Quelle est la différence entre LDR et HDR lors de la capture ?
Lors de la prévisualisation, vous avez la possibilité de choisir le type de sortie entre LDR (plage dynamique basse) et HDR (plage dynamique élevée).\
Même si LDR est choisi, les cartes HDR seront capturées et enregistrées sur votre appareil.\
Il est conseillé de sélectionner le LDR, car cela rendra la taille du projet plus gérable dans Sampler et dans toute application tierce où le fichier sbsar sera utilisé.

+++

## En cours de traitement

+++Comment puis-je utiliser Captis dans mon pipeline 3D actuel si j’utilise des formats de fichiers, des normes et des spécifications spécifiques ou des applications tierces ?
HP Z Captis est géré en mode natif par Adobe Substance 3D Sampler. Une fois que vous avez capturé et numérisé votre échantillon de matière dans Substance 3D Sampler, vous pouvez exporter vos matières numériques en toute transparence :

Dans toutes les applications de l’écosystème Substance 3D (y compris Substance 3D Designer ou Substance 3D Painter qui prennent en charge divers formats d’exportation : https://experienceleague.adobe.com/fr/docs/substance-3d/general-knowledge/ecosystem/import-and-export-formats).

Dans toutes les applications intégrant un format de fichier de Substance comme 3DS Max, Maya, Blender, C4D, Rhino, Browzwear, CLO... (voir la liste complète ici : <https://www.adobe.com/fr/products/substance3d/plugins.html>). Si vous utilisez une application qui n’est pas répertoriée ici, vous pouvez toujours exporter des images de texture PBR et les brancher manuellement dans les applications qui ne prennent pas en charge le format de fichier de Substance de données en mode natif.

+++

+++Combien de photos sont prises pour créer les cartes ?
[8 panneaux lumineux + 1 contre-jour] x [8 états de polarisation] x [8 expositions en bracketing pour HDR] x [4 surprises pour réduire le bruit] = 2048 + 256 (pour contre-jour)

+++

## Gestion des appareils

En savoir plus sur l&#39;appareil et ses spécifications sur le [site Web HP](https://www.hp.com/us-en/workstations/z-captis.html "HP Z Captis").

+++Puis-je modifier l’adresse IP de l’appareil ?
Pour modifier l&#39;adresse IP du périphérique, vous pouvez modifier le fichier Windows C:\Windows\System32\drivers\etc\hosts.txt en ajoutant une ligne supplémentaire :

Par exemple, vous pouvez ajouter 192.168.55.1 captis-device, puis dans <b>Paramètres de Sampler > Stockage et cache > Capture de matériel > Adresse Captis</b>, remplacer l’adresse IP par captis-device

+++

## Problèmes d’utilisation

+++Sampler ne détecte pas HP Z Captis.
Assurez-vous que le HP Z Captis est connecté à un port USB 3.0.

Assurez-vous que le câble USB est connecté à la base du HP Z Captis et non au cône.

+++

+++Mon aperçu est complètement noir dans la fenêtre de Sampler.
Assurez-vous que la protection de l’appareil photo a été supprimée.

+++

+++La copie de fichiers du HP Z Captis sur mon ordinateur est lente.
Assurez-vous que le HP Z Captis est connecté à un port USB 3.0.

Si vous avez demandé à récupérer à la fois la matière et les images photométriques, il est normal que la copie prenne plus de temps.

+++

+++Sampler n’a pas copié les images sur mon ordinateur. Dois-je redémarrer l’analyse ?
Non, pas du tout. Vous pouvez parcourir le contenu de l’appareil et copier les images trouvées dans le dossier Adobe à l’aide de l’explorateur de fichiers de votre système d’exploitation.

+++

+++Le menu indique que le périphérique est en mode de récupération.
Appuyez sur le bouton d&#39;alimentation quelques secondes pour l&#39;éteindre. Rallume-le.

+++

+++J&#39;ai déplacé le cône de sa base vers l&#39;anneau de l&#39;explorateur et je ne peux plus le scanner.
Il est recommandé de désactiver le HP Z Captis avant de le débrancher de sa base ou de l&#39;explorateur ring.

+++

+++L&#39;exportation de mon matériel dans SBSAR est lente.
Assurez-vous que les images ne sont pas au format flottant 32 bits dans le panneau Propriétés.

Vous pouvez également définir le niveau de compression sur « aucun » pour accélérer l’exportation.

+++

+++Je veux modifier le chemin d’enregistrement des matériaux capturés et des images photométriques.
Il est désormais possible de modifier l’emplacement où les matériaux capturés et les images de photométrie seront enregistrées, dans Modifier > Préférences > Stockage et cache > Acquisition de matériau.

+++

+++La fenêtre est plus grande que mon écran et je ne peux pas la redimensionner.
La fenêtre Captivate n’est en effet pas redimensionnable. Vous utilisez peut-être un agrandissement d’écran qui n’est pas géré. Captis prend en charge les éléments suivants :

* Résolution : 1 920 x 1 080
  * Agrandissement maximal : 100 %

* Agrandissement maximal : 100 %

* Résolution : 2 560 x 1 440
  * Agrandissement maximal : 125 %

* Agrandissement maximal : 125 %

* Résolution : 3 840 x 2 160
  * Agrandissement maximal : 200 %

* Agrandissement maximal : 200 %

* Les résolutions inférieures à 1 920 x 1 080 ne sont pas prises en charge.



+++
