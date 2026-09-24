---
helpx_url: 'https://helpx.adobe.com/fr/substance-3d-sampler/release-notes/all-changes.html'
breadcrumb-title: ''
description: Passez en revue toutes les modifications et mises à jour des versions de Substance 3D Sampler pour suivre l’évolution des fonctionnalités et les améliorations au fil du temps.
helpx_description: Sampler > Release Notes > All Changes
title: Toutes les modifications
user-guide-description: ''
user-guide-title: ''
source-git-commit: 275dc218870f111aa99533840a5aea4c3d22f0cf
workflow-type: tm+mt
source-wordcount: '24964'
ht-degree: 0%
---

# Toutes les modifications

Cette page regroupe toutes les modifications apportées à Substance 3D Sampler, depuis les nouvelles fonctionnalités jusqu’aux correctifs de bogues.

## Version 6

### **6.0.4**

*(sortie : 24 septembre 2026)*

**Modifié**
Mise à jour de la Substance Engine de [Moteur] vers la version 9.6.1

**Fixe**
crash [Calques] lors de l’ajout d’une image au masque embossage
[Correctifs généraux de sécurité]

### **6.0.3**

*(sortie : 24 août 2026)*

**Fixe :**

[Rendu] : solution de contournement temporaire inversée pour les pilotes NVIDIA défectueux

### **6.0.2**

*(sortie : 25 juin 2026)*

**Ajouté :**

* &amp;lbrack ; Assets&amp;rbrack ; Vérifiez la version sbsar et avertissez les utilisateurs que le moteur est trop ancien pour le lire
* &amp;lbrack ; Captis&amp;rbrack ; Add back option pour enregistrer la photométrie Captis dans les préférences

**Fixe :**

* &amp;lbrack ; vue 2D&amp;rbrack ; Ne pas « afficher avec le rapport physique » si la taille physique est désactivée
* &amp;lbrack ; Analytics&amp;rbrack ; Événements d&#39;analyse manquants
* &amp;lbrack ; Analytics&amp;rbrack ; Prevent crashpad to report a crash on vk devicelost
* &amp;lbrack ;Application&amp;rbrack ; Ne détruisez pas vkdevices à la sortie pour éviter un crash dans le pilote nvidia
* &amp;lbrack ; Application&amp;rbrack ; Réparer la sortie de l&#39;observateur de collection lié + gestionnaire de canaux
* &amp;lbrack ;Application&amp;rbrack ; Empêcher un crash à la sortie
* Le filtre &amp;lbrack ; Content&amp;rbrack ; « metal finish » n&#39;a pas d&#39;impact sur le métal
* &amp;lbrack ;Content&amp;rbrack ; Ajouter de la taille physique aux filtres dynamiques où elle est manquante
* &amp;lbrack ; Filters&amp;rbrack ; Supprimer le remplissage d&#39;après le contenu de la liste des actifs masqués
* &amp;lbrack ; Layers&amp;rbrack ; Cliquer sur &#39;réinitialiser tous les paramètres&#39; ne réinitialise pas la liste déroulante &#39;s&#39;applique à&#39;
* &amp;lbrack ; Layers&amp;rbrack ; Fix tweak min &amp; max for position widget
* &amp;lbrack ; Layers&amp;rbrack ; Mise à jour correcte du filtre
* &amp;lbrack ; Taille physique&amp;rbrack ; S’assurer que l’échelle physique fonctionne partout + rendre la taille physique correcte avec des filtres dynamiques
* &amp;lbrack ;Project&amp;rbrack ; Vérifier que la résolution de l&#39;actif est la résolution par défaut (2k x 2k) lors de la création d&#39;un nouvel actif
* &amp;lbrack ;Project&amp;rbrack ; Rouvrir le projet en cours utilisé pour ouvrir la version précédente
* &amp;lbrack ; Project&amp;rbrack ; Sampler ne propose plus de restaurer une sauvegarde de projets corrompus
* &amp;lbrack ; Rendu&amp;rbrack ; Rendu de la vignette du matériau à une résolution maximale de 2k
* &amp;lbrack ;UI&amp;rbrack ; Code défensif pour éviter les crashs si l&#39;utilisateur est plus rapide que l&#39;interface utilisateur

### **6.0.1**

*(Publié le 21 mai 2026)*

**Ajouté :**

* &amp;lbrack ;Application&amp;rbrack ; Avertir l’utilisateur lors de l’ouverture d’un projet avec des objets ou des éclairages d&#39;environnement 3D
* &amp;lbrack ; Captis&amp;rbrack ; Adapter l&#39;interface utilisateur aux petits écrans
* &amp;lbrack ; Captis&amp;rbrack ; Mettre à jour l&#39;interface utilisateur Captis
* &amp;lbrack ; Channel Settings&amp;rbrack ; Active automatiquement SSS lorsque vous utilisez le canal SSS dans ASM
* &amp;lbrack ;Moteur&amp;rbrack ; Mettre à jour la Substance Engine à la version 9.4.3
* &amp;lbrack ; Preset&amp;rbrack ; Activer par défaut l&#39;option « Appliquer les valeurs des vignettes prédéfinies »
* &amp;lbrack ;Resources&amp;rbrack ; Affiche « toutes les bibliothèques » par défaut au lieu de « ressources de démarrage » dans le panneau Ressources
* &amp;lbrack ; Scripting&amp;rbrack ; Ajout de fonctions Python pour gérer « Appliqué à » d&#39;un calque
* La liste des actifs &amp;lbrack ; de l&#39;interface utilisateur est désormais réactive : la taille de l&#39;actif s&#39;adapte au conteneur
* &amp;lbrack ;UI&amp;rbrack ; Afficher 3D/Vue 2D par défaut
* &amp;lbrack ;UI&amp;rbrack ; Affiche la fenêtre contextuelle d&#39;optimisation du matériau lors de la suppression d&#39;un matériau de l&#39;explorateur
* &amp;lbrack ; UI&amp;rbrack ; Activer le basculement de l&#39;info-bulle des boutons de la barre de périphériques

**Fixe :**

* &amp;lbrack ; Application&amp;rbrack ; Résoudre les problèmes d&#39;espace colorimétrique
* &amp;lbrack ; Application&amp;rbrack ; Correction du programme de mise à jour des paramètres
* &amp;lbrack ; Application&amp;rbrack ; Active les canaux de numérisation lorsqu&#39;ils sont réglés sur auto
* &amp;lbrack ; Application&amp;rbrack ; Le bouton Nouveau projet de l&#39;écran d&#39;accueil n&#39;efface plus le projet précédent portant le même nom
* &amp;lbrack ;Application&amp;rbrack ; Empêcher un crash à la fermeture sur macOS
* &amp;lbrack ;Application&amp;rbrack ; Empêcher l&#39;accès aux ressources dont les références ne sont pas valides
* &amp;lbrack ;Application&amp;rbrack ; Empêcher le crash lors de l&#39;accès à la surface à partir de VersionedImage dans une modification
* &amp;lbrack ;Application&amp;rbrack ; Empêcher le crash lors de la suppression d&#39;une scène lorsqu&#39;il n&#39;y en a pas
* &amp;lbrack ;Captis&amp;rbrack ; Vérifiez que Captis est déconnecté avant de fermer Sampler
* &amp;lbrack ;Captis&amp;rbrack ; Empêcher l&#39;affichage répété de l&#39;avertissement USB-2
* &amp;lbrack ; Channel Settings&amp;rbrack ; Fix OpenPBR channel names
* &amp;lbrack ; Channel Settings&amp;rbrack ; Update long labels for OpenPBR channels
* &amp;lbrack ;Content&amp;rbrack ; Mettez à jour toutes les unités de maillage des mètres aux centimètres pour les valeurs SSS
* &amp;lbrack ; Export&amp;rbrack ; Vérifier que les valeurs par défaut sont connectées aux filtres dynamiques
* Les images &amp;lbrack ; Export&amp;rbrack ; sont désormais enregistrées dans un thread de travail pour de meilleures performances
* &amp;lbrack ; Filters&amp;rbrack ; crashs de remplissage d&#39;après le contenu lors de l&#39;activation de l&#39;échelle
* &amp;lbrack ; Filters&amp;rbrack ; Impossible d&#39;ouvrir l&#39;emplacement d&#39;un filtre dynamique à partir du panneau des actifs
* &amp;lbrack ; Filters&amp;rbrack ; Réinitialiser tout à l&#39;étape de réglage Limites automatiques
* &amp;lbrack ; Filters&amp;rbrack ; Restore désactive le traitement d&#39;utilisation dans la création de structures arborescentes
* &amp;lbrack ; Filters&amp;rbrack ; Définissez la valeur par défaut correcte pour le paramètre de mise à l&#39;échelle
* &amp;lbrack ; Filters&amp;rbrack ; Mettez à jour les générateurs même s&#39;ils se trouvent dans un calque de remplissage
* &amp;lbrack ; Layers&amp;rbrack ; Interdire de renommer les calques d&#39;en-tête ou de substitution d&#39;entrée
* &amp;lbrack ; Layers&amp;rbrack ; Empêcher le crash pendant l&#39;insertion de calques en raison d&#39;un pointeur balancé
* &amp;lbrack ; Layers&amp;rbrack ; Nombre incorrect d&#39;images dans le nom aplatir le calque
* &amp;lbrack ; Localization&amp;rbrack ; Vérifier que les noms du paramètre prédéfini sont mis à jour lors du changement de langue
* &amp;lbrack ; Localization&amp;rbrack ; Multiple translation issues in resources panel
* &amp;lbrack ; Localization&amp;rbrack ; Quick Actions catégories problèmes de localisation
* &amp;lbrack ; Performance&amp;rbrack ; Charge les réglages uniquement dans la section ouverte
* &amp;lbrack ; Préférences&amp;rbrack ; Effacer le chemin de cache des préférences rétablit la valeur précédente
* &amp;lbrack ; Rendu&amp;rbrack ; Fuite de mémoire lors de l’utilisation du traceur de chemin
* &amp;lbrack ;Rendering&amp;rbrack ; Empêcher la suppression des textures lorsque Vulkan y accède encore
* La rotation de la Texture de &amp;lbrack ;Rendering&amp;rbrack ; n&#39;a pas été convertie de 0-1 à 0-360
* &amp;lbrack ; Scripting&amp;rbrack ; Supprimer les classes inexistantes de la documentation Python
* &amp;lbrack ; Scripting&amp;rbrack ; selectedAsset renvoie Aucun s&#39;il n&#39;y a pas d&#39;actif sélectionné
* &amp;lbrack ;Tools&amp;rbrack ; La réinitialisation d&#39;une valeur de texture arrête désormais la peinture et efface la vue de la pièce
* &amp;lbrack ; UI&amp;rbrack ; Ne fermez pas les sections du panneau des propriétés chaque fois qu&#39;un élément est modifié
* &amp;lbrack ; UI&amp;rbrack ; étiquette de réglage des couleurs Exposée invisible au survol
* &amp;lbrack ; UI&amp;rbrack ; Corriger le comportement réactif de la liste des actifs
* &amp;lbrack ; UI&amp;rbrack ; Corriger la boucle de liaison dans l&#39;info-bulle AssetItem
* &amp;lbrack ; UI&amp;rbrack ; Corriger le double clic sur le groupe de paramètres prédéfinis sélectionné
* &amp;lbrack ; UI&amp;rbrack ; Corriger la zone de dépôt dans le présentateur d&#39;images
* &amp;lbrack ; UI&amp;rbrack ; Corriger l’étiquette avec un bouton dans toutes les langues
* &amp;lbrack ;UI&amp;rbrack ; Corriger l’height de la ligne pour le japonais dans la fenêtre contextuelle de la liste des canaux
* &amp;lbrack ; UI&amp;rbrack ; Fixe sur le champ de longueur de signal accepté
* &amp;lbrack ; UI&amp;rbrack ; Corriger la largeur de la fenêtre contextuelle avec un long élément de contrôle gauche
* &amp;lbrack ; UI&amp;rbrack ; Corriger la fenêtre contextuelle d&#39;aperçu dans les éléments de ressource
* &amp;lbrack ; UI&amp;rbrack ; Correction du sélecteur brut/réfléchissant
* &amp;lbrack ; UI&amp;rbrack ; Corriger les points de suspension
* &amp;lbrack ; UI&amp;rbrack ; Résoudre le problème de troncature de chaîne
* &amp;lbrack ; UI&amp;rbrack ; Corriger le bouton de réinitialisation des réglages du commutateur
* &amp;lbrack ; UI&amp;rbrack ; Masque le menu déroulant par Modèle de matériau lorsqu&#39;un paramètre prédéfini d&#39;exportation personnalisé est sélectionné
* &amp;lbrack ; UI&amp;rbrack ; Supprimer la résolution dans la liste des canaux de la fenêtre contextuelle d&#39;exportation
* &amp;lbrack ;UI&amp;rbrack ; La réinitialisation de la disposition par défaut conserve les paramètres de la visionneuse de projections
* &amp;lbrack ; UI&amp;rbrack ; Restaurer les éléments de menu « Modifier dans Photoshop » et « Modifier dans Illustrator »

**Supprimé(e) :**

* &amp;lbrack ; UI&amp;rbrack ; Supprimer la section « Appliqué à » pour les calques d&#39;importation d&#39;image
* &amp;lbrack ; UI&amp;rbrack ; Supprimer l&#39;info-bulle d&#39;action rapide à ouverture automatique au premier lancement

## Version 5

### **5.1.3 ÎLE FLOTTANTE**

*(Publié Le 6 Janvier 2026)*

**Ajouté :**

* &amp;lbrack ; Captis&amp;rbrack ; Affiche un avertissement si le protocole FTP est désactivé par le pare-feu

**Fixe :**

* &amp;lbrack ; Captis&amp;rbrack ; L&#39;abandon pendant une capture peut entraîner des erreurs
* &amp;lbrack ;Captis&amp;rbrack ; Le téléchargement des résultats à la fin d&#39;une capture utilise trop de RAM
* &amp;lbrack ;Captis&amp;rbrack ; L&#39;exécution d&#39;une mise au point automatique immédiatement après une intensité automatique peut entraîner des erreurs
* &amp;lbrack ; Captis&amp;rbrack ; L&#39;affichage des résultats HDR dans le panneau Résumé
* &amp;lbrack ;UI&amp;rbrack ; Dans certains cas, la boîte de dialogue de dossier sur MacOS ne sélectionne pas le bon dossier

### **5.1.2 ÎLE FLOTTANTE**

*(sortie : 20 novembre 2025)*

**Ajouté :**

* &amp;lbrack ;Application&amp;rbrack ; Détecte la perte du périphérique graphique, avertit l&#39;utilisateur et quitte l&#39;application avec élégance
* &amp;lbrack ; Layers&amp;rbrack ; Amélioration des messages lors de l&#39;aplatissement des calques
* &amp;lbrack ; Layers&amp;rbrack ; Amélioration des vignettes pour l&#39;importation d&#39;images et l&#39;aplatissement des calques
* &amp;lbrack ; Onboarding&amp;rbrack ; Contenu d’apprentissage mis à jour sur l’écran d’accueil
* &amp;lbrack ;Project&amp;rbrack ; Récupérer le dernier état enregistré de la session avant le crash
* &amp;lbrack ; UI&amp;rbrack ; Mise à jour de l&#39;icône d&#39;application

**Fixe :**

* &amp;lbrack ;Application&amp;rbrack ; L&#39;insertion d&#39;un matériau dans la pile de calques de données peut entraîner un crash sur macOS
* &amp;lbrack ;Application&amp;rbrack ; crash possible en cas de forte charge sur macOS
* &amp;lbrack ; Application&amp;rbrack ; crash possible lors de l&#39;ajout de calques lorsque la mémoire vidéo est pleine
* &amp;lbrack ; Application&amp;rbrack ; crash possible lors de l&#39;ouverture d&#39;un projet
* &amp;lbrack ; Captis&amp;rbrack ; Échec si la mise au point automatique est exécutée peu après l&#39;étalonnage automatique de l&#39;intensité
* &amp;lbrack ; Captis&amp;rbrack ; Problèmes de fiabilité et de performances après la première capture
* &amp;lbrack ; Captis&amp;rbrack ; Ralentissements et erreurs lors de la copie de fichiers à la fin d&#39;une capture
* &amp;lbrack ; Captis&amp;rbrack ; Petite fuite de mémoire lors de l&#39;interrogation des informations de l&#39;appareil Captis
* Les paramètres exposés à curseurs multiples &amp;lbrack ; Export&amp;rbrack ; produisent des fichiers .sbsar corrompus
* &amp;lbrack ; Layers&amp;rbrack ; Le motif de répétition automatique est réinitialisé aux valeurs par défaut lors du changement d&#39;actifs
* &amp;lbrack ; Layers&amp;rbrack ; La base color personnalisée par défaut est affichée en rouge
* &amp;lbrack ; Layers&amp;rbrack ; L&#39;aplatissement partiel des calques enfants de tampon de Clone est possible et entraîne des problèmes de rendu
* &amp;lbrack ; Layers&amp;rbrack ; crash possible lors du réglage d&#39;une pile de calques pendant le rendu
* &amp;lbrack ; Layers&amp;rbrack ; Erreur inattendue lors de l&#39;étape de zone d&#39;intérêt de répétition automatique lors de la modification des canaux sources
* &amp;lbrack ;Project&amp;rbrack ; Miniature incorrecte parfois lors de la création d&#39;un nouveau matériau
* &amp;lbrack ; Actions rapides&amp;rbrack ; Certaines actions rapides ont un nombre de saisie incorrect
* Le bouton du groupe d&#39;actions &amp;lbrack ; UI&amp;rbrack ; a des largeurs différentes
* Le bouton &amp;lbrack ; UI&amp;rbrack ; Effacer dans les champs de texte déclenche parfois une perte de focus
* &amp;lbrack ; UI&amp;rbrack ; Les zones de liste déroulante et les champs de texte sont trop grands
* Les icônes et les libellés de l&#39;&amp;interface utilisateur&amp;rbrack ; sont mal alignés
* L&#39;étiquette du champ Nom de l&#39;&amp;interface utilisateur &amp;brack ; n&#39;est pas placée correctement
* Les libellés des boutons d&#39;actions rapides &amp;lbrack ; UI&amp;rbrack ; sont mal alignés
* Les curseurs &amp;lbrack ; UI&amp;rbrack ; montrent des 0 de fin trop décalés

**Supprimé(e) :**

* &amp;lbrack ; Generative AI&amp;rbrack ; Suppression des fonctionnalités d’IA générative. *Cette fonctionnalité a été supprimée de l&#39;application et le service cessera de fonctionner dans les versions précédentes de Sampler le 5 mars.*

### **5.1.1 ÎLE FLOTTANTE**

*(sortie : 18 septembre 2025)*

**Ajouté :**

* &amp;lbrack ; vue 2D&amp;rbrack ; Possibilité d&#39;effectuer un zoom arrière plus important dans Vue 2D pour des textures haute résolution
* &amp;lbrack ; Captis&amp;rbrack ; Avertit les utilisateurs des problèmes lors de la copie de fichiers
* &amp;lbrack ; Layers&amp;rbrack ; Lors de la duplication d&#39;un calque, utilisez un numéro incrémentiel dans le nouveau nom du calque

**Fixe :**

* &amp;lbrack ; vue 2D&amp;rbrack ; Lorsque vous peignez des contours après avoir réinitialisé toutes les propriétés de Tampon de Clone, les contours créés précédemment réapparaissent
* &amp;lbrack ; Application&amp;rbrack ; « Enregistrer le projet actuel ? » la fenêtre contextuelle utilise un nom de projet incorrect
* &amp;lbrack ; Application&amp;rbrack ; Crash à la sortie
* &amp;lbrack ;Application&amp;rbrack ; crash potentiel
* &amp;lbrack ;Application&amp;rbrack ; Parfois, une vignette est générée avec un matériau incorrect
* &amp;lbrack ;Captis&amp;rbrack ; Sur certains appareils, lorsque vous effectuez une numérisation en haute résolution, la map height est noire
* &amp;lbrack ;Captis&amp;rbrack ; Le bouton « Démarrer la capture » n&#39;est plus désactivé lorsqu&#39;aucun nom de capture n&#39;est défini et qu&#39;un étalonnage est en cours d&#39;exécution
* &amp;lbrack ; Export&amp;rbrack ; Lors de l&#39;exportation d&#39;un fichier .fichier sbsar, l&#39;exportation peut échouer sans que l&#39;utilisateur en soit averti
* &amp;lbrack ; Filters&amp;rbrack ; L’écran des paramètres avancés du filtre Répétition automatique scintille parfois lors de l’ajustement des paramètres
* &amp;lbrack ; Filters&amp;rbrack ; Les paramètres par défaut du filtre Répétition produisent des artefacts gris dans la sortie
* &amp;lbrack ;Filters&amp;rbrack ; Parfois, avec des entrées haute résolution, les paramètres avancés du filtre Répétition automatique n&#39;affichent pas les points de motif individuels
* &amp;lbrack ; Filters&amp;rbrack ; La taille du motif pour le paramètre de Répétition automatique de la taille personnalisée a une valeur par défaut incorrecte
* &amp;lbrack ; Layers&amp;rbrack ; Problème de couleur occasionnel avec le filtre Répétition automatique principalement visible sur les matériaux rouges
* &amp;lbrack ; Layers&amp;rbrack ; Parfois, l&#39;ajout de calques réinitialise certaines modifications à leur valeur par défaut
* &amp;lbrack ; Taille physique&amp;rbrack ; La vignette des actifs avec une taille physique a une échelle d’height incorrecte
* &amp;lbrack ; UI&amp;rbrack ; Impossible de renommer les paramètres exposés
* Le bouton d&#39;activation du canal &amp;lbrack ; UI&amp;rbrack ; n&#39;est pas carré
* &amp;lbrack ; UI&amp;rbrack ; Si un libellé de curseur est trop long, le bouton de réinitialisation n&#39;est pas accessible
* &amp;lbrack ; UI&amp;rbrack ; Appuyer sur la touche Retour ou cliquer dehors ne supprime pas le focus des champs de texte
* &amp;lbrack ; UI&amp;rbrack ; Parfois, une info-bulle indésirable apparaît dans le panneau Taille physique
* &amp;lbrack ;UI&amp;rbrack ; La vue 3D affiche un maillage incorrect lors de la création d’un projet vide
* &amp;lbrack ;UI&amp;rbrack ; Lorsque vous exposez une entrée de sélecteur de couleurs, son libellé disparaît au survol
* &amp;lbrack ;UI&amp;rbrack ; Lorsque vous exposez des paramètres, le point de couleur est parfois mal positionné

### **5.1.0 ÎLE FLOTTANTE**

*(sortie : 7 août 2025)*

**Ajouté :**

* &amp;lbrack ; vue 2D&amp;rbrack ; La taille du pinceau s&#39;adapte désormais à la résolution de texture actuelle
* &amp;lbrack ;vue 3D&amp;rbrack ; Activer l&#39;échelle d&#39;affichage native pour le rendu 3D dans les préférences
* &amp;lbrack ;Application&amp;rbrack ; mise à jour du Moteur de rendu
* &amp;lbrack ; Captis&amp;rbrack ; Ajouter la possibilité de « rendre carré » pendant l’aperçu
* &amp;lbrack ;Captis&amp;rbrack ; Détection automatique des tailles physiques
* &amp;lbrack ;Captis&amp;rbrack ; La capture d&#39;un nouveau matériau entraînera la création d&#39;une nouvelle ressource
* &amp;lbrack ; Captis&amp;rbrack ; Modifier la sélection de résolution dans la liste déroulante en pixels par pouce ou centimètre au lieu de la résolution en pixels de la zone maximale
* &amp;lbrack ; Captis&amp;rbrack ; Aide contextuelle sur l&#39;étalonnage de l&#39;alignement
* &amp;lbrack ; Captis&amp;rbrack ; Générer le mappage de rugosité
* &amp;lbrack ; Captis&amp;rbrack ; Avertit l&#39;utilisateur si les fichiers d&#39;étalonnage par défaut sont manquants
* &amp;lbrack ; Filters&amp;rbrack ; Filtre de Répétition automatique pour les matériaux et les numérisations structurés
* &amp;lbrack ; Filters&amp;rbrack ; Nouveau filtre Suppresseur de plis
* &amp;lbrack ; Filters&amp;rbrack ; Nouvelles fonctionnalités du filtre Tampon de Clone
* &amp;lbrack ; Filters&amp;rbrack ; Nouvelles fonctionnalités du filtre Égaliser
* &amp;lbrack ; Layers&amp;rbrack ; Possibilité d&#39;aplatir les calques
* &amp;lbrack ; Calques&amp;rbrack ; Menu contextuel lorsque vous cliquez avec le bouton droit de la souris sur un calque pour le renommer, le dupliquer, le supprimer ou l&#39;aplatir
* &amp;lbrack ; Onboarding&amp;rbrack ; Update Welcome and What&#39;s New screens content
* &amp;lbrack ; Performance&amp;rbrack ; Meilleures performances lors de l&#39;utilisation du filtre Recadrage
* &amp;lbrack ; Performance&amp;rbrack ; Améliorer l&#39;utilisation de la mémoire pour la vue 3D
* &amp;lbrack ; Performance&amp;rbrack ; La mise à jour de la vue 3D est plus rapide
* &amp;lbrack ; Taille physique&amp;rbrack ; Activer « afficher avec rapport physique » lors de l&#39;utilisation de filtres de Substance lorsque la Taille physique est activée
* &amp;lbrack ; Taille physique&amp;rbrack ; Lors de l&#39;importation d&#39;images dans une pile vide, proposer une résolution plus cohérente avec le rapport d&#39;image
* &amp;lbrack ;Quick Actions&amp;rbrack ; 3 nouvelles actions rapides pour le traitement de la numérisation
* &amp;lbrack ; Scripting&amp;rbrack ; API pour aplatir les calques
* &amp;lbrack ; Scripting&amp;rbrack ; Obtenir le nom de fichier de chaque image d&#39;un calque d&#39;importation d&#39;image
* &amp;lbrack ; Scripting&amp;rbrack ; Nouvelle fonction pour activer/désactiver un canal donné d&#39;une ressource
* &amp;lbrack ; UI&amp;rbrack ; Modifiez les icônes et les boutons du panneau Calques pour les adapter aux nouvelles fonctionnalités
* &amp;lbrack ; UI&amp;rbrack ; Avertir de la dépréciation de la création d&#39;éclairages d&#39;environnement

**Fixe :**

* &amp;lbrack ; vue 2D&amp;rbrack ; La sélection de « afficher avec rapport physique » peut ne pas fonctionner lors de l&#39;utilisation de filtres de Substance
* les fichiers &amp;lbrack ; capture 3D&amp;rbrack ; Svg sont répertoriés dans le sélecteur de fichiers mais ne sont pas pris en charge
* Le paramètre d&#39;intensité d&#39;émission de &amp;lbrack ; vue 3D&amp;rbrack ; dans les paramètres de Shader ne fonctionne pas
* &amp;lbrack ; vue 3D&amp;rbrack ; Parfois, la position du maillage est incorrecte lors de la création d&#39;un nouvel actif
* &amp;lbrack ; vue 3D&amp;rbrack ; basculement vers des crashs de rendu de traçage de chemin sur du matériel non pris en charge
* &amp;lbrack ; Application&amp;rbrack ; L&#39;application se bloque lors de la fermeture de la fenêtre contextuelle de mesure manuelle sans définir de taille
* &amp;lbrack ; Application&amp;rbrack ; Crash
* &amp;lbrack ; Application&amp;rbrack ; Se bloque sous Windows lors de l&#39;affichage du bureau (touche Windows + raccourci du clavier D)
* &amp;lbrack ; Application&amp;rbrack ; crash possible lors du changement de langue
* &amp;lbrack ;Captis&amp;rbrack ; Crash lorsque les données d&#39;aperçu ne sont pas valides
* &amp;lbrack ; Captis&amp;rbrack ; Impossible d&#39;effectuer un zoom arrière complet après un zoom avant
* &amp;lbrack ;Captis&amp;rbrack ; Localisation manquante sur certaines étapes de l&#39;Assistant
* &amp;lbrack ; Captis&amp;rbrack ; crash possible à la sortie lors de l&#39;utilisation de Captis
* L&#39;analyse &amp;lbrack ; Captis&amp;rbrack ; ne fonctionne pas si des fichiers d&#39;étalonnage sont manquants sur le périphérique
* L&#39;aperçu du pinceau &amp;lbrack ; Filters&amp;rbrack ; lors de l&#39;utilisation du filtre Tampon de Clone peut être erroné selon la texture et la taille du pinceau
* &amp;lbrack ; Filters&amp;rbrack ; Taille de sortie incorrecte après utilisation du filtre Mise à l&#39;échelle supérieure
* &amp;lbrack ; Filters&amp;rbrack ; Icônes manquantes pour les filtres de rotation et de stylisation de l&#39;environnement
* &amp;lbrack ; Filters&amp;rbrack ; La mise à jour de certains filtres peut entraîner un rendu incorrect
* &amp;lbrack ; Layers&amp;rbrack ; premier rendu incorrect lors de la fusion de deux matériaux
* &amp;lbrack ; Layers&amp;rbrack ; Le bouton de mise à jour des calques affiche « Tout mettre à jour » même s&#39;il n&#39;y a qu&#39;une seule mise à jour
* &amp;lbrack ; Layers&amp;rbrack ; calculs inutiles lors de l&#39;importation d&#39;images dans la pile de calques
* &amp;lbrack ; Performance&amp;rbrack ; Améliorer la gestion des formats de map normaux pour réduire les temps de rendu
* La fenêtre contextuelle de mesure manuelle de &amp;lbrack ; Taille physique&amp;rbrack ; ne fonctionne qu&#39;après avoir effectué une mesure automatique
* &amp;lbrack ; Taille physique&amp;rbrack ; mauvaise résolution d&#39;exportation dans la fenêtre contextuelle Exporter lorsque la Taille physique est activée
* &amp;lbrack ; Quick Actions&amp;rbrack ; Localisation manquante sur les noms d&#39;actifs générés
* L&#39;&amp;aperçu de la ressource i&amp;rbrack ; au survol peut ne pas s&#39;afficher
* &amp;lbrack ;UI&amp;rbrack ; Cliquer sur le bouton Rétablir la valeur par défaut peut interrompre certaines commandes
* Les messages d&#39;erreur &amp;lbrack ; UI&amp;rbrack ; ne sont pas effacés lors du changement de projet
* &amp;lbrack ;UI&amp;rbrack ; Vérifiez que le nom du matériau dans le panneau viewport et propriétés est vide lorsqu&#39;il n&#39;y a aucun actif
* &amp;lbrack ; UI&amp;rbrack ; Le bouton Réinitialiser la valeur par défaut pour le paramètre Point de vue ne fonctionne pas
* &amp;lbrack ; UI&amp;rbrack ; Rétablir la valeur par défaut du chevauchement des boutons
* &amp;lbrack ; UI&amp;rbrack ; Certains boutons ne sont pas cliquables lorsqu’un panneau n’est pas ancré
* &amp;lbrack ; UI&amp;rbrack ; Texture labour V Paramètre partiellement masqué dans les paramètres du visualiseur et dans vue 3D

**Supprimé(e) :**

* &amp;lbrack ; capture 3D&amp;rbrack ; Supprimer la prise en charge de capture 3D
* &amp;lbrack ;Application&amp;rbrack ; Supprimer la prise en charge de macOS x86

### **5.0.3 NOISETTE**

*(Publié le 3 juin 2025)*

**Ajouté :**

* &amp;lbrack ; Captis&amp;rbrack ; Permet de donner à un matériau le même nom qu&#39;un modèle existant
* &amp;lbrack ; Captis&amp;rbrack ; Déplace les messages d&#39;erreur vers les fenêtres contextuelles au lieu des toasts
* &amp;lbrack ; Filters&amp;rbrack ; Mettre à jour la broderie
* &amp;lbrack ; Preferences&amp;rbrack ; Add reset in viewer settings and shaders settings
* &amp;lbrack ; UI&amp;rbrack ; Ne présente pas l&#39;option de menu « Afficher l&#39;emplacement » sur les ressources du projet

**Fixe :**

* le filtre de post-traitement de Maillage &amp;lbrack ; capture 3D&amp;rbrack ; ne produit pas les mappages attendus
* La vue 3D &amp;lbrack ; vue 3D&amp;rbrack ; ne fonctionne pas en raison de la corruption du cache de shader
* &amp;lbrack ; vue 3D&amp;rbrack ; le plan et la grille du Sol sont verticaux lorsque la scène est en Z vers le haut
* &amp;lbrack ;vue 3D&amp;rbrack ; Le maillage disparaît parfois
* &amp;lbrack ;Application&amp;rbrack ; La fermeture de la fenêtre de connexion au démarrage sans connexion entraîne parfois le crash de l&#39;application
* &lbrack;Application&amp;rbrack ; Crash lorsque l&#39;accès au fichier de configuration des plug-ins est refusé
* &amp;lbrack ;Application&amp;rbrack ; Le matériau actuel n&#39;est pas sélectionné lorsque le projet est enregistré
* &amp;lbrack ;Application&amp;rbrack ; La réinitialisation à la disposition par défaut définit la résolution sur 64x64
* &amp;lbrack ;Application&amp;rbrack ; Sampler effectue parfois un crash lors du rendu d’une pile de calques
* &amp;lbrack ;Export&amp;rbrack ; La résolution d&#39;exportation est parfois réinitialisée à 64x64
* &amp;lbrack ; Export&amp;rbrack ; Il est parfois impossible d&#39;exporter des fichiers .sbs/.sbsar
* Le bouton &amp;lbrack ; Layers&amp;rbrack ; Add matériau de base ne fait rien lorsque le matériau est vide
* La répétition de Texture de &amp;lbrack ; Layers&amp;rbrack ; est modifiée lors de la duplication d&#39;un matériau
* La &amp;mesure automatique de Taille physique&amp;rbrack ; ne fonctionne pas si le panneau Taille physique était ancré avant l&#39;importation de l&#39;image
* &amp;lbrack ; Le plug-in Scripting&amp;rbrack ; Autosave est défectueux
* &amp;lbrack ; UI&amp;rbrack ; espacement incorrect dans la boîte de dialogue Exporter
* L&#39;animation des réglages par &amp;brack ; curseur de l&#39;interface utilisateur&amp;rbrack ; ne fonctionne plus
* Les curseurs &amp;lbrack ; UI&amp;rbrack ; ne contraignent pas sur des valeurs entiers si nécessaire
* &amp;lbrack ; UI&amp;rbrack ; Certains menus déroulants sont recadrés

### **5.0.2 NOISETTE**

*(sortie : 22 avril 2025)*

**Fixe :**

* Le bouton &amp;lbrack ; Application&amp;rbrack ; Précédent de la page d&#39;accueil est cassé
* &amp;lbrack ; Application&amp;rbrack ; Sampler ne se lance parfois pas si des données corrompues de versions précédentes sont présentes sur le disque
* &amp;lbrack ;Application&amp;rbrack ; L&#39;image importée n&#39;apparaît ni dans le viewport ni dans la pile de calques
* Le champ d&#39;adresse IP de &amp;lbrack ; Captis&amp;rbrack ; Captis reste vide même après le redémarrage de Sampler
* &amp;lbrack ;Captis&amp;rbrack ; L&#39;aperçu en direct des caméras ne fonctionne que lorsque la langue de l&#39;application est définie sur Anglais
* &amp;lbrack ; Export&amp;rbrack ; Crash pendant l&#39;exportation &amp;lbrack ; Layers&amp;rbrack ; Painting ne fonctionne parfois pas dans les projets précédemment enregistrés
* &amp;lbrack ; Layers&amp;rbrack ; Sampler met parfois à jour toutes les textures lorsqu&#39;une seule couche est mise à jour
* &amp;lbrack ; Layers&amp;rbrack ; Impossible d&#39;utiliser les dégradés par matériau dans la pile de calques après la mise à niveau vers la version 5.0.x
* &amp;lbrack ; Layers&amp;rbrack ; La mise à jour d&#39;un projet avec une version précédente d&#39;Image vers Matériau (AI) rend matériau tout noir
* &amp;lbrack ; Layers&amp;rbrack ; Lorsque vous tentez d’importer une image non prise en charge, Sampler crée un calque rompu
* &amp;lbrack ; La partie scripting&amp;rbrack ; de l&#39;API Python ne fonctionne pas avec un projet vide
* Les éléments de menu &amp;lbrack ;UI&amp;rbrack ; débordent parfois dans le menu Fichier

### **5.0.1 NOISETTE**

*(Publié le 20 mars 2025)*

**Ajouté**

* &amp;lbrack ;Application&amp;rbrack ; Liste de compatibilité du pilote graphique mise à jour
* &amp;lbrack ;Captis&amp;rbrack ; Affiche une fenêtre contextuelle lorsque l&#39;utilisation de HP Z Captis est bloquée par les stratégies du système d&#39;exploitation
* &amp;lbrack ; Actions rapides&amp;rbrack ; Expliquez pourquoi une action rapide est désactivée dans une info-bulle
* &amp;lbrack ;UI&amp;rbrack ; Crash style de l&#39;interface utilisateur de la fenêtre de rapport
* &amp;lbrack ; UI&amp;rbrack ; Lors de la copie dans le Presse-papiers, porter un toast pour dire que c&#39;est terminé

**Fixe :**

* Le curseur Exposition &amp;lbrack ; vue 2D&amp;rbrack ; n&#39;a aucun effet lorsque la projection sphérique est désactivée
* &amp;lbrack ; vue 2D&amp;rbrack ; Peindre en dehors de la texture crée un contour discontinu
* &amp;lbrack ; vue 2D&amp;rbrack ; Le bouton d&#39;exposition n&#39;a pas d&#39;info-bulle.
* &amp;lbrack ; vue 2D&amp;rbrack ; Le zoom latéral sur une image non carrée ne suit pas la souris
* &amp;lbrack ; capture 3D&amp;rbrack ; capture 3D ne fonctionne pas sous Windows 11 24H2
* &amp;lbrack ;capture 3D&amp;rbrack ; Crash si nous quittons Sampler pendant l&#39;étape de reconstruction du maillage
* &amp;lbrack ;vue 3D&amp;rbrack ; Le temps de calcul est parfois affiché sous la forme 0ms
* &amp;lbrack ;vue 3D&amp;rbrack ; Lorsque vous passez de la projection orthographique à la perspective, le viewport devient gris
* &amp;lbrack ; Application&amp;rbrack ; Crash au démarrage lors de la vérification des capacités GPU
* crash &amp;lbrack ; Application&amp;rbrack ; pendant l&#39;installation
* &lbrack;Application&amp;rbrack ; Crash à la fermeture après avoir cliqué avec le bouton droit sur un champ de métadonnées
* L&#39;Éclairage d&#39;environnement &amp;lbrack ;Application&amp;rbrack ; est manquant lors de l&#39;ouverture d&#39;un SBSAR à partir de l&#39;explorateur de fichiers du système d&#39;exploitation
* &amp;lbrack ;Application&amp;rbrack ; L&#39;ouverture d&#39;un fichier .sbsar pendant que Sampler est en cours d&#39;exécution modifie le paramètre de Répétition de Texture
* &amp;lbrack ; Captis&amp;rbrack ; Certaines métadonnées peuvent ne pas être transférées entre les étapes de capture
* &amp;lbrack ; Captis&amp;rbrack ; Le nom de l&#39;actif créé n&#39;est pas celui saisi dans le champ de métadonnées
* &amp;lbrack ;Content&amp;rbrack ; L&#39;exemple de projet demande une mise à jour du filtre mais est déjà à jour
* &lbrack;Filters&amp;rbrack ; Le filtre de réglage Normal/height n&#39;a pas d&#39;icône
* &amp;lbrack ; Layers&amp;rbrack ; Cannot change images in an image import layer
* crashs &amp;lbrack ; Layers&amp;rbrack ; lors de l&#39;utilisation du filtre Mise à l&#39;échelle
* &amp;lbrack ; Layers&amp;rbrack ; La mise en Matériau d&#39;un projet avec une ancienne image rend le matériau entièrement noir
* &amp;lbrack ; Rendering&amp;rbrack ; Le réglage d&#39;une pile de calques immédiatement après la création d&#39;une ressource interrompt le rendu
* &amp;lbrack ; Scripting&amp;rbrack ; Les crashs de plug-in d&#39;enregistrement automatique lorsqu&#39;il n&#39;y a aucun actif dans le projet
* La valeur de l&#39;&amp;épaisseur du pinceau est manquante dans la barre d&#39;outils Pinceau
* &amp;lbrack ;UI&amp;rbrack ; La modification de la langue de l’application ne met pas à jour certains libellés de l’écran d’accueil
* &amp;lbrack ; UI&amp;rbrack ; appuyer sur Echap ou Entrer dans les champs de texte du curseur ne perdra pas le focus
* &amp;lbrack ; UI&amp;rbrack ; Dans le panneau Propriétés, le bouton Tout réinitialiser et le libellé du nom de la ressource se chevauchent
* &amp;lbrack ;UI&amp;rbrack ; Problèmes lors de l’ancrage et de la désancrage de panneaux
* &amp;lbrack ; UI&amp;rbrack ; Le défilement dans un panneau d&#39;incrustation défile également dans la fenêtre sous-jacente
* &amp;lbrack ; UI&amp;rbrack ; Le passage en mode Liste dans la section Projets récents de l’écran d’accueil ne fonctionne pas
* &amp;lbrack ;UI&amp;rbrack ; L&#39;icône du bouton du mode d&#39;affichage Viewport affiche toujours 2D/3D

### **5.0.0 NOISETTE**

*(sortie : 20 février 2025)*

**Ajouté**

* &amp;lbrack ; Onboarding&amp;rbrack ; New Homepage avec un accès rapide au contenu de formation, aux exemples de projet, aux actions rapides et aux projets récents.
* &amp;lbrack ; Onboarding&amp;rbrack ; Démarrez rapidement avec les nouvelles actions rapides, accessibles depuis la page d&#39;accueil et à partir du panneau dédié
* Les actions rapides &amp;lbrack ; Onboarding&amp;rbrack ; &amp;lbrack ; Content&amp;rbrack ; sont des workflows prédéfinis qui remplissent la pile de calques avec la plupart des calques utilisés
* &amp;lbrack ; Onboarding&amp;rbrack ; Possibilité de créer un projet via un nouveau menu Démarrage rapide, via des actions rapides ou un projet personnalisé
* &amp;lbrack ; Onboarding&amp;rbrack ; Possibilité de créer un projet vide directement depuis la page d&#39;accueil via un bouton dédié
* &amp;lbrack ; vue 3D&amp;rbrack ; Nouveau pixelliseur et traceur avancé offrant de nouvelles capacités de rendu (propriétés telles que le revêtement, l&#39;éclat, le translucency, la subsurface scattering) et une cohérence visuelle dans l&#39;écosystème de Substance
* Les paramètres de la visionneuse &amp;lbrack ;vue 3D&amp;rbrack ; sont désormais accessibles directement dans la vue 3D
* &amp;lbrack ; vue 3D&amp;rbrack ; Possibilité d&#39;enregistrer un instantané de rendu dans le presse-papiers ou dans des fichiers
* &amp;lbrack ; vue 3D&amp;rbrack ; Affiche une grille pour visualiser l&#39;origine de la scène
* &amp;lbrack ; vue 3D&amp;rbrack ; Activer le plan du sol pour capturer les ombres et les reflets
* &amp;lbrack ; vue 3D&amp;rbrack ; Contrôle le degré de réflexion et d&#39;opacité de votre plan de sol
* &amp;lbrack ; capture 3D&amp;rbrack ; Positionner le maillage sur le sol
* &amp;lbrack ;Application&amp;rbrack ; Vérifier la compatibilité matérielle au démarrage de l&#39;application
* La fenêtre de rapport de Crash &amp;lbrack ;Application&amp;rbrack ; s&#39;ouvre désormais juste après un crash
* &amp;lbrack ;Content&amp;rbrack ; Ouvrir un projet d&#39;exemple pour commencer facilement
* &amp;lbrack ; Export&amp;rbrack ; Export Adobe Standard Material shader in USD files
* &amp;lbrack ; Generative AI&amp;rbrack ; Cochez la case « Ne pas déduire » lors de l&#39;utilisation d&#39;une image comme entrée dans les workflows Image à Texture
* &amp;lbrack ; Project&amp;rbrack ; Les vignettes sont stockées dans le fichier de projet pour une ouverture plus rapide des projets
* &amp;lbrack ;Project&amp;rbrack ; Paramètre dans les préférences pour stocker les données de cache dans le fichier de projet, avec différents modes (pas de cache, cache léger, cache complet)
* &amp;lbrack ; Scripting&amp;rbrack ; &amp;lbrack ; Breaking change&amp;rbrack ; Qt migration vers Qt6.15 - impact sur la compatibilité des plug-ins existants
* &amp;lbrack ; Scripting&amp;rbrack ; Les plug-ins par défaut et le dossier des scripts se trouvent désormais dans le dossier Documents
* &amp;lbrack ; Scripting&amp;rbrack ; Nouvelle interface utilisateur pour les plug-ins pour une cohérence visuelle avec les panneaux principaux de Sampler
* &amp;lbrack ;Scripting&amp;rbrack ; Accédez à 2 exemples de plug-in pour découvrir les fonctionnalités du plug-in Sampler
* &amp;lbrack ; Scripting&amp;rbrack ; Nouvelle fonction open_3d_catpure()
* &amp;lbrack ; Scripting&amp;rbrack ; Lors de l&#39;insertion d&#39;un calque, contrôlez s&#39;il est inséré au-dessus ou au-dessous de la position cible

**Fixe :**

* &amp;lbrack ;capture 3D&amp;rbrack ; Crash si la capture d&#39;objet ne peut pas être démarrée sur macOS
* &amp;lbrack ; Application&amp;rbrack ; Crash à la sortie
* &amp;lbrack ; Application&amp;rbrack ; Se bloque à la fermeture lors de l’ajout d’actifs au panneau Projet
* &amp;lbrack ; Application&amp;rbrack ; Renommer un actif de projet ne fonctionne pas, sauf si vous appuyez sur Entrée
* Les entrées de menu &amp;lbrack ;Application&amp;rbrack ; Annuler et rétablir ne sont pas désactivées lorsqu&#39;elles devraient l&#39;être
* &amp;lbrack ; Assets&amp;rbrack ; impossible de supprimer des actifs de la section Toutes les bibliothèques du panneau Actifs
* &amp;lbrack ;Content&amp;rbrack ; Atlas creator - Utiliser la map opacity existante si elle est présente
* &amp;lbrack ;Content&amp;rbrack ; Color ID Fusion : correction du choix de couleurs dans la couleur de base
* &amp;lbrack ; Layers&amp;rbrack ; Éviter les calculs inutiles lors de l&#39;utilisation de générateurs
* &amp;lbrack ; Layers&amp;rbrack ; Ajuster un générateur peut entraîner le déclenchement d&#39;un trop grand nombre d&#39;ordinateurs
* &amp;lbrack ; Performance&amp;rbrack ; Améliorer la gestion de la mémoire GPU
* Le cache de rendu &amp;lbrack ; Performance&amp;rbrack ; ne peut pas être utilisé lors du redémarrage de l&#39;application
* Les fichiers en lecture seule &amp;lbrack ; Resources&amp;rbrack ; ne sont pas visibles dans le panneau Actifs
* &amp;lbrack ; Scripting&amp;rbrack ; Autoriser la réutilisation d&#39;un calque après l&#39;ajout d&#39;un autre calque
* &amp;lbrack ; Scripting&amp;rbrack ; La modification de la structure de la pile de calques plusieurs fois dans un script peut échouer

**Supprimé(e) :**

* &amp;lbrack ; Application&amp;rbrack ; Supprime la prise en charge des fichiers image .dng et .nef

## Version 4

### **4.5.2 GRUYERE**

*(Publié Le 7 Novembre 2024)*

**Fixe :**

* &amp;lbrack ; Content&amp;rbrack ; Filtres de fusion Recadrage, Broderie et Height

### **4.5.1 GRUYERE**

*(Publié Le 30 Juillet 2024)*

**Fixe :**

* &amp;lbrack ; Layers&amp;rbrack ; Painting greyscale masks ne fonctionne pas, ce qui affecte les outils tels que Tampon de Clone, Déformation de Peinture, Remplissage d&#39;après le contenu

### **4.5.0 GRUYERE**

*(Publié Le 18 Juillet 2024)*

**Ajouté**

* &amp;lbrack ;Interoperability&amp;rbrack ; Envoyer des matériaux à UE5, Blender, Maya, 3DsMax Unity
* &amp;lbrack ;Content&amp;rbrack ; Nouvelle catégorie de générateur de texture - Dégradés
* &amp;lbrack ;Content&amp;rbrack ; Outils HDRI - nouveau filtre de rotation de l&#39;environnement

**Fixe :**

* &amp;lbrack ; Paramètres exposés&amp;rbrack ; Exposer des valeurs d&#39;entrée .sbsar ne fonctionne pas
* La Base color &amp;lbrack ; Layers&amp;rbrack ; devient rouge avec des images en niveaux de gris
* &amp;lbrack ; Le rendu des Images en niveaux de gris utilisées dans les couches de couleur a un espace colorimétrique incorrect
* &amp;lbrack ; Le scripting&amp;rbrack ; utilisant un paramètre prédéfini d&#39;exportation n&#39;exporte pas toujours les canaux attendus
* &amp;lbrack ;Content&amp;rbrack ; Dirt : appliquer un filtre de Dirt au-dessus de l&#39;image au Matériau génère une normale noire
* &amp;lbrack ;Content&amp;rbrack ; Embossage : la mise à l’échelle d’un motif dans le filtre embossage n’est pas linéaire entre 0 et 1
* &amp;lbrack ; Content&amp;rbrack ; Make it tile - Cohérence normale et height améliorée

### **4.4.1 FONDUE**

*(Publié Le 6 Juin 2024)*

**Fixe :**

* Le filtre de Dirt &amp;lbrack ; Content&amp;rbrack ; est manquant
* Une erreur de réseau &amp;lbrack ;Generative AI&amp;rbrack ; se produit parfois lors de l&#39;utilisation d&#39;Image pour la Texture

### **4.4.0 FONDUE**

*(Publié Le 23 Mai 2024)*

**Ajouté :**

* &amp;lbrack ;Application&amp;rbrack ; le cache capture 3D est maintenant stocké dans un sous-dossier séparé
* &amp;lbrack ;Generative AI&amp;rbrack ; Image to Texture (Beta)
* &amp;lbrack ; Generative AI&amp;rbrack ; Text to Pattern (Beta)
* &amp;lbrack ;Generative AI&amp;rbrack ; Text to Texture (Beta)
* Les actifs de &amp;scripting&amp;rbrack ; possèdent désormais une propriété « resource »
* Les calques de &amp;Scripting&amp;rbrack ; possèdent désormais une propriété « output_utilisations »

**Fixe :**

* crash &amp;lbrack ;Application&amp;rbrack ; lors de l’ouverture d’un fichier de projet endommagé
* &lbrack;Application&amp;rbrack ; Crash lorsque le projet contient des ressources corrompues
* &lbrack;Application&amp;rbrack ; Crash lors de la déconnexion d&#39;un moniteur sous Windows
* Icône d&#39;application &amp;lbrack ; incorrecte dans la barre des tâches Windows
* &amp;lbrack ;Application&amp;rbrack ; La corruption du fichier de configuration principal peut entraîner la suppression de fichiers
* Les panneaux &amp;lbrack ; Application&amp;rbrack ; apparaissent devant les fenêtres contextuelles
* Les générateurs de Textures de &amp;lbrack ;Content&amp;rbrack ; ont des vignettes floues
* &amp;lbrack ; Export&amp;rbrack ; La couche d&#39;opacité générée à partir d&#39;une image importée est rompue lors de l&#39;exportation d&#39;un fichier .sbs/.sbsar
* &amp;lbrack ; Filters&amp;rbrack ; Upscale peut effectuer un crash en fonction de ses calques d’entrée
* &amp;lbrack ;Generative AI&amp;rbrack ; crashs possibles lors de la réception de résultats inattendus du service
* &amp;lbrack ; Scripting&amp;rbrack ; Crash lors du chargement automatique d&#39;un plug-in à partir d&#39;une variable d&#39;environnement
* &amp;lbrack ; Scripting&amp;rbrack ; crash possible lors de l&#39;affectation de l&#39;utilisation de la sortie avec l&#39;API

### **4.3.3 EMPANADA**

*(Publié Le 26 Mars 2024)*

**Ajouté :**

* &amp;lbrack ; capture 3D&amp;rbrack ; Nouveaux paramètres d&#39;UV automatique avancés pendant le post-traitement
* Filtre &amp;lbrack ; Filters&amp;rbrack ; Perforate : possibilité d’inverser et de modifier la taille du motif personnalisé

**Fixe :**

* La Base color de &amp;lbrack ;capture 3D&amp;rbrack ; peut être incorrecte sous macOS
* &amp;lbrack ;capture 3D&amp;rbrack ; Crash lors du traitement d&#39;une nouvelle version
* L&#39;étape de post-traitement de &amp;lbrack ;capture 3D&amp;rbrack ; peut être crash sur macOS
* &amp;lbrack ; capture 3D&amp;rbrack ; Le calque de Transforme par Maillage peut entraîner un rendu incorrect
* crash de &amp;lbrack ;Application&amp;rbrack ; au démarrage de Sampler alors qu&#39;une instance précédente est toujours en cours d&#39;exportation
* &amp;lbrack ;Application&amp;rbrack ; Sampler ne répond pas pendant un moment lors de son premier démarrage
* Le mappage d&#39;Anisotropy angle &amp;lbrack ; Export&amp;rbrack ; n&#39;est pas exporté
* &amp;lbrack ; Filters&amp;rbrack ; L&#39;ajout d&#39;une armure de tissu à la pile de calques peut entraîner un crash
* &amp;lbrack ; Filters&amp;rbrack ; L&#39;ajout d&#39;Embossage à la pile de calques peut entraîner un crash
* &amp;lbrack ; Filters&amp;rbrack ; crashs de remplissage d&#39;après le contenu lors de l&#39;utilisation d&#39;images 32 bits
* &amp;lbrack ; Filters&amp;rbrack ; Embossage : l’opacité des calques sous-jacents n’est pas complètement remplacée
* &amp;lbrack ;Filters&amp;rbrack ; Fill : le mode Fusion ne fonctionne pas dans Designer et Painter
* &amp;lbrack ; Filters&amp;rbrack ; Broderie : le choix de couleur automatique est rompu
* &amp;lbrack ;Preferences&amp;rbrack ; Empêcher de définir un chemin non pris en charge pour le cache capture 3D
* &amp;lbrack ; Preferences&amp;rbrack ; La préférence Format normal ne fonctionne pas
* &amp;lbrack ; Scripting&amp;rbrack ; Les paramètres des canaux de Asset.export_matériau respectent la casse

### **4.3.2 EMPANADA**

*(Publié Le 22 Février 2024)*

**Fixe :**

* &lbrack;L&#39;enregistrement d&#39;un projet sur un partage réseau sous Windows corrompt le fichier de projet

### **4.3.1 EMPANADA**

*(Publié Le 15 Février 2024)*

**Fixe :**

* &amp;lbrack ; capture 3D&amp;rbrack ; Crash lorsque les fichiers image deviennent inaccessibles lors de la génération de masques par lots
* &amp;lbrack ; Export&amp;rbrack ; L&#39;exportation d&#39;un matériau avec un recadrage ou par rapport au calque de stratégie d&#39;entrée donne des résultats non valides
* &amp;lbrack ; Layers&amp;rbrack ; Rare crash lors du rendu d&#39;une pile de calques
* &amp;lbrack ; Filters&amp;rbrack ; Broderie - Correction d’un problème lors de l’utilisation de l’entrée de matériau sur MacOS
* &amp;lbrack ; Filters&amp;rbrack ; Stylisation - Prise en charge des générateurs de Textures
* &amp;lbrack ; Filters&amp;rbrack ; Pattern - Correction du nom des paramètres
* &amp;lbrack ; Localization&amp;rbrack ; « Enregistrer sous... » dans la fenêtre informations sur le matériel, sous le menu aide, apparaît non localisé

### **4.3.0 EMPANADA**

*(Publié Le 25 Janvier 2024)*

**Ajouté**

* &amp;lbrack ; Assets&amp;rbrack ; Nouveau type d&#39;actif : Générateurs de Textures
* &amp;lbrack ; Assets&amp;rbrack ; Nouveaux matériaux inclus dans les ressources de démarrage
* &amp;lbrack ; Assets&amp;rbrack ; Nouveau sélecteur d&#39;actifs pour les paramètres d&#39;image dans le panneau Propriétés
* &amp;lbrack ; Assets&amp;rbrack ; Faites glisser et déposez les générateurs de Textures du panneau Actifs vers les sélecteurs d&#39;images du panneau Propriétés
* &amp;lbrack ; Assets&amp;rbrack ; Glissez et déposez les générateurs de Textures à partir de l&#39;explorateur de fichiers du système d&#39;exploitation
* Les filtres &amp;lbrack ; Assets&amp;rbrack ; peuvent suggérer d&#39;adapter les générateurs via une balise utilisateur sur l&#39;entrée d&#39;image
* Les générateurs de Textures &amp;lbrack ; Assets&amp;rbrack ; peuvent définir quel filtre doit les suggérer via une balise utilisateur
* &amp;lbrack ;Content&amp;rbrack ; Nouveau filtre de recadrage de Perspective
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre de stylisation
* &amp;lbrack ; Content&amp;rbrack ; Mode de fusion sur le filtre de remplissage
* &amp;lbrack ; Content&amp;rbrack ; Filtre de broderie mis à jour
* &amp;lbrack ;Content&amp;rbrack ; Filtre de renvoi à la ligne des Peintures mis à jour
* &amp;lbrack ;Content&amp;rbrack ; Mise à jour de tous les filtres pour prendre en charge les générateurs de Textures
* &amp;lbrack ; Layers&amp;rbrack ; Possibilité de choisir un canal de sortie du générateur de Textures lors de son ajout à la pile de calques
* &amp;lbrack ; Layers&amp;rbrack ; Possibilité de répertorier et d&#39;appliquer facilement des paramètres prédéfinis sur les générateurs de Textures
* &amp;lbrack ; Layers&amp;rbrack ; Affiche un aperçu du générateur de Textures dans les sélecteurs d&#39;images
* Les paramètres du générateur de Textures &amp;lbrack ; Layers&amp;rbrack ; peuvent être exposés et exportés
* &amp;lbrack ; Layers&amp;rbrack ; Affecter l&#39;utilisation de la Base color lors de l&#39;importation d&#39;une seule image avec le modèle de création Importation de Texture
* &amp;lbrack ; Calques&amp;rbrack ; Commentaires lors de la tentative de glisser-déposer de fichiers incompatibles dans les sélecteurs d&#39;images du panneau Propriétés
* &amp;lbrack ; Layers&amp;rbrack ; Générer une couche d&#39;opacité à partir du canal Alpha d&#39;une image importée
* &amp;lbrack ; Layers&amp;rbrack ; Image to Matériau (AI) est plus rapide à calculer lors du changement de catégorie
* &amp;lbrack ; Layers&amp;rbrack ; Sélectionnez le calque le plus pertinent après l&#39;utilisation d&#39;un modèle de création
* &amp;lbrack ; Layers&amp;rbrack ; Les widgets de position peuvent désormais être modifiés à l&#39;aide d&#39;un curseur dans le groupe Paramètres avancés
* &amp;lbrack ; Export&amp;rbrack ; Afficher un pourcentage dans la file d&#39;attente au lieu de nombres bruts
* Le canal d&#39;opacité &amp;lbrack ;Interoperability&amp;rbrack ; est désormais reconnu comme canal Alpha lors de l&#39;envoi vers Painter
* &amp;lbrack ; Application&amp;rbrack ; Nouvelle boîte de dialogue pour afficher et enregistrer les informations sur le matériel
* &amp;lbrack ;Application&amp;rbrack ; Nouvelle préférence pour modifier l&#39;échelle d&#39;height par défaut pour chaque projet
* &amp;lbrack ;Application&amp;rbrack ; Améliorer l&#39;affichage des ressources obsolètes
* &amp;lbrack ; Scripting&amp;rbrack ; New asset.documentResolution() et asset.setDocumentResolution()
* &amp;lbrack ; Scripting&amp;rbrack ; Nouvelle fonction select_asset()
* &amp;lbrack ; Scripting&amp;rbrack ; Python API for Texture Generators
* &amp;lbrack ; Scripting&amp;rbrack ; get_project_assets() renvoie désormais des objets 3D
* La taille de la &amp;vignette de l&#39;actif i&amp;rbrack ; peut être modifiée dans le panneau Actifs
* &amp;lbrack ;UI&amp;rbrack ; Icônes d&#39;affichage du viewport mises à jour

**Fixe :**

* &amp;lbrack ;vue 2D&amp;rbrack ; Le zoom avec la molette de la souris est bloqué à 244 %
* &amp;lbrack ;Application&amp;rbrack ; Crash au démarrage lors de l&#39;initialisation de l&#39;API graphique
* &amp;lbrack ;Application&amp;rbrack ; Crash si le nom du projet contient le caractère #
* &amp;lbrack ; Application&amp;rbrack ; crash possible lors de l&#39;ouverture d&#39;un ancien projet
* &amp;lbrack ;Application&amp;rbrack ; La réouverture du projet peut entraîner un crash
* &amp;lbrack ; Application&amp;rbrack ; Certaines modifications apportées au projet ne sont pas enregistrées et sont perdues sans avertissement lors de la fermeture du projet si elles ne sont pas enregistrées
* &amp;lbrack ; Export&amp;rbrack ; .sbs/.sbsar problèmes d&#39;exportation lors de l&#39;utilisation de plusieurs fichiers portant le même nom
* &amp;lbrack ; Export&amp;rbrack ; Espace colorimétrique incorrect pour les images en niveaux de gris exportées .sbs/.fichier sbsar
* &amp;lbrack ; Filters&amp;rbrack ; Problèmes de comportement de fusion de l&#39;opacité
* Les fichiers .svg &amp;lbrack ; Layers&amp;rbrack ; ne sont pas toujours rendus à la bonne résolution
* &amp;lbrack ; Performance&amp;rbrack ; Certaines sauvegardes de projet sur le disque ne sont pas nécessaires
* &amp;lbrack ;Project&amp;rbrack ; L&#39;importation d&#39;un ancien projet ne charge pas les paramètres prédéfinis associés
* &amp;lbrack ; Scripting&amp;rbrack ; Impossible d&#39;obtenir les paramètres du premier calque inséré
* &amp;lbrack ; UI&amp;rbrack ; La fenêtre contextuelle d’aperçu lors du survol d’une ressource peut apparaître au mauvais emplacement ou sur le mauvais écran
* Les panneaux &amp;lbrack ; UI&amp;rbrack ; non ancrés sont visibles et utilisables en haut de l&#39;écran d&#39;accueil

### **4.2.2 DORAYAKI**

*(Publié Le 5 Décembre 2023)*

**Ajouté :**

* &amp;lbrack ;capture 3D&amp;rbrack ; capture 3D est désormais 5 à 10 % plus rapide sous Windows
* &amp;lbrack ;capture 3D&amp;rbrack ; Améliorer le nettoyage du maillage avant la décimation
* &amp;lbrack ;Moteur&amp;rbrack ; Mettre à jour la Substance Engine à la version 9.0.3
* &amp;lbrack ; Layers&amp;rbrack ; Content-Aware Fill : mise à jour en amont, divers correctifs de cas d&#39;utilisation et prise en charge de Linux

**Fixe :**

* &amp;lbrack ;capture 3D&amp;rbrack ; Cliquer sur « Précédent » après l&#39;alignement puis sur « Suivant » ne met pas à jour le nuage de points
* maillage &amp;lbrack ; capture 3D&amp;rbrack ; affiché avec des trous après avoir été ajouté au projet
* &lbrack;Application&amp;rbrack ; Crash lors de la sortie du mode plein écran après une Capture 3D
* &amp;lbrack ; Application&amp;rbrack ; Crash avec fichiers image conçus
* &amp;lbrack ;Application&amp;rbrack ; Si vous êtes dans « Toutes les bibliothèques » lorsque vous quittez Sampler, le panneau Actifs devient vide au redémarrage
* &amp;lbrack ; Application&amp;rbrack ; Fuite de mémoire lors de l&#39;exportation du matériau
* &amp;lbrack ; Application&amp;rbrack ; L’ouverture d’un enregistrement de projet avec des versions précédentes de Sampler peut entraîner un crash
* &amp;lbrack ;Application&amp;rbrack ; crashs potentiels en cas d&#39;échec de la conversion des maillages 3D
* &amp;lbrack ;Application&amp;rbrack ; crash silencieux lors de l’ouverture d’un fichier .sbsar pendant l’exécution de Sampler
* &amp;lbrack ; Export&amp;rbrack ; Crash lors de l&#39;exportation d&#39;un fichier .sbs/.fichier sbsar avec une utilisation personnalisée
* &amp;lbrack ; Export&amp;rbrack ; Les maps normal exportées sont toujours DirectX quel que soit le paramètre utilisateur
* &amp;lbrack ; Export&amp;rbrack ; L’exportation d’un objet 3D vers un fichier FBX sous macos ne fonctionne pas
* &amp;lbrack ; Export&amp;rbrack ; Incohérences lors de l&#39;exportation d&#39;une Pile de calques avec un filtre Broderie au format .sbs/.fichier sbsar
* &amp;lbrack ; Export&amp;rbrack ; Parfois, l&#39;exportation de fichiers .sbs/.sbsar ne fonctionne pas
* &amp;lbrack ;Export&amp;rbrack ; Parfois, lors de l&#39;exportation d&#39;une image .sbs/.fichier sbsar, le nombre de bits par pixel n&#39;est pas adapté
* &amp;lbrack ; Layers&amp;rbrack ; Rendre un calque de projection invisible rend son premier enfant à la place
* &amp;lbrack ; Layers&amp;rbrack ; Crash lors du chargement du masque dans le calque Luminosité/Contraste
* Les messages d&#39;erreur &amp;lbrack ; Layers&amp;rbrack ; trompeurs s&#39;affichent après la suppression du calque
* &amp;lbrack ; Layers&amp;rbrack ; crash possible lors de la rétrogradation d&#39;une ressource
* &amp;lbrack ; Layers&amp;rbrack ; Certaines sorties ne sont pas connectées aux entrées à moins que l&#39;utilisation ne soit forcée dans le panneau Paramètres des couches
* La liste déroulante du calque de référence &amp;lbrack ; Taille physique&amp;rbrack ; peut être réinitialisée par erreur
* Les icônes &amp;lbrack ;UI&amp;rbrack ; Importer les informations sur le modèle doivent être mises à jour
* &amp;lbrack ; UI&amp;rbrack ; Conseil de raccourci de Viewport s&#39;affiche chaque fois que la disposition de viewport change

### **4.2.1 DORAYAKI**

*(Publié Le 21 Septembre 2023)*

**Ajouté :**

* &amp;lbrack ;Content&amp;rbrack ; Image vers le Matériau - Améliorer la génération de microdétails dans les maps normal
* &amp;lbrack ;Content&amp;rbrack ; Image en Matériau - Nouveau paramètre d&#39;intensité de l&#39;éclat
* Les images &amp;lbrack ; Layers&amp;rbrack ; peuvent être ajoutées dans les calques d&#39;importation d&#39;image
* Les images &amp;lbrack ; Layers&amp;rbrack ; peuvent être supprimées dans les calques d&#39;importation d&#39;image
* &amp;lbrack ; Layers&amp;rbrack ; Les calques non valides peuvent désormais être supprimés
* &amp;lbrack ; vue 2D&amp;rbrack ; Maj+C raccourci pour revenir aux canaux
* &amp;lbrack ;capture 3D&amp;rbrack ; Affiche un toast d&#39;avertissement lorsque l&#39;utilisateur importe moins de 20 images
* &amp;lbrack ;Application&amp;rbrack ; Nouvelles préférences pour définir la valeur par défaut de la répétition de texture de matériau
* &amp;lbrack ; Onboarding&amp;rbrack ; Mise à jour de l&#39;interface utilisateur du tutoriel pour Image vers Matériau (AI) et Mise à niveau
* API capture 3D &amp;lbrack ; Scripting&amp;rbrack ; : DatasetInfo contient plus de données lorsque Capture3dState est défini sur aligné
* &amp;lbrack ; Scripting&amp;rbrack ; New select_asset argument to create_asset(). Nouvelles fonctions : wait_for_calcul() et clear_render_cache()

**Fixe :**

* &amp;lbrack ; Layers&amp;rbrack ; Crash lorsque la zone de recadrage est très petite
* crash &amp;lbrack ; Layers&amp;rbrack ; lors de l&#39;ajout ou de l&#39;ajustement du filtre Recadrage
* &amp;lbrack ; Layers&amp;rbrack ; Rendre la zone de recadrage carrée entraîne une résolution de sortie de matériau incorrecte
* Les sorties &amp;lbrack ; Layers&amp;rbrack ; disparaissent parfois lorsque plusieurs calques sont désactivés
* Le cache de rendu &amp;lbrack ; Layers&amp;rbrack ; peut ne pas être correctement invalidé avec les filtres Image vers Matériau (AI) et Agrandir
* &amp;lbrack ; Layers&amp;rbrack ; Impossible d&#39;ajouter le filtre Agrandir lors de la sélection « Ne plus afficher ce message » dans la fenêtre contextuelle d&#39;avertissement
* &amp;lbrack ; Layers&amp;rbrack ; Impossible de restaurer l&#39;image dans le filtre Broderie une fois modifié
* &amp;lbrack ; Export&amp;rbrack ; La résolution de map normal exportée change lors de la modification du format normal
* &amp;lbrack ; Export&amp;rbrack ; Supprimer le suffixe de nom de fichier « \_environment » lors de l&#39;exportation d&#39;un environnement
* &amp;lbrack ; Export&amp;rbrack ; Impossible d&#39;exporter un fichier .fichier sbsar lorsqu&#39;il y a un calque de Transforme de déformation dans la pile de calques
* &amp;lbrack ; vue 2D&amp;rbrack ; « Adapter à l&#39;écran » ne fonctionne pas lorsque la résolution change
* &amp;lbrack ;Application&amp;rbrack ; Après avoir fermé la fenêtre de l&#39;application pendant le calcul, le processus de l&#39;application peut encore être en cours d&#39;exécution
* &amp;lbrack ; Application&amp;rbrack ; Crash à la sortie
* &amp;lbrack ; Application&amp;rbrack ; Invalider le cache de rendu lors du basculement de réseaux neuronaux à accélération GPU
* &amp;lbrack ; Le fait de nommer un plug-in comme nom de panneau existant provoque des comportements inattendus
* &amp;lbrack ;UI&amp;rbrack ; Cliquer sur un élément avec une info-bulle entraîne la disparition de l&#39;info-bulle jusqu&#39;au redémarrage
* La valeur d&#39;échelle d&#39;Height de &amp;lbrack ; UI&amp;rbrack ; peut changer lors du changement d&#39;actifs
* &amp;lbrack ; UI&amp;rbrack ; Marge incorrecte dans les zones de liste déroulante

### **4.2 DORAYAKI**

*(Publié Le 5 Septembre 2023)*

**Ajouté :**

* &amp;lbrack ; Content&amp;rbrack ; Amélioration considérable des filtres Image en Matériau (AI) et Delighter
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre Upscale
* &amp;lbrack ; Content&amp;rbrack ; Le filtre Recadrage a désormais une résolution de sortie dynamique.
* &amp;lbrack ; Matériau Creation Template&amp;rbrack ; Add Document size setting.
* &amp;lbrack ; Matériau Creation Template&amp;rbrack ; Nouveau bouton bascule « Ajouter un recadrage ».
* &amp;lbrack ; Matériau Creation Template&amp;rbrack ; New « Upscale Matériau » toggle
* &amp;lbrack ; Modèle de création de Matériau&amp;rbrack ; Afficher la taille de l&#39;image importée
* &amp;lbrack ; Matériau Creation Template&amp;rbrack ; Donner un commentaire lorsque certaines images importées ne peuvent pas être utilisées
* &amp;lbrack ; Matériau Creation Template&amp;rbrack ; Avertir lorsque les tailles d&#39;image sont incohérentes
* &amp;lbrack ; Modèle de création de Matériau&amp;rbrack ; Nouveaux avertissements et info-bulles
* &amp;lbrack ; Layers&amp;rbrack ; Affiche la résolution des calques dans la pile de calques
* &amp;lbrack ; Layers&amp;rbrack ; La résolution de calcul des calques peut désormais être définie sur Taille du document ou Taille d&#39;entrée
* &amp;lbrack ; Layers&amp;rbrack ; Afficher la résolution des calques dans la pile de calques
* &amp;lbrack ; Layers&amp;rbrack ; Basculer une stratégie de résolution de calque vers Document ou Entrée de calque le cas échéant
* &amp;lbrack ; Layers&amp;rbrack ; Avertit l&#39;utilisateur lorsqu&#39;un filtre Mise à l&#39;échelle est ajouté manuellement et fournit de la documentation
* &amp;lbrack ; Layers&amp;rbrack ; Avertit l&#39;utilisateur lors d&#39;une mise à l&#39;échelle linéaire et propose d&#39;utiliser le filtre Mise à l&#39;échelle à la place
* &amp;lbrack ; Layers&amp;rbrack ; Computing an Image to Matériau (AI) layer peut désormais être annulé plus rapidement, pour améliorer les temps de rendu lors de l&#39;ajustement de la pile de calques
* &amp;lbrack ; Layers&amp;rbrack ; Le calcul d&#39;un calque Upscale peut désormais être annulé plus rapidement, pour améliorer les temps de rendu lors du réglage de la pile de calques
* &amp;lbrack ; Export&amp;rbrack ; Autoriser la résolution de remplacement des textures exportées
* La &amp;liste des canaux à exporter de lbrack ; export&amp;rbrack ; est maintenant triée
* &amp;lbrack ; Export&amp;rbrack ; Afficher la résolution des canaux dans la liste des canaux à exporter
* &amp;lbrack ; Application&amp;rbrack ; Nouvelle préférence pour activer ou désactiver les réseaux neuronaux à accélération GPU
* &amp;lbrack ; UI&amp;rbrack ; Amélioration des listes déroulantes de résolution
* &amp;lbrack ; UI&amp;rbrack ; Nouvelles icônes pour les filtres de Transforme de Maillage, de post-traitement de Maillage et d&#39;armure
* &amp;lbrack ; UI&amp;rbrack ; Renommer le panneau « Partager » en « Exporter »
* &amp;lbrack ; Scripting&amp;rbrack ; Ajouter la prise en charge de la résolution de sortie des calques à l&#39;API d&#39;exportation
* &amp;lbrack ; Scripting&amp;rbrack ; Ajout de la taille Recadrer, Agrandir et Document à l&#39;API d&#39;importation d&#39;images
* &amp;lbrack ; Onboarding&amp;rbrack ; New tutorials
* &amp;lbrack ; Onboarding&amp;rbrack ; Update Welcome and What&#39;s New screens content
* &amp;lbrack ;Moteur&amp;rbrack ; Mettre à jour la Substance Engine à la version 9.0.1

**Fixe :**

* &amp;lbrack ; capture 3D&amp;rbrack ; Amélioration de la précision du nommage des options dans les paramètres de paramètres d&#39;alignement
* &amp;lbrack ; Application&amp;rbrack ; L&#39;importation d&#39;images avec un non-multiple de 16 dimensions peut entraîner un crash
* &amp;lbrack ;Application&amp;rbrack ; Crash lors de la duplication d&#39;un actif dans le panneau Projet
* &amp;lbrack ; Application&amp;rbrack ; Crash lors du changement d’actifs dans le panneau Projet
* &amp;lbrack ;Content&amp;rbrack ; La peinture d&#39;un masque personnalisé pour le filtre du Snow ne fonctionne pas correctement
* les modifications des Paramètres exposés &amp;lbrack ; Paramètres exposés&amp;rbrack ; peuvent être perdues lors du changement de matériaux
* &amp;lbrack ;Interoperability&amp;rbrack ; L&#39;envoi d&#39;un Matériau à partir du panneau Exporter peut entraîner un crash
* &amp;lbrack ; Layers&amp;rbrack ; Content-Aware Fill arrête le calcul lors du passage d&#39;une entrée d&#39;image unique à une entrée de matériau
* crash &amp;lbrack ; Layers&amp;rbrack ; après la duplication d&#39;un Éclairage d&#39;environnement contenant un matériau
* Le calque d&#39;importation d&#39;image &amp;lbrack ; Layers&amp;rbrack ; affiche un nom d&#39;image incorrect dans le panneau Propriétés si le fichier image a été renommé
* &amp;lbrack ; Layers&amp;rbrack ; Parfois, une double flèche s&#39;affiche sur un calque inactif
* &amp;lbrack ; Layers&amp;rbrack ; Parfois, modifier l&#39;utilisation de sortie d&#39;une image dans un calque d&#39;importation d&#39;image ne fonctionne pas
* &amp;lbrack ; Layers&amp;rbrack ; Typos in the Creation Template Window
* L’info-bulle d’intégration du viewport 3D &amp;lbrack ; UI&amp;rbrack ; présente des problèmes de focus
* Le nom de l&#39;image &amp;lbrack ; UI&amp;rbrack ; peut déborder si le nom du fichier est trop long
* &amp;lbrack ; UI&amp;rbrack ; Problèmes mineurs de mise en page de la barre d&#39;outils Pinceau lors de l&#39;utilisation de la gomme
* Les chaînes &amp;lbrack ; UI&amp;rbrack ; sont tronquées dans certaines langues dans le panneau Paramètres du visualiseur
* &amp;lbrack ;UI&amp;rbrack ; Lorsque la fenêtre contextuelle de l&#39;info-bulle du viewport est affichée, appuyer sur « space » crée un nouveau projet

### **4.1.2 CANNOLI**

*(Publié Le 20 Juin 2023)*

**Fixe :**

* &amp;lbrack ; Layers&amp;rbrack ; Fuite de mémoire lors du réglage des matériaux de Substance et des filtres provoquant des crashs

### **4.1.1 CANNOLI**

*(Publié Le 6 Juin 2023)*

**Ajouté**

* &amp;lbrack ;Moteur&amp;rbrack ; Mettre à jour la Substance Engine à la version 9.0
* &amp;lbrack ;Interoperability&amp;rbrack ; Envoyer des objets 3D à Stager et Painter

**Fixe :**

* &amp;lbrack ; capture 3D&amp;rbrack ; Applications crashs en cas d&#39;échec du rendu capture 3D
* &amp;lbrack ;capture 3D&amp;rbrack ; Crash lorsqu&#39;une image ne peut pas être chargée
* &amp;lbrack ; capture 3D&amp;rbrack ; Crash lorsque vous atteignez l&#39;étape de reconstruction du Maillage
* &amp;lbrack ; capture 3D&amp;rbrack ; Crash lors du redimensionnement du cadre de sélection
* &amp;lbrack ; capture 3D&amp;rbrack ; L&#39;importation de masques conformes à la convention n&#39;affecte pas le masque correctement
* &amp;lbrack ; capture 3D&amp;rbrack ; Le rendu présente des problèmes lors du réglage du cadre de sélection
* &amp;lbrack ; capture 3D&amp;rbrack ; La commutation entre les options de rendu de version et de basculement pendant le post-processus Capture 3D est lente
* &amp;lbrack ;capture 3D&amp;rbrack ; La commutation entre les versions pendant l&#39;étape de post-traitement de capture 3D est parfois interrompue
* crash &amp;lbrack ; Application&amp;rbrack ; au démarrage
* crash &amp;lbrack ; Application&amp;rbrack ; lors de la duplication d&#39;un matériau renommé
* crash &amp;lbrack ;Application&amp;rbrack ; lors de l&#39;ouverture d&#39;un projet .alch hérité sans son dossier de dépendances
* &amp;lbrack ;Application&amp;rbrack ; Crash lors de la connexion/déconnexion d&#39;un écran, l&#39;ordinateur se met en veille ou est accessible à distance
* crashs d&#39;&amp;application&amp;rbrack ; et fuites de mémoire liées à la gestion non persistante des actifs
* &amp;lbrack ;Export&amp;rbrack ; Le choix du format de matériau pour les types de fichiers d&#39;objets 3D qui incorporent ou référencent des textures doit être désactivé
* &amp;lbrack ; Export&amp;rbrack ; Crash si un problème se produit lors de l’exportation d’objets 3D
* &amp;lbrack ; Export&amp;rbrack ; Crash lors de l&#39;exportation d&#39;un fichier .sbs/.fichier sbsar
* &amp;lbrack ; Export&amp;rbrack ; Crash lors de l&#39;importation d&#39;un paramètre prédéfini personnalisé ayant le même libellé mais pas le même nom de fichier
* &amp;lbrack ; Export&amp;rbrack ; L&#39;exportation d&#39;un éclairage d&#39;environnement vers un fichier .sbs/.fichier sbsar ne fonctionne pas toujours
* &amp;lbrack ; Export&amp;rbrack ; Gltf/Glb export encode les textures en base64
* Le champ de texte &amp;lbrack ; Export&amp;rbrack ; Name ne fonctionne pas lors de la refocalisation
* La répétition &amp;lbrack ; Export&amp;rbrack ; Preserve ne fonctionne pas lors de l&#39;exportation d&#39;une image vers un calque Matériau (alimenté par l&#39;IA) vers un fichier .sbs/.fichier sbsar
* &amp;lbrack ; Export&amp;rbrack ; Lors de l&#39;exportation gltf et du remplacement de fichiers, la liste des fichiers à remplacer n&#39;est pas correcte
* &amp;lbrack ; Paramètres exposés&amp;rbrack ; La valeur de départ aléatoire ne fonctionne pas dans les fichiers .sbs/.sbsar exportés
* &amp;lbrack ; Layers&amp;rbrack ; Content-Aware Fill crash parfois lorsqu&#39;il est ajouté pour la deuxième fois
* &amp;lbrack ; Layers&amp;rbrack ; Crash lors du calcul d&#39;une pile de calques
* Le cache disque &amp;lbrack ; Layers&amp;rbrack ; Image to Matériau (AI) ne fonctionne pas
* &amp;lbrack ; Layers&amp;rbrack ; crash possible lors de l&#39;ajustement d&#39;un calque
* &amp;lbrack ; Performance&amp;rbrack ; Fuites de mémoire
* &amp;lbrack ;Project&amp;rbrack ; Crash lors de l&#39;enregistrement d&#39;un projet
* &amp;lbrack ;Project&amp;rbrack ; L&#39;importation du même projet deux fois de suite duplique les ressources
* Les boutons &amp;lbrack ; UI&amp;rbrack ; Arrondis avec une seule icône ne sont pas affichés correctement

### 4.1.0 Cannoli

*(Publié Le 28 Mars 2023)*

**Ajouté :**

* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre de broderie
* &amp;lbrack ;Content&amp;rbrack ; Nouveau filtre Déformation de Peinture
* &amp;lbrack ; UI&amp;rbrack ; option Ajouter une exportation dans le menu Fichier
* Le bouton &amp;lbrack ; capture 3D&amp;rbrack ; Back est maintenant disponible sur l&#39;étape d&#39;alignement
* &amp;lbrack ; capture 3D&amp;rbrack ; Images Gérer l&#39;orientation EXIF du JPEG
* &amp;lbrack ; capture 3D&amp;rbrack ; Scripting - Nouvelle propriété dataset_info.caméra
* &amp;lbrack ; capture 3D&amp;rbrack ; Ajout de la prise en charge de Linux (voir la documentation)
* &amp;lbrack ;capture 3D&amp;rbrack ; Vérifier l&#39;accès en lecture des images importées
* &amp;lbrack ;Onboarding&amp;rbrack ; Learn - 2 nouveaux tutoriels (Broderie et déformation de Peinture)
* &amp;lbrack ; Onboarding&amp;rbrack ; Contenu mis à jour

**Fixe :**

* &amp;lbrack ;capture 3D&amp;rbrack ; Conserver la position de la caméra lors du changement de version
* &amp;lbrack ; capture 3D&amp;rbrack ; Fusionner tous les groupes d&#39;un objet en un seul
* &amp;lbrack ; capture 3D&amp;rbrack ; a renommé les maillages générés en Original
* &lbrack;Application&amp;rbrack ; Crash lors de la tentative de génération de la vignette d&#39;une image inexistante
* L&#39;icône de la corbeille &amp;lbrack ; Assets&amp;rbrack ; ne fait rien dans le panneau Actifs
* &amp;lbrack ; Content&amp;rbrack ; La mise à jour des filtres avec des emplacements de matériau ne fonctionne pas comme prévu
* &amp;lbrack ; Export&amp;rbrack ; crash possible lors de l’exportation d’une ressource avec des filtres spécifiques
* &amp;lbrack ; Export&amp;rbrack ; SBS/SBSAR Export - les calques d&#39;importation d&#39;image avaient la priorité sur les paramètres d&#39;image
* Le paramètre prédéfini d&#39;exportation &amp;lbrack ; Export&amp;rbrack ; UE4 ne fonctionne pas avec PNG
* &amp;lbrack ; Layers&amp;rbrack ; Crash lors de la suppression simultanée d&#39;un matériau et d&#39;un filtre depuis l&#39;explorateur du système d&#39;exploitation
* crash de &amp;lbrack ; Layers&amp;rbrack ; lors du glissement d’un Fichier sbsar avec un fichier image
* La couche d&#39;opacité de &amp;laers&amp;rbrack ; broidery peut être entièrement blanche
* La langue chinoise de &amp;lbrack ;Localization&amp;rbrack ; peut être affichée par défaut sous Linux
* &amp;lbrack ; Performance&amp;rbrack ; Correction d’un problème de mémoire lors de la suppression d’un calque d’une ressource
* &amp;lbrack ; Projet&amp;rbrack ; crash possible lors de l&#39;enregistrement
* &amp;lbrack ;UI&amp;rbrack ; Ajouter un espacement manquant sur le bouton de menu de la version
* &amp;lbrack ; UI&amp;rbrack ; Le bouton Annuler ne s&#39;affiche pas correctement
* &amp;lbrack ; UI&amp;rbrack ; Désactiver l&#39;animation des curseurs pour les paramètres de post-traitement capture 3D
* &amp;lbrack ; UI&amp;rbrack ; La fenêtre Modèle de création de Matériau ne se ferme pas lorsque vous cliquez en dehors
* &amp;lbrack ; UI&amp;rbrack ; L&#39;accesseur rapide du filtre se ferme lorsqu&#39;il clique en dehors

**Problèmes Connus :**

* &amp;lbrack ; Le sélecteur de couleurs&amp;rbrack ; Choisir une couleur sur un deuxième moniteur avec une résolution différente peut ne pas fonctionner
* Le widget d&#39;éclairage de forme &amp;lbrack ; Content&amp;rbrack ; ne fonctionne pas en mode projection sphérique
* Le Matériau &amp;lbrack ; d&#39;interopérabilité&amp;rbrack ; avec le displacement envoyé à Stager perdra les contrôles de displacement

### 4.0.2 Bananes

*(Publié Le 9 Mars 2023)*

**Ajouté :**

* &amp;lbrack ;capture 3D&amp;rbrack ; L&#39;utilisation du disque affiche la quantité utilisée
* &amp;lbrack ;capture 3D&amp;rbrack ; L&#39;importation de photos est asynchrone et plus rapide
* &amp;lbrack ; Scripting&amp;rbrack ; Nouvelles classes et fonctions de script de la fonction capture 3D
* &amp;lbrack ; Scripting&amp;rbrack ; Nouvelle classe ExportController pour effectuer des actions lorsque l&#39;exportation est terminée, échouée ou annulée
* &amp;lbrack ; Scripting&amp;rbrack ; Passer des arguments les scripts python s&#39;exécutent avec —run-script
* &amp;lbrack ; UI&amp;rbrack ; retour d’informations de l’interface utilisateur lorsque vous faites glisser un actif sur le panneau Calques
* Le filtre de température de couleur &amp;lbrack ; Content&amp;rbrack ; fonctionne désormais sur les matériaux
* &amp;lbrack ;Content&amp;rbrack ; Normal aux filtres Heights dispose d&#39;une nouvelle option pour préserver la répétition

**Fixe :**

* &amp;lbrack ; capture 3D&amp;rbrack ; Taille d&#39;image corrigée dans l&#39;étape d&#39;alignement du jeu de données
* &amp;lbrack ;capture 3D&amp;rbrack ; Supprimer les vertex en double après l&#39;UV
* &amp;lbrack ; capture 3D&amp;rbrack ; MacOS - Meilleure détection si capture 3D est disponible
* &amp;lbrack ; capture 3D&amp;rbrack ; Crash lors de la fermeture de la fenêtre Capture 3D lors de l&#39;importation d&#39;images
* &amp;lbrack ;capture 3D&amp;rbrack ; Crash lors de la génération d&#39;une nouvelle version
* &amp;lbrack ;capture 3D&amp;rbrack ; Crash lors de la tentative de chargement de l&#39;objet 3D dans la visionneuse
* &amp;lbrack ; capture 3D&amp;rbrack ; Crash lors de l&#39;utilisation d&#39;un chemin avec des caractères non UTF8
* &amp;lbrack ; capture 3D&amp;rbrack ; Tentatives de frappe
* les Maillages &amp;lbrack ; capture 3D&amp;rbrack ; ne sont plus mis à l&#39;échelle pour s&#39;adapter au cube unitaire
* &amp;lbrack ; capture 3D&amp;rbrack ; Empêcher un crash lors de la fermeture de Capture 3D lors du rendu
* &amp;lbrack ; capture 3D&amp;rbrack ; La suppression d&#39;un masque fait disparaître l&#39;image
* crash de &amp;lbrack ;Application&amp;rbrack ; lors de l’importation simultanée de deux ressources
* &amp;lbrack ; Application&amp;rbrack ; Sauvegarde la version précédente des ressources lors de l’ouverture d’un projet si elles n’ont jamais été sauvegardées
* &amp;lbrack ;Application&amp;rbrack ; Mettre correctement en cache les maps bakées lorsque tous les mappages ne sont pas bakés
* &amp;lbrack ;Application&amp;rbrack ; crash plein écran lorsqu&#39;un objet 3D est affiché.
* &amp;lbrack ;Application&amp;rbrack ; Le dernier matériau est dupliqué lors de l&#39;enregistrement du projet
* &amp;lbrack ; Application&amp;rbrack ; Empêcher le crash lors de l&#39;annulation du calcul de post-traitement du Maillage pendant l&#39;étape de baking
* &amp;lbrack ;Application&amp;rbrack ; La réouverture du projet actuel n&#39;annule pas les modifications
* &amp;lbrack ;Application&amp;rbrack ; Arrêter de générer des vignettes pour les objets 3D
* &amp;lbrack ; vue 2D&amp;rbrack ; Crash lors de l&#39;utilisation de l&#39;outil pinceau
* &amp;lbrack ; Content&amp;rbrack ; Content Aware Fill - Le calcul peut être bloqué
* Le filtre Créateur d&#39;&amp;atlas de contenu&amp;rbrack ; réduit la taille de la couche d&#39;opacité
* &amp;lbrack ; Export&amp;rbrack ; Fix clear Failed exports queue
* L&#39;exportation OBJ &amp;lbrack ; Export&amp;rbrack ; crée un objet 100 fois plus petit que prévu
* Les images couleur &amp;lbrack ; Layers&amp;rbrack ; importées sous forme de couches de niveaux de gris sont désormais considérées comme des niveaux de gris
* Les fichiers &amp;lbrack ; Export&amp;rbrack ; FBX ne peuvent pas être importés dans des applications tierces
* Les noms de sortie de &amp;lbrack ;Export&amp;rbrack ; Shader dans les fichiers USD ne sont pas corrects
* Le nom de l&#39;image &amp;lbrack ; Layers&amp;rbrack ; n&#39;est pas mis à jour lorsque son nom est modifié sur l&#39;explorateur du système d&#39;exploitation
* &amp;lbrack ; Script&amp;rbrack ; Affiche un message d&#39;erreur lors du rechargement d&#39;un script non valide
* &amp;lbrack ;UI&amp;rbrack ; bouton de Matériau de base désactivé lorsque non disponible
* &amp;lbrack ; UI&amp;rbrack ; Crash lors de l&#39;accès à la boîte de dialogue Fichier dans la fenêtre Modèle de création de Matériau
* L&#39;accesseur rapide &amp;lbrack ; UI&amp;rbrack ; est accessible même lorsque le panneau Calques est fermé
* Les icônes Envoyer à &amp;lbrack ;UI&amp;rbrack ; sont mal alignées
* &amp;lbrack ; UI&amp;rbrack ; L&#39;icône de calque change lorsque vous cliquez sur l&#39;icône de Fusion

**Problèmes Connus :**

* &amp;lbrack ; Le sélecteur de couleurs&amp;rbrack ; Choisir une couleur sur un deuxième moniteur avec une résolution différente peut ne pas fonctionner
* Le widget d&#39;éclairage de forme &amp;lbrack ; Content&amp;rbrack ; ne fonctionne pas en mode projection sphérique
* Le Matériau &amp;lbrack ; d&#39;interopérabilité&amp;rbrack ; avec le displacement envoyé à Stager perdra les contrôles de displacement

### 4.0.1 Bananes

*(Publié Le 7 Février 2023)*

**Fixe :**

* &amp;lbrack ;capture 3D&amp;rbrack ; Lors de l&#39;utilisation de masques, la projection de texture peut être rompue
* Les artefacts de &amp;lbrack ;capture 3D&amp;rbrack ; peuvent apparaître sur votre objet
* &amp;lbrack ; capture 3D&amp;rbrack ; Le maillage exporté est peut-être vraiment petit

**Problèmes Connus :**

* les exportations FBX et OBJ de &amp;lbrack ;capture 3D&amp;rbrack ; réduisent l&#39;échelle du résultat
* &amp;lbrack ; capture 3D&amp;rbrack ; capture 3D est disponible sur MacOS même si votre matériel n&#39;est pas compatible. Consultez la documentation.
* &amp;lbrack ;capture 3D&amp;rbrack ; Crash lorsque la reconstruction du maillage est terminée.
* &amp;lbrack ; Layers&amp;rbrack ; Content-Aware Fill peut être bloqué si vous modifiez les calques en dessous
* &amp;lbrack ; Le sélecteur de couleurs&amp;rbrack ; Choisir une couleur sur un deuxième moniteur avec une résolution différente peut ne pas fonctionner
* Le widget d&#39;éclairage de forme &amp;lbrack ; Content&amp;rbrack ; ne fonctionne pas en mode projection sphérique
* Le Matériau &amp;lbrack ; d&#39;interopérabilité&amp;rbrack ; avec le displacement envoyé à Stager perdra les contrôles de displacement

### 4.0.0 Bananes

*(Publié Le 31 Janvier 2023)*

**Ajouté :**

* &amp;lbrack ;capture 3D&amp;rbrack ; Créer des objets 3D à partir d&#39;images
* &amp;lbrack ; capture 3D&amp;rbrack ; Assistant capture 3D dédié
* &amp;lbrack ;capture 3D&amp;rbrack ; Importer ou générer du noir et des masques blancs sur votre jeu de données
* &amp;lbrack ; capture 3D&amp;rbrack ; Résultat de l&#39;alignement : afficher toutes les fonctions correspondantes sous forme de nuage de points
* &amp;lbrack ; capture 3D&amp;rbrack ; Résultat de l&#39;alignement : affichez les caméras associées à chaque photo alignée et interagissez avec elles
* &amp;lbrack ; capture 3D&amp;rbrack ; Définir la zone de reconstruction avec un widget de cadre de sélection
* &amp;lbrack ; capture 3D&amp;rbrack ; Redimensionnez, translatez et faites pivoter tous les axes du widget du cadre de sélection
* &amp;lbrack ; capture 3D&amp;rbrack ; Définir la précision géométrique du maillage reconstruit
* &amp;lbrack ;capture 3D&amp;rbrack ; Optimisez votre maillage et vos textures en créant une nouvelle version
* &amp;lbrack ; capture 3D&amp;rbrack ; Chacune des versions est automatiquement décimée selon le numéro de face cible défini
* &amp;lbrack ;capture 3D&amp;rbrack ; L&#39;étape de post-traitement déplie automatiquement, re-projette les textures, puis bake l&#39;height normal et les informations d&#39;AO du maillage en mode high-poly
* &amp;lbrack ;capture 3D&amp;rbrack ; Ajouter le résultat d&#39;origine ou une version au projet Sampler
* &amp;lbrack ; capture 3D&amp;rbrack ; Nouveau calque de post-traitement de Maillage pour décimer, déplier, reprojeter automatiquement les textures et baker les détails du calque de maillage sous-jacent
* &amp;lbrack ; capture 3D&amp;rbrack ; Nouveau calque de Transforme de Maillage pour mettre à l&#39;échelle, faire pivoter ou translater le calque de maillage sous-jacent
* &amp;lbrack ; Export&amp;rbrack ; New Export window
* &amp;lbrack ; Export&amp;rbrack ; Paramètres et interface utilisateur dédiés selon le type de ressource (matériau, éclairage d&#39;environnement, maillage)
* &amp;lbrack ; Export&amp;rbrack ; Export the maillage as USD, USDA, USDZ, glTF, glb, obj, fbx, stl
* &amp;lbrack ; Export&amp;rbrack ; Définir le type de matériau lors de l&#39;exportation de fichiers de Substance (SBSAR, SBS)
* &amp;lbrack ; UI&amp;rbrack ; Déplacer les paramètres de cache vers un nouvel onglet dans le menu contextuel Préférences
* Les viewports 2D et 3D de &amp;lbrack ;Application&amp;rbrack ; peuvent désormais être redimensionnés, permutés et empilés verticalement
* &amp;lbrack ;Application&amp;rbrack ; Nouvelle variable d&#39;environnement SAMPLER_RESOURCES_PATH pour ajouter des ressources de démarrage supplémentaires
* &amp;lbrack ; Scripting&amp;rbrack ; Ajout de variables d’environnement SAMPLER_PLUGIN_PATH et SAMPLER_SCRIPT_PATH pour importer des plug-ins et des scripts au démarrage
* &amp;lbrack ; Scripting&amp;rbrack ; Ajout de fonctions d&#39;exportation pour les matériaux, les éclairages d&#39;environnement et les objets 3D
* &amp;lbrack ; Scripting&amp;rbrack ; Ajout d&#39;identifiants, de valeurs par défaut, de valeurs minimales et maximales, de libellés et de valeurs d&#39;énumération aux paramètres
* &amp;lbrack ; Scripting&amp;rbrack ; Ajout de la fonction import_textures pour entrer une utilisation personnalisée lors de l&#39;importation d&#39;images

**Fixe :**

* &lbrack;Application&amp;rbrack ; Crash lors de l&#39;ouverture d&#39;un projet récent et de l&#39;enregistrement dans la boîte de dialogue de confirmation
* La boîte de dialogue Fichier &amp;lbrack ;Application&amp;rbrack ; empêche l&#39;ouverture des fichiers .ssa
* Les boîtes de dialogue du fichier &amp;lbrack ;Application&amp;rbrack ; peuvent apparaître dans une fenêtre en arrière-plan sur macOS
* &amp;lbrack ;Application&amp;rbrack ; crash potentiel lors de l&#39;ouverture de projets 3.2
* &amp;lbrack ; Application&amp;rbrack ; La sélection d&#39;un fichier ferme la boîte de dialogue Fichier avant d&#39;afficher les avertissements
* &amp;lbrack ; Paramètres exposés&amp;rbrack ; L&#39;exportation d&#39;éclairages d&#39;environnement paramétriques ne fonctionne pas
* &amp;lbrack ; Layers&amp;rbrack ; le lien « Cliquer ici pour parcourir » dans la pile de calques ne fonctionne plus
* &amp;lbrack ; Layers&amp;rbrack ; La peinture de plusieurs images dans le même calque ne fonctionne pas toujours
* &amp;lbrack ; Layers&amp;rbrack ; La définition d&#39;une image dans les propriétés du calque ne met pas à jour la vignette du sélecteur d&#39;images
* &amp;lbrack ; Layers&amp;rbrack ; Ajuster une ressource Sampler ajoutée en tant que calque ne fonctionne pas
* &amp;lbrack ;Project&amp;rbrack ; Mise à jour de ressource indésirable lors de l&#39;ouverture d&#39;un projet
* &amp;lbrack ; Scripting&amp;rbrack ; Naviguer vers le dossier du plug-in échoue parfois sous Windows
* &amp;lbrack ; Scripting&amp;rbrack ; Crash lors de l&#39;utilisation de &#39;open_project()&#39; dans un script Python
* L&#39;exportation du JPEG &amp;lbrack ;Scripting&amp;rbrack ; est manquante dans l&#39;API
* &amp;lbrack ; Scripting&amp;rbrack ; Le panneau Journal n&#39;est pas en lecture seule
* La valeur du paramètre &amp;lbrack ; Scripting&amp;rbrack ; image_picker ne fonctionne pas
* Icône d&#39;élément manquant pour les éclairages d&#39;environnement dans le panneau Projet &amp;lbrack ;UI&amp;rbrack ;
* Le menu déroulant Format d’&amp;lbrack ; UI&amp;rbrack ; Envoyer vers Designer dans les préférences peut être vide
* &amp;lbrack ; UI&amp;rbrack ; Certains boutons ont un style incorrect
* &amp;lbrack ; UI&amp;rbrack ; Le libellé chevauche les boutons dans les widgets Groupe de boutons
* La position de l&#39;info-bulle &amp;lbrack ;UI&amp;rbrack ; est incorrecte pour « Outils » dans le menu Définir la taille physique
* &amp;lbrack ; UI&amp;rbrack ; Lors de la modification de la langue, le menu Fichier est mal aligné

**Problèmes Connus :**

* &amp;lbrack ;capture 3D&amp;rbrack ; Lors de l&#39;utilisation de masques, la projection de texture peut être rompue
* &amp;lbrack ; capture 3D&amp;rbrack ; De petits artefacts peuvent apparaître sur votre objet si votre échelle dans la transforme du Maillage est trop petite
* &amp;lbrack ; capture 3D&amp;rbrack ; Le maillage exporté est peut-être vraiment petit. Réinitialiser l’échelle de la transforme du Maillage et réexporter
* &amp;lbrack ; Le sélecteur de couleurs&amp;rbrack ; Choisir une couleur sur un deuxième moniteur avec une résolution différente peut ne pas fonctionner
* Le widget d&#39;éclairage de forme &amp;lbrack ; Content&amp;rbrack ; ne fonctionne pas en mode projection sphérique
* Le Matériau &amp;lbrack ; d&#39;interopérabilité&amp;rbrack ; avec le displacement envoyé à Stager perdra les contrôles de displacement

## Version 3

### 3.4.1 Arancini

*(Publié Le 6 Octobre 2022)*

**Ajouté :**

* Écrans &amp;lbrack ; Onboarding&amp;rbrack ; New Welcome et What&#39;s New
* &amp;lbrack ; Onboarding&amp;rbrack ; Mise à jour de l’interface utilisateur de l’écran d’accueil
* &amp;lbrack ; Onboarding&amp;rbrack ; New Learn content in the Home screen
* &amp;lbrack ; Scripting&amp;rbrack ; Consigne une erreur dans le panneau Journal lorsqu&#39;une méthode n&#39;est pas reconnue
* &amp;lbrack ; Scripting&amp;rbrack ; Nouveau module ssa.assistants pour activer l&#39;impression dans le panneau Journal
* &amp;lbrack ; Application&amp;rbrack ; Prise en charge du nouveau widget de boutons côte à côte de Substance 3D Designer

**Fixe :**

* &amp;lbrack ; Export&amp;rbrack ; Crash lors de l&#39;exportation d&#39;un fichier .fichier sbsar référençant une image manquante
* &amp;lbrack ; Export&amp;rbrack ; Crash lors de l’exportation d’un fichier faisant référence à un fichier image corrompu
* &amp;lbrack ; Export&amp;rbrack ; L&#39;exportation d&#39;un fichier .fichier sbsar avec un calque de broderie crée un matériau gris
* &amp;lbrack ; Export&amp;rbrack ; L&#39;exportation d&#39;un matériau vers un fichier .sbs/fichier sbsar peut générer un matériau entièrement transparent
* Le paramètre Format normal d&#39;&amp;export&amp;rbrack ; n&#39;est pas exposé correctement dans les fichiers .sbs/.sbsar
* &amp;lbrack ; Export&amp;rbrack ; L&#39;exportation Sbs/sbsar d&#39;une pile de calques faisant référence à un fichier .svg est interrompue
* Le calque de Transforme &amp;lbrack ; Export&amp;rbrack ; n&#39;est pas exporté correctement / Enscape mis à jour - Paramètre prédéfini d&#39;exportation Revit
* &amp;lbrack ; Paramètres exposés&amp;rbrack ; Crash lors de la suppression d&#39;un calque contenant un paramètre exposé
* &amp;lbrack ; Paramètres exposés&amp;rbrack ; La mise à jour d&#39;un calque obsolète dans la pile de calques peut entraîner une liste corrompue de paramètres exposés
* Les paramètres &amp;lbrack ; de Paramètres exposés&amp;rbrack ; qui ne doivent pas être exportés le sont de toute façon
* &amp;lbrack ; Paramètres exposés&amp;rbrack ; La suppression d&#39;un filtre de fusion lors de la suppression d&#39;un calque n&#39;expose pas ses paramètres
* &amp;lbrack ; Paramètres exposés&amp;rbrack ; Les paramètres de texte interrompent les exportations .sbs/.sbsar
* &amp;lbrack ; Layers&amp;rbrack ; Crash lors de la dépose d&#39;une pile de calques dans une autre pile de calques
* crash &amp;lbrack ; Layers&amp;rbrack ; en cas d&#39;échec du chargement d&#39;un filtre
* &amp;lbrack ; Layers&amp;rbrack ; Impossible de recharger l&#39;image précédente lors de la réinitialisation du champ Image
* &amp;lbrack ; Layers&amp;rbrack ; Cannot undo/redo transforme tool changes
* Le calque de tampon de Clone &amp;lbrack ; Layers&amp;rbrack ; est bloqué après avoir cliqué sur « Réinitialiser tous les paramètres »
* &amp;lbrack ; Layers&amp;rbrack ; L&#39;utilisation des boutons de réinitialisation empêche de dessiner dans le champ Image
* &amp;lbrack ; Layers&amp;rbrack ; Le bouton Réinitialiser n&#39;efface pas le masque de dessin dans le champ Image
* &amp;lbrack ; Layers&amp;rbrack ; Le bouton Réinitialiser dans le champ Image ne fait rien si l&#39;utilisateur a peint quelque chose
* Le cache de rendu &amp;lbrack ; Layers&amp;rbrack ; ne fonctionne pas lors de l&#39;utilisation de l&#39;outil Pinceau
* Le calque &amp;lbrack ; Layers&amp;rbrack ; Supprimé peut toujours apparaître dans le panneau Propriétés
* Le calcul de calque &amp;lbrack ; Layers&amp;rbrack ; peut se bloquer lors du basculement entre les ressources du projet
* &amp;lbrack ;Project&amp;rbrack ; Parfois, Sampler ne parvient pas à ouvrir un projet à partir du disque
* &amp;lbrack ; vue 2D&amp;rbrack ; La Vue 2D revient toujours par défaut à la sortie Matériau

**Problèmes Connus :**

* &amp;lbrack ; Le sélecteur de couleurs&amp;rbrack ; Choisir une couleur sur un deuxième moniteur avec une résolution différente peut ne pas fonctionner
* Le widget d&#39;éclairage de forme &amp;lbrack ; Content&amp;rbrack ; ne fonctionne pas en mode projection sphérique
* Le Matériau &amp;lbrack ; d&#39;interopérabilité&amp;rbrack ; avec le displacement envoyé à Stager perdra les contrôles de displacement

### 3.4.0 Arancini

*(Publié Le 6 Septembre 2022)*

**Ajouté :**

* &amp;lbrack ; Paramètres exposés&amp;rbrack ; Nouveau Panneau Paramètres exposés
* &amp;lbrack ; Paramètres exposés&amp;rbrack ; Nouveau bouton au survol des paramètres pour exposer et annuler l&#39;exposition des paramètres du panneau Propriétés
* &amp;lbrack ; Paramètres exposés&amp;rbrack ; Nouveau menu contextuel accessible via un clic droit sur les paramètres pour exposer aux paramètres du panneau Propriétés et les rendre non visibles
* les Paramètres exposés &amp;lbrack ; Paramètres exposés&amp;rbrack ; sont répertoriés dans le Panneau Paramètres exposés
* &amp;lbrack ; Paramètres exposés&amp;rbrack ; Des points de couleur et des disques de couleur sont ajoutés à plusieurs endroits pour identifier facilement les paramètres exposés
* Les étiquettes de paramètres de &amp;lbrack ; Paramètres exposés&amp;rbrack ; peuvent être modifiées dans le Panneau Paramètres exposés
* &amp;lbrack ; Paramètres exposés&amp;rbrack ; Affiche un avertissement pour les paramètres non exportables
* &amp;lbrack ; Paramètres exposés&amp;rbrack ; Affiche un avertissement si vous déplacez un calque avec des paramètres de fusion exposés à un endroit où ils deviennent masqués
* les Paramètres exposés &amp;lbrack ; Paramètres exposés&amp;rbrack ; sont exportés aux formats SBS et SBSAR
* &amp;lbrack ; Metadata&amp;rbrack ; prend en charge les modèles de métadonnées personnalisés
* &amp;lbrack ; Metadata&amp;rbrack ; Nouveau modèle de métadonnées de propriétés physiques CLO
* &amp;lbrack ; Metadata&amp;rbrack ; Ajouter des icônes au survol pour ajouter/supprimer des métadonnées personnalisées
* &amp;lbrack ; Python API&amp;rbrack ; New Python API
* API &amp;lbrack ; Python API&amp;rbrack ; pour la création de ressources
* API &amp;lbrack ; Python API&amp;rbrack ; pour la gestion des calques
* API &amp;lbrack ; Python API&amp;rbrack ; pour la gestion des paramètres
* API &amp;lbrack ; Python API&amp;rbrack ; pour la gestion de projet
* &amp;lbrack ; Python API&amp;rbrack ; Un plug-in peut être activé et désactivé
* La documentation de l&#39;API &amp;lbrack ; Python est accessible dans le menu Aide
* &amp;lbrack ; Scripting&amp;rbrack ; Nouvelle section Plug-ins et nouveaux scripts dans le menu contextuel Préférences
* &amp;lbrack ; Scripting&amp;rbrack ; Créer et importer des plug-ins pour personnaliser l’interface de Sampler avec vos propres panneaux
* Les plug-ins &amp;lbrack ;Scripting&amp;rbrack ; font partie de l&#39;interface de Sampler et peuvent être ancrés et déplacés comme les panneaux Sampler standard
* &amp;lbrack ; Scripting&amp;rbrack ; Barre de boutons dédiée pour les plug-ins dans la barre d’outils de droite de Sampler
* &amp;lbrack ; Scripting&amp;rbrack ; Créer et importer des scripts pour exécuter une liste de tâches données
* &amp;lbrack ; Scripting&amp;rbrack ; Lancer des scripts Python via le menu Scripts
* &amp;lbrack ; Les plug-ins et les scripts de&amp;rbrack ; peuvent être supprimés, réordonnés et rechargés à partir de la fenêtre Préférences
* &amp;lbrack ; Scripting&amp;rbrack ; Added —run-script paramètres de ligne de commande
* &amp;lbrack ; Panneau Journaux&amp;rbrack ;
* &amp;lbrack ; Logs&amp;rbrack ; Panneau Activer les journaux de la fenêtre Préférences
* &amp;lbrack ; Logs&amp;rbrack ; Nouvelle barre d&#39;actions pour effacer, copier/coller, exporter les journaux
* &amp;lbrack ; Properties&amp;rbrack ; Nouveau bouton au survol des paramètres pour réinitialiser la valeur des paramètres
* &amp;lbrack ; Properties&amp;rbrack ; New menu contextuel accessible via un clic droit sur les paramètres pour réinitialiser leur valeur
* &amp;lbrack ;Content&amp;rbrack ; Image vers le Matériau (optimisé par l’IA) fonctionne désormais sur MacOS
* &amp;lbrack ;Moteur&amp;rbrack ; Mettre à jour le moteur de Substance vers la version 8.6.0

**Fixe :**

* &amp;lbrack ; L&#39;application&amp;rbrack ; pouvait avoir un crash à la fermeture lorsqu&#39;une génération de vignettes était en cours
* L&#39;application &amp;lbrack ;Application&amp;rbrack ; peut se mettre en crash lors de l&#39;utilisation de « Enregistrer sous » à la sortie
* L&#39;application &lbrack;Application&rbrack; peut se bloquer lors de l&#39;arrêt de MacOS
* &amp;lbrack ;Application&amp;rbrack ; L&#39;enregistrement avec la boîte de dialogue Couleur ouverte n&#39;enregistre pas ses modifications
* &amp;lbrack ; Export&amp;rbrack ; La convention de dénomination d&#39;utilisation n&#39;est pas correcte lors de l&#39;exportation
* &amp;lbrack ; Layers&amp;rbrack ; Déposer un matériau au-dessus d&#39;un filtre peut provoquer un crash
* &amp;lbrack ; Layers&amp;rbrack ; La mise à jour d&#39;une pile de calques obsolète peut entraîner la mise à jour de piles de calques indépendantes
* &amp;lbrack ; Les champs de métadonnées&amp;rbrack ; vides sont exportés
* &amp;lbrack ; Metadata&amp;rbrack ; Lorsqu&#39;il n&#39;y a qu&#39;un seul élément de métadonnées, l&#39;interface utilisateur vous permet de le réorganiser
* &amp;lbrack ;Project&amp;rbrack ; Compute ne se termine jamais après la duplication d&#39;un matériau
* L&#39;&amp;élément de projet lbrack;Project&rbrack; est dupliqué après l&#39;enregistrement initial du projet
* &amp;lbrack ;Project&amp;rbrack ; calculs inutiles lors du changement de ressource
* &amp;lbrack ; Rendu&amp;rbrack ; Certaines piles de calques ne s&#39;affichent pas correctement après la suppression d&#39;un calque
* &amp;lbrack ; Security&amp;rbrack ; Fix CVE-2015-20107
* Les sorties 2D &amp;lbrack ; UI&amp;rbrack ; peuvent être floues en fonction de la taille de la fenêtre
* L&#39;aperçu de la ressource &amp;lbrack ; UI&amp;rbrack ; peut rester ouvert en premier lorsque l&#39;application perd le focus
* Les coins arrondis de l&#39;écran de démarrage &amp;lbrack ; UI&amp;rbrack ; ont un arrière-plan carré opaque

**Problèmes Connus :**

* &amp;lbrack ; Le sélecteur de couleurs&amp;rbrack ; Choisir une couleur sur un deuxième moniteur avec une résolution différente peut ne pas fonctionner
* Le widget d&#39;éclairage de forme &amp;lbrack ; Content&amp;rbrack ; ne fonctionne pas en mode projection sphérique
* Le Matériau &amp;lbrack ; d&#39;interopérabilité&amp;rbrack ; avec le displacement envoyé à Stager perdra les contrôles de displacement

### 3.3.2 Courgettes

*(Publié Le 28 Juin 2022)*

**Fixe :**

* &amp;lbrack ;Application&amp;rbrack ; Corriger un crash potentiel lors de l&#39;ouverture d&#39;un projet
* &amp;lbrack ; Export&amp;rbrack ; Le redémarrage de Sampler interrompt la liste des paramètres prédéfinis d&#39;exportation personnalisés importés
* &amp;lbrack ;Interoperability&amp;rbrack ; Corriger le crash lorsqu’un matériau envoyé depuis Designer est supprimé, puis renvoyé depuis Designer
* &amp;lbrack ; Project&amp;rbrack ; Impossible de supprimer le dernier matériau ou éclairage d&#39;environnement s&#39;il s&#39;agit du dernier actif du projet
* &amp;lbrack ;Project&amp;rbrack ; Un clic droit sur un éclairage d&#39;environnement fait apparaître l&#39;astérisque « modifications non enregistrées »

**Problèmes Connus :**

* &amp;lbrack ; Le sélecteur de couleurs&amp;rbrack ; Choisir une couleur sur un deuxième moniteur avec une résolution différente peut ne pas fonctionner
* Le widget d&#39;éclairage de forme &amp;lbrack ; Content&amp;rbrack ; ne fonctionne pas en mode projection sphérique
* Le Matériau &amp;lbrack ; d&#39;interopérabilité&amp;rbrack ; avec le displacement envoyé à Stager perdra les contrôles de displacement

### 3.3.1 Courgettes

*(Publié Le 7 Juin 2022)*

**Ajouté :**

* &amp;lbrack ;Application&amp;rbrack ; Prise en charge native d’Apple Silicon (M1)
* &amp;lbrack ; UI&amp;rbrack ; Nouveau raccourci, touche C, pour parcourir les canaux dans la Vue 2D
* &amp;lbrack ; Tools&amp;rbrack ; Champ numérique pour modifier la valeur de couleur en niveaux de gris dans la barre d&#39;outils Pinceau

**Fixe :**

* &amp;lbrack ;Tools&amp;rbrack ; L’utilisation de l’outil Pinceau sous Windows avec une échelle d’interface utilisateur fractionnée (150 %) décale les traits
* &amp;lbrack ; Performance&amp;rbrack ; Améliorer la consommation de mémoire
* Les informations de la Taille physique &amp;lbrack ; Taille physique&amp;rbrack ; peuvent être manquantes lors de son activation
* Le défilement de la &amp;souris lbrack ; UI&amp;rbrack ; ne fonctionne parfois pas comme prévu lorsque vous appuyez sur la touche Alt
* L&#39;application &amp;lbrack ; peut se mettre en crash lors de l&#39;ouverture d&#39;un projet enregistré
* &amp;lbrack ; Application&amp;rbrack ; Crash lors du glisser-déposer de plusieurs images et de l&#39;utilisation de l&#39;importation de Textures dans la fenêtre Modèle de création de Matériaux
* &amp;lbrack ;Application&amp;rbrack ; crash potentiel lors de l&#39;enregistrement d&#39;un projet contenant un filtre personnalisé
* &amp;lbrack ; Application&amp;rbrack ; Parfois, l&#39;état de la touche Contrôle est perdu lors du changement d&#39;application
* &amp;lbrack ; Assets&amp;rbrack ; Crash lors du changement de nom d&#39;un dossier local

**Problèmes Connus :**

* &amp;lbrack ; Le sélecteur de couleurs&amp;rbrack ; Choisir une couleur sur un deuxième moniteur avec une résolution différente peut ne pas fonctionner
* Le widget d&#39;éclairage de forme &amp;lbrack ; Content&amp;rbrack ; ne fonctionne pas en mode projection sphérique
* Le Matériau &amp;lbrack ; d&#39;interopérabilité&amp;rbrack ; avec le displacement envoyé à Stager perdra les contrôles de displacement

### 3.3.0 Courgettes

*(Publié Le 17 Mai 2022)*

**Ajouté :**

* &amp;lbrack ;Content&amp;rbrack ; Nouveau filtre Remplissage d’après le contenu (Windows et Mac)
* &amp;lbrack ; Content&amp;rbrack ; Content-Aware Fill travaille sur les images, les matériaux PBR et les éclairages d&#39;environnement
* &amp;lbrack ;Content&amp;rbrack ; Ajouter le paramètre « Conserver la Répétition » à Image en Matériau (optimisé par l&#39;IA)
* &amp;lbrack ;Content&amp;rbrack ; Le Transforme de Perspective peut afficher une grille entre ses quatre points
* &amp;lbrack ;Interoperability&amp;rbrack ; Envoyer des matériaux à Adobe Substance 3D Stager
* &amp;lbrack ; Tools&amp;rbrack ; Centrez la transformation en appuyant sur Ctrl lors du redimensionnement du Transforme ou de l’outil Recadrage
* &amp;lbrack ; Tools&amp;rbrack ; Verrouillez le rapport au carré en appuyant sur Maj lors du redimensionnement du Transforme ou de l’outil Recadrage
* Le curseur de tampon de Clone &amp;lbrack ; Tools&amp;rbrack ; offre un aperçu de ce qui sera tamponné
* &amp;lbrack ;Tools&amp;rbrack ; Affichez un aperçu du contenu original dans le curseur de la Gomme lors de l&#39;utilisation du tampon de Clone
* &amp;lbrack ; Tools&amp;rbrack ; Ctrl+clic crée un tampon dans le calque Tampon de Clone
* &amp;lbrack ; Tools&amp;rbrack ; Les tampons de duplication successifs sont désormais regroupés dans un seul calque
* &amp;lbrack ; Tools&amp;rbrack ; Brush Toolbar UI Revamp
* &amp;lbrack ; Tools&amp;rbrack ; La position de la barre d&#39;outils Pinceau est persistante pendant une session
* &amp;lbrack ; Tools&amp;rbrack ; New brush répétition options by axe
* &amp;lbrack ; Tools&amp;rbrack ; Masquer/afficher l&#39;incrustation sur la Vue 2D lors de la peinture
* &amp;lbrack ; Tools&amp;rbrack ; New raccourci, touche X, pour basculer entre Pinceau et Gomme
* &amp;lbrack ; Tools&amp;rbrack ; New raccourci, « &amp;lbrack ; » « &amp;rbrack ; » pour modifier l&#39;épaisseur du pinceau
* &amp;lbrack ;Tools&amp;rbrack ; New raccourci, touche « E », pour basculer la Gomme
* &amp;lbrack ; vue 2D&amp;rbrack ; Nouveau mode de Projection sphérique lors de la création d&#39;un éclairage d&#39;environnement
* L&#39;outil &amp;lbrack ; vue 2D&amp;rbrack ; Brush est pris en charge avec le mode projection sphérique
* &amp;lbrack ; L&#39;outil de position vue 2D&amp;rbrack ; est pris en charge avec le mode projection sphérique
* &amp;lbrack ; vue 2D&amp;rbrack ; La fonction Annuler/Rétablir est prise en charge avec le mode projection sphérique
* &amp;lbrack ;vue 2D&amp;rbrack ; En Projection sphérique, définissez la position par défaut pour regarder au centre de l&#39;environnement
* &amp;lbrack ; vue 2D&amp;rbrack ; Nouveau contrôle d&#39;exposition
* &amp;lbrack ; UI&amp;rbrack ; Dans le panneau Propriétés, la modification de l&#39;image affiche la source du contenu (Image ou d&#39;un calque)
* &amp;lbrack ; UI&amp;rbrack ; Amélioration de l’arrière-plan déroulant des sorties de calque/matériau
* &amp;lbrack ; UI&amp;rbrack ; Nouvelle position des informations de résolution dans la vue 2D
* &amp;lbrack ; UI&amp;rbrack ; Nouvelle info-bulle avec raccourcis des commandes de navigation de la vue 3D
* &amp;lbrack ; UI&amp;rbrack ; Nouvelle info-bulle avec options de pinceau
* &amp;lbrack ; UI&amp;rbrack ; Nouvelle info-bulle avec raccourcis des commandes de navigation dans les projections
* &amp;lbrack ; Compound Filters&amp;rbrack ; Compound Filters gère les variations qui fonctionnent sur les images, les matériaux PBR et les éclairages d&#39;environnement
* &amp;lbrack ; Compound Filters&amp;rbrack ; Tweak order correspond à l&#39;ordre de liste des nœuds dans le filtre composé
* &amp;lbrack ; Compound Filters&amp;rbrack ; Les ajustements de différents nœuds avec le même groupe seront fusionnés dans un seul groupe dans le panneau Propriétés
* &amp;lbrack ; Application&amp;rbrack ; Dispose de paramètres de visionneuse dédiés par type de ressource

**Fixe :**

* &amp;lbrack ; L&#39;application&amp;rbrack ; peut avoir un crash lors du passage à Vue 2D
* &amp;lbrack ;Application&amp;rbrack ; Corriger un blocage ou un crash possible lors de l&#39;exportation multiple
* &amp;lbrack ;Application&amp;rbrack ; Rendre les valeurs par défaut des couches cohérentes avec Substance 3D Designer
* &amp;lbrack ;Application&amp;rbrack ; Le chargement d&#39;un projet ne déclenche pas le recalcul du matériau
* &amp;lbrack ;Application&amp;rbrack ; Mise à jour de l&#39;URL de texture de la documentation d&#39;importation
* &amp;lbrack ;Content&amp;rbrack ; Lors de l&#39;utilisation d&#39;un filtre composé, il demande à être mis à jour quand il ne devrait pas, lors du rechargement
* &amp;lbrack ;Content&amp;rbrack ; Les détails de la map height disparaissent lors de l&#39;utilisation de la Fusion d&#39;opacité
* &amp;lbrack ; UI&amp;rbrack ; Dans la boîte de dialogue Couleur, il est possible de sortir de la plage en utilisant les champs de texte du curseur
* La liste d&#39;utilisation de &amp;lbrack ; UI&amp;rbrack ; a une barre de défilement verticale inutile

**Problèmes Connus :**

* &amp;lbrack ; Le sélecteur de couleurs&amp;rbrack ; Choisir une couleur sur un deuxième moniteur avec une résolution différente peut ne pas fonctionner
* Le widget d&#39;éclairage de forme &amp;lbrack ; Content&amp;rbrack ; ne fonctionne pas en mode projection sphérique
* Le Matériau &amp;lbrack ; d&#39;interopérabilité&amp;rbrack ; avec le displacement envoyé à Stager perdra les contrôles de displacement

### 3.2.1 Yakitori

*(Publié Le 8 Mars 2022)*

**Ajouté :**

* &amp;lbrack ; Export&amp;rbrack ; Export dpi metadata in image files
* &amp;lbrack ; Taille physique&amp;rbrack ; Conserver le rapport avec les textures non carrées lors de la modification des dimensions physiques
* les métadonnées de Taille physique de &amp;lbrack ; Taille physique&amp;rbrack ; sont immédiatement appliquées lorsque la taille physique change
* &amp;lbrack ; UI&amp;rbrack ; Réglez le curseur de l&#39;échelle maximale de l&#39;Height afin qu&#39;il puisse influencer tout type de matériau lorsque la Taille physique est activée
* &amp;lbrack ; UI&amp;rbrack ; Nouvelles info-bulles sur les filtres de recherche dans le panneau Actifs
* &amp;lbrack ;UI&amp;rbrack ; Utilisez des info-bulles pour expliquer quand les boutons sont désactivés dans le panneau Actifs
* &amp;lbrack ; Content&amp;rbrack ; Mise à jour du filtre de contraste de luminosité

**Fixe :**

* Le bouton de rotation de &amp;lbrack ; vue 2D&amp;rbrack ; de 90° dans les outils Recadrage et Transformé ne fonctionne pas comme prévu
* Le widget de recadrage &amp;lbrack ;vue 2D&amp;rbrack ; est parfois manquant
* &amp;lbrack ; Application&amp;rbrack ; L&#39;effacement d&#39;un paramètre d&#39;image ne reconnecte pas le calque sous-jacent
* &amp;lbrack ; Application&amp;rbrack ; Crash à la fermeture après avoir enregistré un projet
* &amp;lbrack ; Application&amp;rbrack ; Crash lors du glisser-déposer du matériau actif dans une collection du panneau Actifs
* &amp;lbrack ; Application&amp;rbrack ; Glissez-déposez une ressource dans le viewport par crash
* &amp;lbrack ; Content&amp;rbrack ; Normal blend a un ajustement de la valeur de départ aléatoire
* Le filtre Snow de &amp;lbrack ;Content&amp;rbrack ; a une sortie normale incorrecte en fonction des valeurs des paramètres de neige fraîche et fondue
* Filtre &amp;lbrack ; Content&amp;rbrack ; Parquet : correction de seams inattendus
* &amp;lbrack ;Content&amp;rbrack ; Filtre de broderie : supprimer le fil dans le mappage métallique
* &amp;lbrack ;Content&amp;rbrack ; Arrondi aux inférieurs - Filtre : corriger le nombre de carreaux x et y
* &amp;lbrack ; Content&amp;rbrack ; Brique mural filter : sortie normale et height à 16 bits
* &amp;lbrack ; Export&amp;rbrack ; Le nom de fichier par défaut dans la fenêtre contextuelle d&#39;exportation n&#39;est pas le nom de matériau actuel
* &amp;lbrack ; Export&amp;rbrack ; L&#39;exportation avec rapport physique et paramètre prédéfini d&#39;exportation donne des dimensions incorrectes
* &amp;lbrack ; Export&amp;rbrack ; Métallique est manquant dans le paramètre prédéfini d&#39;exportation CLO
* &amp;lbrack ; Export&amp;rbrack ; Lorsque vous remplacez un paramètre prédéfini personnalisé d&#39;exportation, le nom d&#39;affichage n&#39;est pas mis à jour
* &amp;lbrack ; Les couches&amp;rbrack ; les couches personnalisées du premier calque inséré ne sont pas découvertes
* Le Matériau &amp;lbrack ; Layers&amp;rbrack ; est réévalué lors de la modification des réglages d&#39;un calque masqué
* Les info-bulles &amp;lbrack ; de localisation ne sont pas localisées dans le panneau Exporter
* &amp;lbrack ; Taille physique&amp;rbrack ; La désactivation de la Taille physique d&#39;un actif ne supprime pas l&#39;échelle physique
* La valeur d&#39;échelle d&#39;Height de &amp;lbrack ; Taille physique&amp;rbrack ; ne peut pas être définie en dehors des limites du curseur la première fois
* &amp;lbrack ;Taille physique&amp;rbrack ; L&#39;importation d&#39;une image sans taille physique empêche l&#39;ouverture du projet
* La Taille physique &amp;lbrack ; Taille physique&amp;rbrack ; est définie par erreur sur zéro lorsqu&#39;elle est manquante
* l&#39;état de la case à cocher Taille physique&amp;rbrack ; Taille physique de l&#39;échelle physique n&#39;est pas mis à jour la première fois qu&#39;elle est affichée
* &amp;lbrack ; UI&amp;rbrack ; Matériau de base et Normal à l&#39;Height n&#39;ont pas de catégorie
* Le curseur &amp;lbrack ; UI&amp;rbrack ; est parfois invisible lorsque vous peignez une image
* &amp;lbrack ; UI&amp;rbrack ; Désactiver les options « Copier tout » et « Couper tout » dans le menu d&#39;édition d&#39;un champ de texte s&#39;il est vide
* Les noms des filtres &amp;lbrack ; UI&amp;rbrack ; comportent des caractères incorrects
* Le bouton de verrouillage de la Taille physique &amp;lbrack ; UI&amp;rbrack ; n&#39;a pas le style correct
* &amp;lbrack ; UI&amp;rbrack ; Le bouton de fermeture dans la barre de recherche du panneau Actifs n&#39;efface pas la chaîne de recherche

**Problèmes Connus :**

* &amp;lbrack ; Le sélecteur de couleurs&amp;rbrack ; Choisir une couleur sur un deuxième moniteur avec une résolution différente peut ne pas fonctionner

### 3.2.0 Yakitori

*(Publié Le 25 Janvier 2022)*

**Ajouté :**

* &amp;lbrack ; Taille physique&amp;rbrack ; Nouveau panneau de Taille physique
* &amp;lbrack ; Taille physique&amp;rbrack ; Ajouter des options de Taille physique à la fenêtre Modèle de création de Matériau
* &amp;lbrack ; Taille physique&amp;rbrack ; Ajouter un outil de mesure de Taille physique
* &amp;lbrack ; Taille physique&amp;rbrack ; Outil d&#39;auto-mesure Ajouter une Taille physique
* &amp;lbrack ; Taille physique&amp;rbrack ; Outil de diagnostic Ajouter une Taille physique
* &amp;lbrack ; Taille physique&amp;rbrack ; Autoriser la définition de la valeur z de la Taille physique
* &amp;lbrack ; Taille physique&amp;rbrack ; Widget déroulant pour définir le niveau de zoom dans la Vue 2D
* &amp;lbrack ; Taille physique&amp;rbrack ; Nouvelle option « Afficher avec rapport physique » dans le menu déroulant du niveau de zoom
* &amp;lbrack ; Taille physique&amp;rbrack ; Nouvelle option « Adapter à la taille physique » dans le niveau de zoom déroulant
* &amp;lbrack ; Taille physique&amp;rbrack ; Afficher la Taille physique dans la Vue 2D
* &amp;lbrack ; Taille physique&amp;rbrack ; Afficher la Taille physique dans le viewport 3D
* &amp;lbrack ; Taille physique&amp;rbrack ; Dans la boîte de dialogue d&#39;importation d&#39;image, affichez la profondeur de taille physique si une map height a été importée
* &amp;lbrack ; Taille physique&amp;rbrack ; Afficher la Taille physique dans le menu contextuel de l&#39;actif
* &amp;lbrack ; Taille physique&amp;rbrack ; Définissez l&#39;unité de longueur dans les Préférences
* &amp;lbrack ; Taille physique&amp;rbrack ; Exporter les textures en respectant le rapport physique
* &amp;lbrack ; Metadata&amp;rbrack ; Possibilité d&#39;ajouter des métadonnées personnalisées à une ressource créée par l&#39;utilisateur
* &amp;lbrack ; Export&amp;rbrack ; Export custom metadata to .sbs(ar) files
* &amp;lbrack ; Export&amp;rbrack ; Exporter les métadonnées de description, de catégorie, d&#39;auteur et de balises vers les fichiers .sbs(ar)
* &amp;lbrack ; Export&amp;rbrack ; Export the Taille physique to .sbs(ar) files
* &amp;lbrack ; Export&amp;rbrack ; Définir le paramètre de compression .fichier sbsar
* &amp;lbrack ; Export&amp;rbrack ; Export the asset thumbnail to .sbs(ar) files
* &amp;lbrack ; Export&amp;rbrack ; Définir le type de graphe lors de l&#39;exportation d&#39;un fichier .sbs(ar)
* &amp;lbrack ;Application&amp;rbrack ; Realtime Moteur 2021 n’est plus disponible
* &amp;lbrack ; Application&amp;rbrack ; Annuler/Rétablir prend désormais en charge les modifications des curseurs de Répétition (U,V) et d&#39;échelle height
* &amp;lbrack ;Rendering&amp;rbrack ; Générer le cache disque lorsque la ressource créée est enregistrée
* &amp;lbrack ; Assets&amp;rbrack ; Utilisez Ctrl+clic pour activer plusieurs filtres de type d’actif dans le panneau Ressources
* &amp;lbrack ; UI&amp;rbrack ; Possibilité de verrouiller les curseurs de Répétition (U,V)
* &amp;lbrack ; UI&amp;rbrack ; Ajouter un menu contextuel avec « Copier », « Couper », « Coller », « Copier tout » et « Couper tout » dans les champs de texte
* &amp;lbrack ; UI&amp;rbrack ; Unité de longueur (mètres, pouces, parsecs, ...) prise en charge dans les libellés et les champs de texte
* &amp;lbrack ; UI&amp;rbrack ; L&#39;utilisateur peut définir la précision décimale utilisée pour afficher les nombres
* &amp;lbrack ; UI&amp;rbrack ; Utilisez des unités dans les fenêtres de mesure partout où c&#39;est pertinent
* &amp;lbrack ; Localization&amp;rbrack ; Le nom par défaut de la nouvelle ressource est maintenant localisé
* &amp;lbrack ; Content&amp;rbrack ; Nouveau générateur d&#39;armure de tissu
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre de changement de canal
* &amp;lbrack ;Content&amp;rbrack ; Tous les filtres concernés sont désormais conscients de la Taille physique
* &amp;lbrack ; Content&amp;rbrack ; Nouvelles icônes de finition en bois
* &amp;lbrack ;Content&amp;rbrack ; Tous les filtres sont désormais compatibles avec les canaux Adobe Standard Material (ASM)
* Les filtres &amp;lbrack ; Content&amp;rbrack ; peuvent désormais avoir une variante « environnement »

**Fixe :**

* &amp;lbrack ; vue 2D&amp;rbrack ; Le canal reste dans la liste lorsqu&#39;il est supprimé
* &amp;lbrack ; Application&amp;rbrack ; Impossible de dupliquer une ressource chargée à partir de l&#39;explorateur de fichiers du système d&#39;exploitation
* &amp;lbrack ; Application&amp;rbrack ; Crash à la sortie
* &amp;lbrack ;Application&amp;rbrack ; Crash parfois lorsque vous cliquez sur « Ressources de démarrage » dans le panneau Ressources
* &amp;lbrack ; Application&amp;rbrack ; Crash lors de la suppression d&#39;un matériau
* La variable d&#39;environnement « SUBSTANCE_DISABLE_SPECIFIC_FEATURES » de &amp;lbrack ;Application&amp;rbrack ; est toujours active lorsqu&#39;elle est définie sur « 0 » ou « ».
* &amp;lbrack ; Application&amp;rbrack ; Figer lors de l&#39;enregistrement d&#39;un projet avec plusieurs matériaux
* &amp;lbrack ; Application&amp;rbrack ; L&#39;importation d&#39;une image peut entraîner un crash
* &amp;lbrack ;Application&amp;rbrack ; Ressources de démarrage manquantes au premier lancement
* &amp;lbrack ; Export&amp;rbrack ; L&#39;exportation d&#39;une ressource entraîne parfois un crash
* &amp;lbrack ; Layers&amp;rbrack ; Impossible d&#39;importer des images lorsque le panneau Calques est fermé ou invisible
* &amp;lbrack ; Layers&amp;rbrack ; La modification de la langue entraîne le recalcul de l&#39;actif actuel
* &amp;lbrack ; Layers&amp;rbrack ; La modification de l&#39;utilisation d&#39;une image importée ne met pas à jour la variante de filtre à utiliser
* &amp;lbrack ; Layers&amp;rbrack ; Image to Matériau (AI) n&#39;est parfois pas calculé lors de l&#39;ajustement des calques en dessous
* &amp;lbrack ; Layers&amp;rbrack ; Image to Matériau (AI) est parfois recalculé lorsque cela n&#39;est pas nécessaire
* &amp;lbrack ; Layers&amp;rbrack ; Aucune mise à jour n&#39;est suggérée lorsqu&#39;un filtre personnalisé est mis à jour sur le disque
* &amp;lbrack ; Layers&amp;rbrack ; La couche normale a parfois un format de pixels incorrect
* &amp;lbrack ; Layers&amp;rbrack ; Certains calques sont toujours calculés même lorsqu&#39;ils ne sont pas visibles
* &amp;lbrack ; Layers&amp;rbrack ; Les outils Vue 2D peuvent être rompus lorsque vous activez/désactivez la visibilité d&#39;un calque
* &amp;lbrack ; Layers&amp;rbrack ; L&#39;interface utilisateur se fige lors de l&#39;utilisation de Image vers Matériau (AI)
* &amp;lbrack ; Layers&amp;rbrack ; Le fait de basculer la visibilité du calque de filtre de Transforme casse l&#39;outil Vue 2D et peut entraîner un crash
* &amp;lbrack ; Layers&amp;rbrack ; Trop de recalculs lors de la suppression d&#39;un calque de la pile de calques
* &amp;lbrack ; Layers&amp;rbrack ; Lorsqu&#39;un filtre complexe contient une entrée/sortie inhabituelle ou personnalisée, Sampler ne la calcule pas
* &amp;lbrack ; Le panneau Actifs de performance&amp;rbrack ; est lent à s&#39;ouvrir
* &amp;lbrack ; Performance&amp;rbrack ; Éviter de recalculer inutilement la pile de calques
* &amp;lbrack ; Performance&amp;rbrack ; Le chargement des ressources du projet prend trop de temps
* Le cache de rendu &amp;lbrack ; Performance&amp;rbrack ; sur le disque ne peut pas être utilisé
* &amp;lbrack ; Performance&amp;rbrack ; Le basculement entre les calques est lent
* &amp;lbrack ; Performance&amp;rbrack ; L&#39;ajustement d&#39;un matériau ou d&#39;un filtre est lent
* &amp;lbrack ;Project&amp;rbrack ; L&#39;enregistrement d&#39;un projet en quittant peut entraîner un crash
* &amp;lbrack ;Rendering&amp;rbrack ; La suppression d&#39;une image peut supprimer toutes les sorties
* &amp;lbrack ; Rendu&amp;rbrack ; Le temps de rendu affiché dans le viewport est incorrect lors de l&#39;ajustement
* &amp;lbrack ; UI&amp;rbrack ; Impossible de faire défiler verticalement dans la fenêtre contextuelle d’exportation si nécessaire
* &amp;lbrack ; UI&amp;rbrack ; Il est possible d&#39;ouvrir la fenêtre contextuelle d&#39;exportation lorsqu&#39;il n&#39;y a rien à exporter
* &amp;lbrack ; UI&amp;rbrack ; Certaines fenêtres ne défilent pas si leur contenu déborde
* Les champs de texte &amp;lbrack ; UI&amp;rbrack ; ne sont pas sélectionnés lorsque vous cliquez dessus ou que vous ouvrez un menu
* &amp;lbrack ; UI&amp;rbrack ; Le nom du mode de fusion dans le panneau des propriétés est parfois incorrect
* &amp;lbrack ; UI&amp;rbrack ; L&#39;option Enregistrer du menu Fichier est parfois grisée
* &amp;lbrack ; UI&amp;rbrack ; Le champ de texte ne disparaît pas après avoir renommé deux matériaux
* &amp;lbrack ; UI&amp;rbrack ; Typo dans la fenêtre contextuelle des préférences

**Problèmes Connus :**

* &amp;lbrack ; Le sélecteur de couleurs&amp;rbrack ; Choisir une couleur sur un deuxième moniteur avec une résolution différente peut ne pas fonctionner

### 3.1.2 Xocoatl

*(Publié Le 14 Décembre 2021)*

**Fixe :**

* &amp;lbrack ;Interoperability&amp;rbrack ; Open .fichier sbsar with Substance 3D Sampler from Bridge peut échouer sous Windows
* &amp;lbrack ; Layers&amp;rbrack ; Le déplacement du seul calque sous lui-même entraîne le crash
* Le bouton des paramètres du canal &amp;lbrack ;UI&amp;rbrack ; disparaît lors du changement de langue
* &amp;lbrack ;UI&amp;rbrack ; Le nom du matériau dans le panneau Propriétés disparaît après l&#39;enregistrement du projet
* &amp;lbrack ; Assets&amp;rbrack ; Cliquer sur « Toutes les bibliothèques » peut entraîner un crash

**Problèmes Connus :**

* Le calcul lourd &amp;lbrack ; Realtime Moteur 2021&amp;rbrack ; peut effectuer le crash de l’application
* &amp;lbrack ;Realtime Moteur 2021&amp;rbrack ; Realtime Moteur 2021 effectuera le crash sur un ordinateur Windows sur lequel le processeur AMD et le GPU Nvidia sont installés
* &amp;lbrack ; Le sélecteur de couleurs&amp;rbrack ; Choisir une couleur sur un deuxième moniteur avec une résolution différente peut ne pas fonctionner

### 3.1.1 Xocoatl

*(Publié Le 24 Novembre 2021)*

**Ajouté :**

* &amp;lbrack ;Interoperability&amp;rbrack ; Envoyer des ressources (SBS ou SBSAR) à Substance 3D Designer
* &lbrack;Interopérabilité&amp;rbrack ; Définissez dans les préférences le format par défaut pour l&#39;interopérabilité avec Substance 3D Designer
* &amp;lbrack ;Interoperability&amp;rbrack ; Recevoir plusieurs ressources d’Adobe Bridge
* &amp;lbrack ; UI&amp;rbrack ; Nouveau widget Générateur aléatoire
* &amp;lbrack ; UI&amp;rbrack ; Mise à jour du menu contextuel
* &amp;lbrack ; Assets&amp;rbrack ; Faites glisser et déposez des images du panneau Actifs vers le panneau Propriétés
* &amp;lbrack ; Project&amp;rbrack ; Les noms de fichier sont nettoyés pour éviter certains caractères spécifiques
* &amp;lbrack ; Branding&amp;rbrack ; Icône de fichier de mise à jour pour les fichiers SBSAR
* &amp;lbrack ;Moteur&amp;rbrack ; Substance Engine de mise à jour version 8.3.0

**Fixe :**

* &amp;brack ; Content&amp;rbrack ; Crop - Conserver le rapport lors du recadrage d&#39;images non carrées
* &amp;lbrack ;Content&amp;rbrack ; Transforme : la transformation horizontale n’est pas inversée lors de l’utilisation du widget
* &amp;brack ; Content&amp;rbrack ; Gravel : correction de la peinture de masque personnalisée sur tous les canaux
* &amp;lbrack ;Content&amp;rbrack ; Arrondi aux inférieurs - résolvez les problèmes de répétition et de répétition des motifs
* &amp;lbrack ; Assets&amp;rbrack ; Griser l’option Adobe Bridge si elle n’est pas installée
* &amp;brack ; Sélecteur de couleurs&amp;rbrack ; La touche Échap ferme le sélecteur de couleurs
* &amp;lbrack ; Rendering&amp;rbrack ; Fix Scattering Distance Scale with using greyscale input
* Les options &amp;lbrack ; Partager&amp;rbrack ; Envoyer vers sont uniquement disponibles avec des licences Adobes
* &amp;lbrack ; Project&amp;rbrack ; Résoudre un problème de performances de la mémoire

**Problèmes Connus :**

* Le calcul lourd &amp;lbrack ; Realtime Moteur 2021&amp;rbrack ; peut effectuer le crash de l’application
* &amp;lbrack ;Realtime Moteur 2021&amp;rbrack ; Realtime Moteur 2021 effectuera le crash sur un ordinateur Windows sur lequel le processeur AMD et le GPU Nvidia sont installés
* &amp;lbrack ; Le sélecteur de couleurs&amp;rbrack ; Choisir une couleur sur un deuxième moniteur avec une résolution différente peut ne pas fonctionner

### 3.1.0 Xocoatl

*(Publié Le 28 Septembre 2021)*

**Ajouté :**

* &amp;brack ; Sélecteur de couleurs&amp;rbrack ; Nouvelle interface utilisateur du sélecteur de couleurs
* &amp;lbrack ; Sélecteur de couleurs&amp;rbrack ; Affichez un aperçu côte à côte des couleurs actuelle et précédente
* &amp;lbrack ; Sélecteur de couleurs&amp;rbrack ; saisissez votre couleur sous forme hexadécimale
* &amp;brack ; Sélecteur de couleurs&amp;rbrack ; Nouvelle pipette avec aperçu des couleurs
* &amp;lbrack ; Sélecteur de couleurs&amp;rbrack ; La pipette peut choisir une couleur en dehors de Sampler
* &amp;lbrack ; Sélecteur de couleurs&amp;rbrack ; Ajustez votre couleur dans les espaces colorimétriques RGB ou HSV
* &amp;lbrack ; Sélecteur de couleurs&amp;rbrack ; Enregistrer et gérer les nuances
* &amp;lbrack ; Interoperability&amp;rbrack ; Edit images in Illustrator from Image Import layer or Image parameters
* &amp;lbrack ; Interoperability&amp;rbrack ; Edit images in Photoshop from Image Import layer or Image parameters
* &amp;lbrack ; Widget&amp;rbrack ; New Crop Widget
* &amp;lbrack ; Widget&amp;rbrack ; Appuyez sur Entrée pour valider votre recadrage
* &amp;lbrack ; Widget&amp;rbrack ; Le widget Recadrage lit la taille de l&#39;image pour l&#39;adapter au widget et conserver le rapport lors du redimensionnement
* &amp;lbrack ; UI&amp;rbrack ; Nouvelle interface utilisateur du curseur de redimensionnement
* &amp;lbrack ; Application&amp;rbrack ; Ajouter la sélection du format normal dans les préférences
* &amp;lbrack ; Application&amp;rbrack ; Le format normal dans les calques d&#39;importation d&#39;images suit le format normal par défaut défini dans les préférences
* &amp;lbrack ;Application&amp;rbrack ; Dans Vue 2D, la normale s&#39;affiche selon le format défini dans les préférences
* &amp;lbrack ; Application&amp;rbrack ; La normale est exportée dans le format normal défini dans les préférences
* &amp;lbrack ; Export&amp;rbrack ; Ajouter un paramètre de format normal aux exportations SBS et Fichier sbsar
* &amp;lbrack ; Export&amp;rbrack ; Ajouter des paramètres de shader aux exportations SBS et Fichier sbsar
* &amp;lbrack ; Export&amp;rbrack ; Définir la résolution par défaut des graphes SBS exportés
* &amp;lbrack ; Compound Filters&amp;rbrack ; Assemblez les filtres SSA avec 7z
* &amp;lbrack ; Compound Filters&amp;rbrack ; Ajouter des métadonnées de catégorie dans les filtres composés
* &amp;lbrack ; Compound Filters&amp;rbrack ; Compound Filters peut comporter une vignette incorporée
* &amp;lbrack ; Compound Filters&amp;rbrack ; Ajout de l&#39;extension Compound Filters (.ssafilter) à la boîte de dialogue Obtenir le contenu
* &amp;lbrack ; Compound Filters&amp;rbrack ; Import Compound Filters (.ssafilter) in the Assets panel
* &amp;lbrack ;Moteur&amp;rbrack ; Mettre à jour Substance moteur vers la version 8.2.0

**Fixe :**

* &amp;lbrack ; Application&amp;rbrack ; Les dossiers locaux connectés peuvent se bloquer
* &amp;lbrack ; Application&amp;rbrack ; Crash à la sortie
* crash &amp;lbrack ;Application&amp;rbrack ; lors du lancement de deux instances de Sampler
* &amp;lbrack ; Content&amp;rbrack ; Le filtre de recadrage a un réglage de vitesse aléatoire
* &amp;lbrack ;Content&amp;rbrack ; Certains matériaux de Substance ne sont parfois pas mis à niveau
* &amp;lbrack ; Export&amp;rbrack ; Crash lors de l&#39;exportation avec un nouveau paramètre prédéfini personnalisé
* &amp;lbrack ; Export&amp;rbrack ; La taille estimée du package est manquante dans la fenêtre contextuelle d&#39;exportation
* &amp;lbrack ; Export&amp;rbrack ; Correction de la fuite de mémoire lors de l’exportation de fichiers SBS et SBSAR
* &amp;lbrack ; Compound Filters&amp;rbrack ; Les filtres composés peuvent avoir des entrées en double
* &amp;lbrack ; Compound Filters&amp;rbrack ; Crash si un filtre a des références non satisfaites
* &amp;lbrack ; Compound Filters&amp;rbrack ; Crash lors de la réorganisation d&#39;une pile de calques contenant un filtre composé
* &amp;lbrack ; Compound Filters&amp;rbrack ; Le rendu se bloque parfois
* &amp;lbrack ; Image Import&amp;rbrack ; L&#39;importation d&#39;une image déclenche plusieurs rendus
* &amp;lbrack ; Layers&amp;rbrack ; Crash en cas d&#39;annulation/de rétablissement
* crash &amp;lbrack ; Layers&amp;rbrack ; lors de l&#39;ajout d&#39;un Matériau de base
* &amp;lbrack ; Layers&amp;rbrack ; Crash lors de l&#39;utilisation d&#39;une image non valide comme éclairage d&#39;environnement
* &amp;lbrack ; Layers&amp;rbrack ; Corriger l&#39;importation en double lors de l&#39;insertion d&#39;un filtre à plusieurs graphes
* &amp;lbrack ; Layers&amp;rbrack ; La réorganisation des calques ne fonctionne pas toujours
* &lbrack;Project&amp;rbrack ; Crash lors du chargement d&#39;un fichier de projet incomplet
* crash &amp;lbrack ;Project&amp;rbrack ; lors de l&#39;ouverture d&#39;un projet corrompu
* &amp;lbrack ; Project&amp;rbrack ; Certaines ressources peuvent disparaître d&#39;un projet
* &amp;lbrack ;Properties&amp;rbrack ; Corriger les paramètres prédéfinis manquants du filtre
* Impossible de définir les paramètres d&#39;&amp;angle de l&#39;interface utilisateur
* &amp;lbrack ; UI&amp;rbrack ; Les métadonnées des filtres s’affichent dans le panneau Actifs
* &amp;lbrack ; UI&amp;rbrack ; Le regroupement par catégorie masque les filtres
* &amp;lbrack ;UI&amp;rbrack ; Problème de défilement dans le panneau Actifs
* &amp;lbrack ; UI&amp;rbrack ; Le panneau d’exportation dispose désormais d’une barre de défilement
* &amp;lbrack ; UI&amp;rbrack ; La vignette ne s&#39;affiche pas pour certains formats d&#39;image dans le sélecteur d&#39;images

**Problèmes Connus :**

* Le calcul lourd &amp;lbrack ; Realtime Moteur 2021&amp;rbrack ; peut effectuer le crash de l’application
* &amp;lbrack ;Realtime Moteur 2021&amp;rbrack ; Realtime Moteur 2021 effectuera le crash sur un ordinateur Windows sur lequel le processeur AMD et le GPU Nvidia sont installés
* &amp;lbrack ; Le sélecteur de couleurs&amp;rbrack ; Choisir une couleur sur un deuxième moniteur avec une résolution différente peut ne pas fonctionner

### 3.0.1 Gaufre

*(Publié Le 27 Juillet 2021)*

**Ajouté :**

* &amp;lbrack ; Brush&amp;rbrack ; Activer les couleurs dans l&#39;outil Pinceau si l&#39;entrée d&#39;image le prend en charge
* &amp;brack ; Pinceau&amp;rbrack ; Maintenir la touche Maj enfoncée dans l&#39;outil Pinceau permet de tracer des lignes droites
* &amp;lbrack ; Brush&amp;rbrack ; Affiche un aperçu de la ligne en maintenant la touche Maj enfoncée dans l&#39;outil Pinceau
* L&#39;outil &amp;brack ; Brush&amp;rbrack ; Brush prend désormais en charge les fonctions annuler et rétablir
* &amp;lbrack ; vue 2D&amp;rbrack ; La couleur par défaut de l&#39;entrée d&#39;image est utilisée lors de la peinture
* &amp;lbrack ; Layers&amp;rbrack ; Read Substance input default value in SBSAR files
* &amp;lbrack ; Rendering&amp;rbrack ; Permet de combiner l&#39;height avec la normale
* Prise en charge de la diffusion sub-surface &amp;lbrack ; Rendering&amp;rbrack ; (non disponible sur MacOS)
* &amp;lbrack ; Assets&amp;rbrack ; Utiliser le type de graphe SBSAR pour déterminer le type d&#39;actif
* &amp;lbrack ; Assets&amp;rbrack ; Meilleures performances pour la recherche et la découvrabilité des actifs dans le panneau Actifs
* &amp;lbrack ; Assets&amp;rbrack ; Ajout d’une entrée « Toutes les bibliothèques » dans le panneau Actifs qui affiche tous les actifs de toutes vos bibliothèques
* &amp;lbrack ; Assets&amp;rbrack ; L&#39;utilisateur peut désormais choisir de regrouper les actifs par catégorie ou type
* &amp;lbrack ; Import&amp;rbrack ; Détection automatique des textures d&#39;anisotropie, de manteau, d&#39;éclat et de specular edge color à l&#39;importation
* &amp;lbrack ; UI&amp;rbrack ; Remplacer le titre du panneau avec une icône
* &amp;lbrack ; UI&amp;rbrack ; Mise à jour du style des champs de texte
* &amp;lbrack ;UI&amp;rbrack ; Nouveau texte de description dans la fenêtre de création du modèle d&#39;Éclairage d&#39;environnement
* &amp;lbrack ; Application&amp;rbrack ; Exporter les ressources avec la résolution actuelle lors de l&#39;envoi vers une application externe
* La résolution par défaut du Matériau d’&amp;lbrack ;Application&amp;rbrack ; est désormais de 2048\*2048 (1024\*1024 sous macos)
* &amp;lbrack ;Content&amp;rbrack ; Nouveaux motifs dans le filtre des vignettes d&#39;Arrondi aux inférieurs
* &amp;lbrack ; Content&amp;rbrack ; Nouveau mode bicolore dans le filtre Remplacement de couleur

**Fixe :**

* &amp;lbrack ; vue 2D&amp;rbrack ; Le premier trait de l&#39;outil pinceau est parfois interrompu
* &amp;lbrack ; vue 2D&amp;rbrack ; Ressources gratuites lorsque l&#39;outil pinceau n&#39;est pas visible
* &amp;lbrack ; vue 2D&amp;rbrack ; Utilisez le curseur de redimensionnement à droite dans le widget de transforme
* Les widgets &amp;lbrack ; vue 2D&amp;rbrack ; ne s&#39;affichent pas si l&#39;utilisateur a déjà effectué un panoramique dans la Vue 2D
* crash &amp;lbrack ;Application&amp;rbrack ; lors de l’ouverture d’un projet dont le workflow est interrompu
* &amp;lbrack ;Application&amp;rbrack ; Corriger l&#39;arrêt de l&#39;application pour éviter d&#39;inonder le journal d&#39;erreurs inutiles
* &amp;lbrack ; Application&amp;rbrack ; Rétablir, supprimer et enregistrer les raccourcis clavier ne fonctionnent pas sur certains systèmes d&#39;exploitation
* &amp;lbrack ; Application&amp;rbrack ; Annuler/rétablir la modification de l&#39;utilisation de l&#39;image dans le calque d&#39;importation est rompue
* &amp;lbrack ; Export&amp;rbrack ; Les images exportées en couleur d&#39;émission ont un nom erroné
* &amp;lbrack ;Export&amp;rbrack ; Environment est de 8 bits lors de l&#39;utilisation de l&#39;exportation SBSAR
* &amp;lbrack ; Export&amp;rbrack ; Supprime les espaces superflus dans les noms de fichiers d&#39;image exportés
* &amp;lbrack ; Export&amp;rbrack ; Remplacement ou suppression d&#39;un paramètre d&#39;exportation prédéfini personnalisé par crashs
* &amp;lbrack ; Layers&amp;rbrack ; Éviter le crash en cas d&#39;incompatibilité du nombre d&#39;entrées
* crash &amp;lbrack ; Layers&amp;rbrack ; lors de l&#39;insertion d&#39;un calque de Matériau de base
* Le nombre d&#39;entrées du filtre &amp;lbrack ; Layers&amp;rbrack ; est limité à la valeur par défaut
* &amp;lbrack ; Layers&amp;rbrack ; Redo remplace par erreur le type de Fusion par Fusion Height
* &amp;lbrack ; Layers&amp;rbrack ; Remove drop zone above input headers
* &amp;lbrack ; Layers&amp;rbrack ; Layers sont insérés au mauvais endroit autour des en-têtes d&#39;entrée
* Le bouton &amp;lbrack ; Layers&amp;rbrack ; Reset all settings ne réinitialise pas les valeurs des widgets déroulants
* &amp;lbrack ; Layers&amp;rbrack ; Annuler/rétablir lors de la modification d’une image sur le calque d’importation d’image marque le projet comme modifié et donc permet d’enregistrer
* Les utilisations de &amp;calques&amp;rbrack ; peuvent être arrêtées par les calques de fusion
* &lbrack;Project&amp;rbrack ; Crash lors du chargement d&#39;un projet hérité avec un dossier de dépendances manquant
* crash de &amp;lbrack ;Project&amp;rbrack ; lors de l&#39;utilisation d&#39;annuler/rétablir après l&#39;enregistrement
* &amp;lbrack ; Project&amp;rbrack ; L&#39;ouverture d&#39;un Fichier sbsar contenant un éclairage d&#39;environnement crée un actif de matériau
* &amp;lbrack ;Project&amp;rbrack ; Renommer un matériau peut déclencher une génération de vignettes
* &amp;lbrack ;Project&amp;rbrack ; L&#39;enregistrement après avoir renommé un matériau marque le projet comme non modifié
* &amp;lbrack ;Project&amp;rbrack ; Certaines modifications apportées après avoir renommé un matériau ne sont pas enregistrées
* &amp;lbrack ;Rendering&amp;rbrack ; Des points lumineux sont visibles sur l&#39;environnement avec le moteur en temps réel 2020
* &amp;lbrack ;Rendu&amp;rbrack ; Crash lors du redimensionnement à l’aide de Real Time Moteur 2021
* &amp;lbrack ; Rendu&amp;rbrack ; Recalculer les ombres au niveau de l&#39;height
* Les dossiers &amp;lbrack ; Assets&amp;rbrack ; connectés arrêtent l&#39;indexation des nouveaux actifs lors de l&#39;ajout d&#39;un fichier non valide
* &amp;lbrack ; Assets&amp;rbrack ; Crash lors de la connexion d&#39;un dossier local avec de nombreux matériaux
* &amp;lbrack ;UI&amp;rbrack ; boutons d&#39;affichage 2D/3D sans info-bulles
* &amp;lbrack ; UI&amp;rbrack ; Toutes les ressources du panneau Actifs sont mises en surbrillance au lancement
* Le chemin de navigation &amp;lbrack ; UI&amp;rbrack ; disparaît parfois dans le panneau Actifs lors de l’importation de matériaux
* &amp;lbrack ;UI&amp;rbrack ; Le changement de langue n’affecte pas le panneau Projet
* &amp;lbrack ; UI&amp;rbrack ; Le panneau Paramètres de canal affiche les informations de workflow héritées
* &amp;lbrack ; UI&amp;rbrack ; Aligner correctement le texte « Aucun paramètre pour cet élément » pour les filtres sans réglages dans le panneau des propriétés
* Les éléments &amp;lbrack ; UI&amp;rbrack ; sont mal alignés dans l’écran d’accueil et dans le menu contextuel des préférences
* Les titres du panneau &amp;lbrack ; UI&amp;rbrack ; ont une largeur incorrecte
* &amp;lbrack ; UI&amp;rbrack ; Le défilement est parfois interrompu dans le panneau Propriétés
* L&#39;écran de démarrage de l&#39;&amp;UI&amp;rbrack ; est flou et son rapport est incorrect
* &amp;lbrack ; UI&amp;rbrack ; Le mode plein écran n&#39;est pas plein écran
* Les panneaux &amp;lbrack ;UI&amp;rbrack ; non ancrés sont toujours au-dessus, même lorsque l’application n’est pas active dans MacOS
* &amp;lbrack ; UI&amp;rbrack ; Mettre à jour l&#39;image de bannière d&#39;écran d&#39;accueil
* Le filtre de Répétition &amp;lbrack ; Content&amp;rbrack ; ne traite pas le canal ambient occlusion
* &amp;lbrack ; Content&amp;rbrack ; Quilt Stitch problème avec la sélection du seam de l&#39;assemblage de courbure et le motif en losange
* Le filtre &amp;lbrack ;Content&amp;rbrack ; Embossage fonctionne en 256 px par 256 px
* &amp;lbrack ;Content&amp;rbrack ; Résoudre le problème de répétition avec les carreaux d&#39;Arrondi aux inférieurs lorsque le décalage est supérieur à 0

**Problèmes Connus :**

* &amp;lbrack ;Realtime Moteur 2021&amp;rbrack ; Heavy calcul, crash de l’application
* &amp;lbrack ;Realtime Moteur 2021&amp;rbrack ; Realtime Moteur 2021 effectuera le crash sur les ordinateurs Windows équipés à la fois du processeur AMD et du GPU Nvidia

### 3.0.0 Gaufre

*(Publié Le 23 Juin 2021)*

**Ajouté :**

* La Substance Alchemist &amp;lbrack ;Branding&amp;rbrack ; devient Adobe Substance 3D Sampler
* &amp;lbrack ;Branding&amp;rbrack ; Nouvelles icônes d&#39;application
* &amp;lbrack ; UI&amp;rbrack ; Nouvelle expérience utilisateur et interface utilisateur
* &amp;lbrack ; UI&amp;rbrack ; New Splashscreen
* Les panneaux &amp;lbrack ; UI&amp;rbrack ; ne peuvent pas être ancrés et peuvent être ancrés dans l&#39;interface
* &amp;lbrack ; UI&amp;rbrack ; Ancrez jusqu&#39;à 3 panneaux dans la même colonne
* &amp;lbrack ;UI&amp;rbrack ; Ancrez jusqu&#39;à 3 panneaux dans le même panneau (Tabulations)
* &amp;lbrack ; UI&amp;rbrack ; Désancrer les panneaux pour créer une fenêtre distincte dans le même écran ou dans un écran différent
* &amp;lbrack ; UI&amp;rbrack ; Le pop-up des panneaux fermés lorsque vous cliquez sur leurs icônes
* &amp;lbrack ; UI&amp;rbrack ; Réorganisez vos barres gauche et droite en déplaçant les icônes des panneaux
* &amp;lbrack ;UI&amp;rbrack ; Nouvelle barre d&#39;outils pour accéder directement à des filtres spécifiques (Recadrage, Transforme, Transforme de Perspective, Tampon de Clone)
* &amp;lbrack ; UI&amp;rbrack ; Nouveau bouton « Obtenir le contenu » dans la barre de gauche
* &amp;lbrack ; UI&amp;rbrack ; Importez des fichiers directement dans vos ressources avec le bouton Obtenir du contenu
* &amp;lbrack ; UI&amp;rbrack ; Importez des fichiers directement dans vos calques à l&#39;aide du bouton Obtenir du contenu
* &amp;lbrack ;UI&amp;rbrack ; Accédez directement au site Web Substance 3D Assets en Adobe à l&#39;aide du bouton Obtenir le contenu
* Le widget de résolution &amp;lbrack ; UI&amp;rbrack ; est désormais directement accessible dans le viewport
* &amp;lbrack ; UI&amp;rbrack ; Tous les éléments de l&#39;interface utilisateur sont désormais chargés dynamiquement
* &amp;lbrack ;UI&amp;rbrack ; Raccourci : utilisez « 2 » pour activer/désactiver la visibilité de la Vue 2D
* &amp;lbrack ;UI&amp;rbrack ; Raccourci : utilisez « 3 » pour activer/désactiver la visibilité de la vue 3D
* &amp;lbrack ; Écran d&#39;accueil&amp;rbrack ; Créez un projet en un clic avec le bouton Nouveau
* &amp;lbrack ; Écran d’accueil&amp;rbrack ; Nouvelle bannière d’illustration
* &amp;lbrack ; Project&amp;rbrack ; Tous les projets sont désormais associés à un fichier unique
* &amp;lbrack ;Project&amp;rbrack ; Nouvelle extension de fichier de projet .ssa
* &amp;lbrack ;Project&amp;rbrack ; Enregistrer en tant que projet vous demandera de sélectionner l&#39;emplacement où enregistrer votre projet
* &amp;lbrack ;Project&amp;rbrack ; La fermeture de Sampler vous demandera d&#39;enregistrer votre projet s&#39;il n&#39;est pas enregistré
* &amp;lbrack ;Project&amp;rbrack ; La fermeture de Sampler vous demandera d&#39;enregistrer votre projet si des modifications ont été apportées depuis le dernier enregistrement
* &lbrack;Project&amp;rbrack ; Le nom de votre projet est affiché au-dessus du viewport
* &lbrack;Project&amp;rbrack ; Le nom du projet est en italique avec une étoile s&#39;il n&#39;est pas enregistré ou s&#39;il contient des modifications depuis le dernier enregistrement
* &amp;lbrack ;Project&amp;rbrack ; Ouvrir un fichier de projet .ssa directement à partir de l&#39;explorateur du système d&#39;exploitation
* &amp;lbrack ;Project&amp;rbrack ; L&#39;ouverture d&#39;un fichier .sbsar depuis votre explorateur de système d&#39;exploitation lancera Sampler avec un nouveau projet doté de ce .fichier sbsar prêt à l&#39;emploi
* &amp;lbrack ;Project&amp;rbrack ; Ouvrez un fichier .alch (ancien fichier de Substance Alchemist) à partir de votre explorateur de système d&#39;exploitation
* &amp;lbrack ; Panneau Projet&amp;rbrack ; Nouveau panneau contenant tous les actifs créés dans un projet
* &amp;lbrack ; Panneau Projet&amp;rbrack ; Créer une ressource (matériau ou éclairage d&#39;environnement) à l’aide de l’icône +
* &amp;lbrack ; Panneau Projet&amp;rbrack ; Un clic droit sur la ressource ouvre un menu contextuel
* &amp;lbrack ; Panneau Projet&amp;rbrack ; À partir du menu contextuel accessible via un clic droit, vous pouvez supprimer une ressource
* &amp;lbrack ; Panneau Projet&amp;rbrack ; À partir du menu contextuel accessible via un clic droit, vous pouvez dupliquer une ressource
* &amp;lbrack ; Panneau Projet&amp;rbrack ; À partir du menu contextuel accessible via un clic droit, vous pouvez renommer une ressource
* &amp;lbrack ; Panneau Projet&amp;rbrack ; Le basculement entre les ressources ne perdra pas les modifications
* &amp;lbrack ; Resolution&amp;rbrack ; Vous pouvez désormais définir une résolution non carrée pour tous vos actifs
* &amp;lbrack ; Resolution&amp;rbrack ; La valeur de la résolution est enregistrée par ressource dans un projet
* &amp;lbrack ; Éclairage d&#39;environnement&amp;rbrack ; Créer un éclairage d&#39;environnement dans Substance 3D Sampler
* &amp;lbrack ; Éclairage d&#39;environnement&amp;rbrack ; Lors de la création d&#39;un éclairage d&#39;environnement, le glisser-déposer d&#39;images affichera la fenêtre Modèle de création d&#39;Éclairage d&#39;environnement
* &amp;lbrack ; Éclairage d&#39;environnement&amp;rbrack ; Dans le modèle de création d&#39;Éclairage d&#39;environnement, sélectionnez Importation d&#39;environnement pour attribuer votre image à l&#39;environnement dans la vue 3D
* &amp;lbrack ; Éclairage d&#39;environnement&amp;rbrack ; Dans le modèle de création d&#39;Éclairage d&#39;environnement, sélectionnez Fusion HDR pour créer un éclairage d&#39;environnement à partir de plusieurs images à 360 degrés avec une exposition différente
* &amp;lbrack ; Éclairage d&#39;environnement&amp;rbrack ; Dans le modèle de création d&#39;Éclairage d&#39;environnement, sélectionnez Utiliser comme bitmap pour modifier vos images avant de créer un éclairage d&#39;environnement
* &amp;lbrack ; Éclairage d&#39;environnement&amp;rbrack ; Affectez l&#39;utilisation de l&#39;environnement dans le calque d&#39;importation d&#39;image pour affecter directement l&#39;image à l&#39;environnement dans la vue 3D
* &amp;lbrack ; Éclairage d&#39;environnement&amp;rbrack ; Dans la Vue 2D de la couche d&#39;environnement, une correction automatique des couleurs est effectuée pour que le rendu soit identique à celui de la vue 3D
* &amp;lbrack ; Éclairage d&#39;environnement&amp;rbrack ; Nouveau contenu dédié à la création d&#39;éclairages d&#39;environnement
* &amp;lbrack ; Panneau Actifs&amp;rbrack ; Les panneaux Ressources et Filtres sont fusionnés dans un nouveau panneau Actifs
* &amp;lbrack ; Panneau Actifs&amp;rbrack ; Le panneau Actifs prend désormais en charge les types d’actifs suivants : matériaux, filtres et images
* &amp;lbrack ; Panneau des actifs&amp;rbrack ; Tous les actifs de démarrage sont accessibles dans la section Actifs de démarrage
* La section Actifs de &amp;brack ; du panneau Actifs est en lecture seule
* &amp;lbrack ; Panneau Actifs&amp;rbrack ; Nouvelle section « Vos actifs »
* &amp;lbrack ; La section Panneau Actifs&amp;rbrack ; « Vos actifs » est l&#39;endroit où vous pouvez importer toutes vos ressources
* &amp;lbrack ; Panneau Actifs&amp;rbrack ; Tous les actifs de « Vos actifs » sont ajoutés dans un dossier spécifique de vos documents
* &amp;lbrack ; Assets Panel&amp;rbrack ; Connecter les dossiers locaux dans le panneau Actifs pour ajouter de nouvelles sections
* &amp;lbrack ; Assets Panel&amp;rbrack ; La recherche portera sur le dossier actuel et ses sous-dossiers
* &amp;lbrack ; Panneau Actifs&amp;rbrack ; Naviguer entre les dossiers et les sous-dossiers avec les chemins de navigation
* &amp;lbrack ; Assets Panel&amp;rbrack ; Filtre le dossier actif par matériau, par filtre ou par image
* &amp;lbrack ; Assets Panel&amp;rbrack ; Combine plusieurs filtres pour obtenir uniquement des matériaux et des images
* &amp;lbrack ; Panneau Actifs&amp;rbrack ; Changez l&#39;affichage en basculant entre une grille ou une liste
* &amp;lbrack ; Les filtres du panneau Actifs sont représentés par leur icône
* &amp;lbrack ; Le panneau Actifs&amp;rbrack ; Les images sont représentées avec leur aperçu
* &amp;lbrack ; Assets Panel&amp;rbrack ; L&#39;augmentation de la largeur modifiera la disposition du panneau avec une vue spécifique pour naviguer entre les dossiers
* &amp;lbrack ; Panneau Actifs&amp;rbrack ; Dans les sections non en lecture seule, supprimez un actif en le faisant glisser sur l’icône du chutier
* &amp;lbrack ; Panneau Actifs&amp;rbrack ; Un clic droit sur l’actif ouvre un menu contextuel
* &amp;lbrack ; Panneau Actifs&amp;rbrack ; Dans le menu contextuel accessible via un clic droit, accédez aux métadonnées de l&#39;actif (nom, catégorie, emplacement)
* &amp;lbrack ; Panneau Actifs&amp;rbrack ; Dans le menu contextuel accessible via un clic droit, supprimez l&#39;actif (disponible uniquement dans les sections non en lecture seule)
* &amp;lbrack ; Panneau Actifs&amp;rbrack ; Dans le menu contextuel accessible via un clic droit, parcourez votre actif dans Adobe Bridge
* &amp;lbrack ; Panneau Calques&amp;rbrack ; Nouvelle icône pour ajouter directement un matériau de base sur vos calques
* &amp;lbrack ; Layers Panel&amp;rbrack ; Raccourci - Maj + B ajoutera un matériau de base au-dessus de vos calques
* &amp;lbrack ; Panneau Calques&amp;rbrack ; Les calques disposent désormais d&#39;une prévisualisation par vignettes (miniature de Matériau, icône de filtre ou aperçu d&#39;image)
* &amp;lbrack ; Panneau Propriétés&amp;rbrack ; Nouvelle conception du titre du panneau Propriétés avec le nom et la vignette de l&#39;actif
* &amp;lbrack ; Panneau Propriétés&amp;rbrack ; Les calques de filtre prennent désormais en charge les paramètres prédéfinis
* Panneau Propriétés &amp;lbrack ; Sur le calque d&#39;importation d&#39;image, cliquez avec le bouton droit sur l&#39;aperçu de l&#39;image pour modifier l&#39;image dans Photoshop
* &amp;lbrack ; Adobe Bridge&amp;rbrack ; Parcourir votre ressource dans Adobe Bridge, lance Bridge à l&#39;emplacement de la ressource
* &amp;lbrack ; Adobe Photoshop&amp;rbrack ; Edit in Adobe Photoshop ouvrira l&#39;image dans Photoshop pour la modifier
* &amp;lbrack ;Adobe Photoshop&amp;rbrack ; À chaque enregistrement dans Adobe Photoshop, l&#39;image modifiée sera rechargée dans Sampler
* &amp;lbrack ;Substance 3D Designer&amp;rbrack ; Les ressources envoyées depuis Adobe Substance 3D Designer arriveront directement dans la section « Vos ressources » du panneau Ressources
* &amp;lbrack ; Export&amp;rbrack ; Envoyer des ressources directement à Adobe Substance 3D Painter et Adobe Substance 3D Stager
* &amp;lbrack ; Export&amp;rbrack ; Envoyer des matériaux et des éclairages d&#39;environnement à Adobe Substance 3D Painter
* &amp;lbrack ; Export&amp;rbrack ; Envoyer des éclairages d&#39;environnement à Adobe Substance 3D Stager
* &amp;lbrack ;Rendering&amp;rbrack ; Les nouvelles propriétés de matériau sont désormais prises en charge et rendues en 3D
* &amp;lbrack ; Rendu&amp;rbrack ; Prise en charge de l&#39;Éclat (Couleur de l&#39;éclat, opacité de l&#39;Éclat et rugosité de l&#39;Éclat)
* &amp;lbrack ; Rendering&amp;rbrack ; Ajout de la prise en charge du revêtement (Coat color, Coat roughness, Coat normal, Coat specular level et IOR du revêtement)
* &amp;lbrack ; Rendu&amp;rbrack ; Ajout de la prise en charge de l&#39;Anisotropie (Anisotropy level et Anisotropy angle)
* &amp;lbrack ; Rendu&amp;rbrack ; Ajout de la prise en charge du Specular edge color
* &amp;lbrack ; Rendering&amp;rbrack ; Activez ces nouvelles propriétés dans le panneau Paramètres de couche
* &amp;lbrack ;Rendering&amp;rbrack ; Introduction d’un nouveau moteur de rendu Realtime Moteur (2021) en version Beta
* &amp;lbrack ; Rendering&amp;rbrack ; Basculez entre les deux versions de rendu dans le panneau Paramètres du visualiseur
* &amp;lbrack ;Rendering&amp;rbrack ; Le moteur de rendu Realtime Moteur (2021) prend en charge les propriétés de matériau de translucency, d&#39;absorption et de diffusion
* &amp;lbrack ;Rendering&amp;rbrack ; Le moteur de rendu Realtime Moteur (2021) introduit une nouvelle façon de calculer les ombres à partir de l&#39;éclairage d&#39;environnement
* &amp;lbrack ;Rendering&amp;rbrack ; Le moteur de rendu Realtime Moteur (2021) calcule en temps réel l&#39;irradiance de l&#39;éclairage d&#39;environnement
* &amp;lbrack ; Panneau Paramètres de Shader&amp;rbrack ; Nouveau panneau Paramètres de Shader pour modifier des paramètres de shader de matériau spécifiques
* &amp;lbrack ; Shader Settings Panel&amp;rbrack ; New parameters (Échelle normale, Échelle de l&#39;height, niveau de l&#39;height, Intensité des émissions, IOR, Intensité du Coat normal et IOR du pelage)
* &amp;lbrack ; Panneau Paramètres de Shader&amp;rbrack ; Paramètres spécifiques pour le Moteur en temps réel 2021 (Subsurface scattering, Distance de diffusion, Décalage rouge et Diffusion Rayleigh)
* &amp;lbrack ; Panneau des paramètres de Shader&amp;rbrack ; Les valeurs des paramètres sont enregistrées par ressource
* &amp;lbrack ; Panneau Paramètres du visualiseur&amp;rbrack ; Ajout d&#39;un aperçu des éclairages d&#39;environnement par défaut
* &amp;lbrack ; Panneau Paramètres du visualiseur&amp;rbrack ; Ajout d&#39;un aperçu des maillages par défaut
* &amp;lbrack ; Panneau Paramètres du visualiseur&amp;rbrack ; Nouveau paramètre d&#39;opacité d&#39;environnement
* &amp;lbrack ; Panneau Paramètres du visualiseur&amp;rbrack ; Nouveau paramètre de flou d’environnement (spécifique au moteur de rendu Realtime Moteur 2021)
* &amp;lbrack ; Localization&amp;rbrack ; Nouvelles traductions en allemand et en français
* &amp;lbrack ;Content&amp;rbrack ; Nouveaux matériaux de démarrage par défaut
* &amp;lbrack ;Content&amp;rbrack ; Nouveaux éclairages d&#39;environnement par défaut
* &amp;lbrack ; Content&amp;rbrack ; Tous les filtres ont été mis à jour, nettoyés et optimisés
* &amp;lbrack ; Content&amp;rbrack ; Le filtre de réglage a été divisé en plusieurs filtres
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre Luminosité/Contraste
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre Teinte/Saturation
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre Vibrance
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre Netteté
* &amp;lbrack ;Content&amp;rbrack ; Nouveau réglage Normal/Height
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre Panneaux
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre Doigt
* Filtre &amp;lbrack ; Content&amp;rbrack ; New Weaves
* &amp;lbrack ;Content&amp;rbrack ; Nouveau filtre de transforme de déformation
* &amp;lbrack ;Content&amp;rbrack ; Nouvel Height au filtre AO
* &amp;lbrack ;Content&amp;rbrack ; Nouvel Height au filtre normal
* &amp;lbrack ;Content&amp;rbrack ; Color Replace - Remplace dans les nouveaux canaux pris en charge (Éclat, Revêtement, Anisotropie,...)
* &amp;brack ; Content&amp;rbrack ; Color variation - Mode manuel pour sélectionner exactement les couleurs à modifier
* &amp;lbrack ;Content&amp;rbrack ; Répétition - option pour visualiser les seams coupés
* &amp;lbrack ;Content&amp;rbrack ; Répétition : option permettant de mettre en peinture les seams coupés pour une répétition parfaite
* &amp;lbrack ;Content&amp;rbrack ; Match - option permettant d&#39;ajouter un matériau correspondant à sa couleur et à sa rugosité
* &amp;lbrack ; Content&amp;rbrack ; Match : fonctionne désormais sur les images pour correspondre à la couleur d’une autre image
* &amp;lbrack ; Content&amp;rbrack ; Environment light - Nouveau filtre Température de couleur
* &amp;lbrack ; Content&amp;rbrack ; Environment light - Nouveau filtre Exposition
* &amp;lbrack ; Content&amp;rbrack ; Environment light - Nouveau filtre Aperçu de l&#39;exposition
* &amp;lbrack ;Content&amp;rbrack ; Environment light - Nouveau filtre de Nadir patch
* &amp;lbrack ;Content&amp;rbrack ; Environment light - Nouveau filtre de Nadir extract
* &amp;lbrack ; Content&amp;rbrack ; Environment light - Nouveaux filtres d&#39;éclairage (Sphère, Trait, Forme, Plan)
* &amp;lbrack ; Content&amp;rbrack ; Environment light - Nouveau filtre Correctif de panorama
* &amp;lbrack ; Content&amp;rbrack ; Environment light - Nouveau filtre Redresser l’horizon
* &amp;lbrack ;Content&amp;rbrack ; Environment light - Nouveau filtre de fusion HDR

**Problèmes Connus :**

* &amp;lbrack ;Realtime Moteur 2021&amp;rbrack ; Modification de la mise en page, crash de l’application
* &amp;lbrack ;Realtime Moteur 2021&amp;rbrack ; Heavy calcul, crash de l’application
* &amp;lbrack ; Panneaux&amp;rbrack ; MacOS : les panneaux non ancrés sont placés devant toutes les applications
* Les widgets de Transforme et de position de &amp;lbrack ;Widgets&amp;rbrack ; peuvent disparaître. Masquez et affichez le calque pour les faire apparaître.
* &amp;lbrack ; Export&amp;rbrack ; L&#39;exportation SBSAR d&#39;un éclairage d&#39;environnement perd la précision de 32 nombres de bits par pixel
* &amp;lbrack ; Panneau des actifs&amp;rbrack ; Les actifs peuvent être mis en surbrillance lors de l&#39;ouverture d&#39;un dossier
* &amp;lbrack ; Panneau Propriétés&amp;rbrack ; La réinitialisation des paramètres ne réinitialise pas l&#39;interface utilisateur de la zone de liste déroulante
* &amp;lbrack ;Localization&amp;rbrack ; Le changement de langue n&#39;affecte pas le panneau de projet tant qu&#39;il n&#39;est pas recréé

## Version 2

### 2.3.2 (2020.3.2) Vermicelli

*(Publié Le 23 Février 2021)*

**Ajouté :**

* &amp;lbrack ; Prise en charge de Localization&amp;rbrack ; en japonais

**Fixe :**

* &amp;lbrack ; Layers&amp;rbrack ; Le réglage d&#39;un matériau dans le filtre de broderie perd l&#39;image de la broderie

**Problèmes Connus :**

* L’utilisation de la fonctionnalité Image vers Matériau (optimisée par l’IA) sur les images haute résolution peut être lente
* Les filtres Fond basé sur le contenu sont lents en haute résolution
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Impossible d’enregistrer deux fois exactement la même pile de calques de matériau

### 2.3.1 (2020.3.1) Vermicelli

*(Publié Le 17 Décembre 2020)*

**Ajouté :**

* &amp;lbrack ; Moteur&amp;rbrack ; mise à jour de la Substance Engine
* &amp;lbrack ; Application&amp;rbrack ; Variable d&#39;environnement pour désactiver des fonctionnalités spécifiques
* &amp;lbrack ; Content&amp;rbrack ; Remplacer la couleur - Nouvelle option de segmentation avancée
* &amp;lbrack ;Content&amp;rbrack ; Arrondi aux inférieurs Tiles : nouveaux motifs et options disponibles
* &amp;lbrack ; Content&amp;rbrack ; Broderie - Réorganisation complète du filtre
* &amp;lbrack ;Content&amp;rbrack ; Adjustment - Nouveau paramètre métallique + correction du transforme d&#39;opacité sécurisée

**Fixe :**

* &amp;lbrack ; Layers&amp;rbrack ; Impossible d&#39;importer deux fois le même filtre personnalisé
* &amp;lbrack ; Layers&amp;rbrack ; Impossible d&#39;utiliser l&#39;entrée d&#39;image avec l&#39;outil Pinceau
* &amp;lbrack ; Export&amp;rbrack ; Export .jpg au lieu de .jpeg
* &amp;lbrack ; UI&amp;rbrack ; Mettre à jour les crédits d&#39;image de l&#39;écran d&#39;accueil
* &amp;lbrack ; UI&amp;rbrack ; Réparer le séparateur invisible dans les menus
* Les boutons radio &amp;lbrack ; UI&amp;rbrack ; affichent une info-bulle lorsqu&#39;ils sont tronqués
* &amp;lbrack ; UI&amp;rbrack ; Typo : Matériaux pour démarrer
* Les caractères &amp;lbrack ;Application&amp;rbrack ; UTF-8 dans les noms de fichier ne fonctionnent pas
* &amp;lbrack ; Localization&amp;rbrack ; Disable italic font style for chinese locale
* &amp;lbrack ; Localization&amp;rbrack ; Chaîne localisée divisée en 2 lignes
* &amp;lbrack ; Localization&amp;rbrack ; Ajuster le nom du dossier et le remplacer par des points de suspension s&#39;il est trop long
* &amp;lbrack ; Localization&amp;rbrack ; Format des nombres avec séparateur des milliers
* &amp;lbrack ; Localization&amp;rbrack ; Localiser l&#39;affichage de la date et de l&#39;heure
* &amp;lbrack ; Localization&amp;rbrack ; Localize color picker sous Windows
* &amp;lbrack ;Content&amp;rbrack ; Transforme : lorsque la transformation sécurisée est activée, la normale pivote correctement tous les 45°
* &amp;lbrack ; Content&amp;rbrack ; Surface relief - Résoudre le problème de répétition avec le bruit fractal perlin (bruit avancé)
* &amp;lbrack ;Content&amp;rbrack ; Brickwall Pattern - Entrée Height en 16 bits
* &amp;lbrack ; Content&amp;rbrack ; Matériau Icon Render - problème de reflets de Specular
* &amp;lbrack ; Content&amp;rbrack ; Color Variation : pas de changement de couleur entre les entrées de couleur et le résultat
* &amp;lbrack ; Content&amp;rbrack ; Color Variation - Mise à jour des performances

**Problèmes Connus :**

* L’utilisation de la fonctionnalité Image vers Matériau (optimisée par l’IA) sur les images haute résolution peut être lente
* Les filtres Fond basé sur le contenu sont lents en haute résolution
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Impossible d’enregistrer deux fois exactement la même pile de calques de matériau

### 2.3.0 (2020.3.0) Vermicelli

*(Publié Le 26 Octobre 2020)*

**Ajouté :**

* &amp;lbrack ; Image vers Matériau&amp;rbrack ; Prise en charge de la série NVIDIA RTX 3000
* &amp;lbrack ; Image à Matériau&amp;rbrack ; Nouveaux paramètres pour contrôler les détails de la géométrie
* &amp;lbrack ; Image à Matériau&amp;rbrack ; Nouveaux paramètres pour contrôler la rugosité
* &amp;lbrack ; Image à Matériau&amp;rbrack ; Nouveaux paramètres pour contrôler l&#39;intensité du plaisir
* &amp;lbrack ; Thumbnails&amp;rbrack ; Nouveau générateur de vignettes basé sur le rendu PBR de la Substance Designer
* &amp;lbrack ; Thumbnails&amp;rbrack ; Mettre à jour les matériaux de base et les atlas pour incorporer leur miniature
* &lbrack;Thumbnails&amp;rbrack ; Récupérez la vignette du fichier .fichier sbsar si elle existe
* &amp;lbrack ; Thumbnails&amp;rbrack ; Modifier la qualité des vignettes dans les Préférences
* &amp;lbrack ; Moteur&amp;rbrack ; Mise à jour vers la version 8 de la Substance Engine
* &amp;lbrack ; Localization&amp;rbrack ; Chinese localization
* &amp;lbrack ;UI&amp;rbrack ; Sélecteur de nuanciers expérimental
* &amp;lbrack ;Content&amp;rbrack ; New Map d&#39;environnement - Studio 06
* &amp;lbrack ; Content&amp;rbrack ; Ajouter un filtre Atlas Generator
* &amp;lbrack ; Content&amp;rbrack ; Add Atlas splitter filter
* &amp;lbrack ; Content&amp;rbrack ; Add Discarded Gums filter
* &amp;lbrack ; Content&amp;rbrack ; Add Fingerprints filter
* &amp;lbrack ; Content&amp;rbrack ; Add Scratches filter
* &amp;lbrack ;Content&amp;rbrack ; Ajouter un filtre Surface Relief (remplacer le filtre de modulation d&#39;height)
* &amp;lbrack ; Content&amp;rbrack ; Ajouter un filtre de déformation
* &amp;lbrack ; Content&amp;rbrack ; Ajouter un filtre Inverser
* &amp;lbrack ; Content&amp;rbrack ; Ajouter un filtre Coloriser
* &amp;lbrack ; Content&amp;rbrack ; Add Replace Color Filters
* &amp;lbrack ;Content&amp;rbrack ; Transformer : ajouter la possibilité de désactiver la transformation sur un canal spécifique
* &lbrack;Content&amp;rbrack ; Transforme : ajouter une rotation lorsque le transforme sécurisé est activé
* &amp;lbrack ; Content&amp;rbrack ; Color Variation : ajoutez une option de segmentation pour choisir comment distribuer les couleurs

**Fixe :**

* &amp;lbrack ; Layers&amp;rbrack ; Mettez correctement à jour l&#39;interface utilisateur lorsque vous effectuez plusieurs actions d&#39;annulation/de rétablissement
* &amp;lbrack ; Layers&amp;rbrack ; Empêcher les crashs lors de plusieurs actions Annuler/Rétablir
* &amp;lbrack ; Layers&amp;rbrack ; Crash lors de l&#39;utilisation de Image vers Matériau (optimisé par l&#39;IA), avec log : ordinal de périphérique non valide
* &amp;lbrack ; Filters&amp;rbrack ; Améliorer la détection des cartes graphiques NVIDIA pour les fonctionnalités spécifiques à NVidia
* &lbrack;Application&amp;rbrack ; Crash lors de la fermeture de l&#39;application
* &amp;lbrack ;Application&amp;rbrack ; Correction de la détection de la quantité de VRAM sur MacOS
* &amp;lbrack ; Export&amp;rbrack ; Certains paramètres prédéfinis d&#39;exportation sont parfois manquants
* &amp;lbrack ; Content&amp;rbrack ; Effet Peinture à l&#39;huile - Correction de la plage d&#39;heights avec une amplitude de displacement élevée
* &amp;lbrack ; Content&amp;rbrack ; Make It Tile Avancé - Aucune couleur de base délavée à l&#39;exportation
* &amp;lbrack ; Content&amp;rbrack ; Make It Tile Advanced : Masque blanc sur la couleur de base lorsque l&#39;AO est trop fort
* &amp;lbrack ;Content&amp;rbrack ; Adjustment : fonctionne désormais sur les images (scan1, ...)

**Problèmes Connus :**

* L’utilisation de la fonctionnalité Image vers Matériau (optimisée par l’IA) sur les images haute résolution peut être lente
* Les filtres Fond basé sur le contenu sont lents en haute résolution
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Impossible d’enregistrer deux fois exactement la même pile de calques de matériau

### 2.2.1 (2020.2.1) Udon

*(Publié Le 21 Juillet 2020)*

**Ajouté :**

* &amp;lbrack ; Layers&amp;rbrack ; In App Error message when Image to Matériau (Optimisé par l&#39;IA) is out of memory

**Fixe :**

* &amp;lbrack ; Layers&amp;rbrack ; Image to Matériau (optimisé par l’IA) ne fonctionne pas avec les workflows Specular/Brillance
* &amp;lbrack ; Layers&amp;rbrack ; effectue des Crashs lorsqu&#39;il n&#39;y a pas assez de mémoire vidéo lors de l&#39;utilisation de Image to Matériau (optimisé par l&#39;IA)
* &amp;lbrack ; Layers&amp;rbrack ; Le cache de disque n&#39;est pas utilisé pour l&#39;affichage lors de l&#39;ouverture d&#39;une pile
* &amp;lbrack ; Layers&amp;rbrack ; Detection of Nvidia RTX 8000
* &amp;lbrack ; Layers&amp;rbrack ; Il est parfois impossible de déplacer un calque en dehors d&#39;une entrée Éclaboussure
* &amp;lbrack ; Layers&amp;rbrack ; Le cache de disque n&#39;est pas utilisé lors de l&#39;insertion d&#39;une pile dans une pile
* &amp;lbrack ; Layers&amp;rbrack ; Certaines utilisations de couches sont calculées bien qu&#39;elles ne soient pas utilisées
* Des sorties &amp;lbrack ; Layers&amp;rbrack ; Blank sont parfois créées lors de l&#39;importation d&#39;images
* &amp;lbrack ; vue 2D&amp;rbrack ; Passer à un autre calque avec le mode Dessin activé bloque le panoramique et le zoom
* &amp;lbrack ;Content&amp;rbrack ; Snow - problème 8 bits sur la map normal
* &amp;lbrack ;Content&amp;rbrack ; Pavement : problème de 8 bits sur la map normal
* &amp;lbrack ;Content&amp;rbrack ; Equalizer - Problème de 8 bits sur la map normal
* &amp;lbrack ;Content&amp;rbrack ; Gravel Generator - problème de 8 bits sur la map normal
* &amp;lbrack ; Content&amp;rbrack ; Arrondi aux inférieurs Tiles - Opacité et specular level de la poignée
* &amp;lbrack ; Content&amp;rbrack ; Blender cycles eeve export preset - inverser la map normal
* &amp;lbrack ; Content&amp;rbrack ; Correction du problème des images volumineuses avec Image vers Matériau (optimisé par l’IA)
* crash &lbrack;Application&rbrack; lors de la sélection de « Sauvegarder et redémarrer » sur erreur de base de données
* crash de &amp;lbrack ;Application&amp;rbrack ; lorsque vous cliquez rapidement sur la même ressource
* &amp;lbrack ; Application&amp;rbrack ; crashs rares en sortie
* crash de &amp;lbrack ;Application&amp;rbrack ; lors de l&#39;abandon de fichiers sur l&#39;écran d&#39;accueil
* &amp;lbrack ;Application&amp;rbrack ; Crash lorsqu&#39;un fichier d&#39;environnement corrompu est chargé
* &amp;lbrack ; Application&amp;rbrack ; Rare crash lors du basculement rapide du fichier de rendu
* &amp;lbrack ; Application&amp;rbrack ; Se bloque lors de la fermeture pendant le calcul d&#39;une ressource
* &amp;lbrack ;Application&amp;rbrack ; Rare crash au démarrage sous macos
* &lbrack;Application&amp;rbrack ; bloqué lors de la fermeture de l&#39;application peu après le démarrage
* &amp;lbrack ;Rendu&amp;rbrack ; La vue 3D scintille parfois
* Le sélecteur de couleurs et les widgets de générateur aléatoire de l’&amp;ibrack ;UI&amp;rbrack ; ne sont pas alignés avec le reste des réglages
* &amp;lbrack ;Rendu&amp;rbrack ; Affichage d&#39;un temps de calcul incorrect
* &amp;lbrack ; Export&amp;rbrack ; Certains paramètres prédéfinis d&#39;exportation sont parfois manquants

**Problèmes Connus :**

* L’utilisation de la fonctionnalité Image vers Matériau (optimisée par l’IA) sur les images haute résolution peut être lente
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Les filtres Fond basé sur le contenu sont lents en haute résolution
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Impossible d’enregistrer deux fois exactement la même pile de calques de matériau

### 2.2.0 (2020.2.0) Udon

*(Publié Le 15 Juin 2020)*

**Ajouté :**

* &amp;lbrack ;Create&amp;rbrack ; Nouveau filtre Image vers Matériau (alimenté par l&#39;IA) disponible sous Windows et Linux
* &amp;lbrack ;Create&amp;rbrack ; Rename Bitmap to Matériau to Image to Matériau (B2M)
* &amp;lbrack ; Fenêtre contextuelle Importer une image&amp;rbrack ; Nouveau modèle de création de Matériau
* &amp;lbrack ; Image Import&amp;rbrack ; Nouvelle option « Ajouter un matériau de base »
* &amp;lbrack ; Image Import&amp;rbrack ; Pouvoir faire glisser et déposer des images supplémentaires dans le modèle de création de Matériau
* &amp;lbrack ; Image Import&amp;rbrack ; Pouvoir supprimer des images dans le modèle de création de Matériau
* &amp;lbrack ; Importation d&#39;images&amp;rbrack ; Attribuer automatiquement un canal aux bitmaps importés en fonction de leur nom de fichier
* &amp;lbrack ; Image Import&amp;rbrack ; Être capable d&#39;inverser les maps normal
* &amp;lbrack ; vue 2D&amp;rbrack ; Introduction d&#39;un mode peinture
* &amp;lbrack ; vue 2D&amp;rbrack ; Les mosaïques de peinture
* &amp;lbrack ; vue 2D&amp;rbrack ; Définissez une valeur de niveaux de gris pour la couleur du pinceau
* &amp;lbrack ; vue 2D&amp;rbrack ; Panoramique et zoom pendant la peinture
* &amp;lbrack ; vue 2D&amp;rbrack ; X raccourci pour inverser la valeur des niveaux de gris du pinceau
* les raccourcis &amp;lbrack ; vue 2D&amp;rbrack ; &amp;lbrack ; et &amp;rbrack ; pour modifier l&#39;épaisseur du pinceau
* &amp;lbrack ; vue 2D&amp;rbrack ; Ctrl (ou Cmd) + Molette de la souris pour modifier l’épaisseur du pinceau
* &amp;lbrack ; vue 2D&amp;rbrack ; Il est désormais possible de modifier la position de la source lors de l&#39;utilisation de Clone Patch
* &amp;lbrack ; Layers&amp;rbrack ; Maj + glisser-déposer pour créer des atlas de dispersion automatique
* &amp;lbrack ; Layers&amp;rbrack ; Alt + glisser-déposer insère un matériau en tant que décalcomanie
* &amp;lbrack ; Layers&amp;rbrack ; Exposer facilement les matrices de transformation de la Substance Designer
* &amp;lbrack ; Calques&amp;rbrack ; La suppression de textures dans une pile non vide affecte automatiquement les couches correctes
* &amp;lbrack ; Layers&amp;rbrack ; Nouveau type de calque : Filtres composés
* &amp;lbrack ; Parameters&amp;rbrack ; prend en charge les entrées de chaîne de Substance
* &amp;lbrack ; UI&amp;rbrack ; Ajout d’ombres portées pour les fenêtres contextuelles et les menus
* &amp;lbrack ; UI&amp;rbrack ; Nouveau widget de couleur avec options de clic droit (effacer, copier, coller)
* &amp;lbrack ; UI&amp;rbrack ; Nouveau widget d&#39;image avec l&#39;option de l&#39;outil de peinture
* &amp;lbrack ;UI&amp;rbrack ; Possibilité de passer la peinture sur une image importée dans un widget d&#39;image
* &amp;lbrack ; Rendu&amp;rbrack ; Nouvelle position de caméra par défaut
* Les fichiers de Substance &amp;lbrack ;Export&amp;rbrack ; sont exportés pour la Substance Designer 2020.1.2 (10.1.2)
* &amp;lbrack ; Performance&amp;rbrack ; Meilleur temps de démarrage de l&#39;application
* &amp;lbrack ; Performance&amp;rbrack ; Améliorer la gestion des tâches asynchrones
* &amp;lbrack ; Performance&amp;rbrack ; Améliorer les performances de la pile de calques lors de l&#39;ajout, de la suppression ou du déplacement de calques
* &amp;lbrack ; Performance&amp;rbrack ; Image vers Matériau (optimisé par l&#39;IA) s&#39;exécute plus rapidement sur les GPU RTX
* &amp;lbrack ;Content&amp;rbrack ; Nouveaux maillages : T-Shirt Femme, T-Shirt Homme, Chaussure
* &amp;lbrack ;Content&amp;rbrack ; Nouveau mode de Fusion - Par Fusion de canal
* &amp;lbrack ; Content&amp;rbrack ; Opacité fusionner la correction d&#39;height avec 2 nouveaux paramètres (position de l&#39;height et échelle de l&#39;height)
* &amp;lbrack ; Content&amp;rbrack ; Ajouter des réglages d&#39;Height en mode Fusion d&#39;Height
* &amp;lbrack ; Content&amp;rbrack ; Utiliser l&#39;option d&#39;informations sur l&#39;Height dans la Fusion de masque personnalisée
* &amp;lbrack ; Content&amp;rbrack ; Nouvel outil de correction de Perspective
* &amp;lbrack ; Content&amp;rbrack ; Pattern Generator : ajoutez un paramètre pour inverser le motif
* &amp;lbrack ;Content&amp;rbrack ; Pattern Generator - Ajouter un nouveau paramètre Remplacer les détails de Matériau
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre de décalcomanie
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre de mousse
* &amp;lbrack ;Content&amp;rbrack ; Nouveau filtre de Fissures
* &amp;lbrack ;Content&amp;rbrack ; Nouveau filtre Validation PBR
* &amp;lbrack ;Content&amp;rbrack ; Nouveau filtre Carreaux d&#39;Arrondi aux inférieurs
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre Quilt Stich
* &amp;lbrack ;Content&amp;rbrack ; Atlas scatter : ajouter une entrée de masque personnalisée pour activer l’option de peinture
* &amp;lbrack ;Content&amp;rbrack ; Dirt : ajouter une entrée de masque personnalisée pour activer l’option de peinture
* &amp;lbrack ; Content&amp;rbrack ; paramètre prédéfini d’exportation CLO
* &amp;lbrack ; Content&amp;rbrack ; VStitcher : paramètre prédéfini d’exportation
* Les paramètres prédéfinis &amp;lbrack ; Content&amp;rbrack ; Unity HDRP exportent un detailMap

**Fixe :**

* Les images &amp;lbrack ; importées des calques sont chargées trop de fois
* &amp;lbrack ; Layers&amp;rbrack ; Crash lors de la création d&#39;un patch de duplication au bas de la pile
* &amp;lbrack ; Layers&amp;rbrack ; L&#39;ajout d&#39;un matériau au bas de la pile la rend instable
* Le filtre &amp;lbrack ; Layers&amp;rbrack ; après l&#39;importation d&#39;images ne fonctionne pas correctement
* La valeur de type de flux de travail &amp;lbrack ; Layers&amp;rbrack ; n&#39;est pas mise à jour lors du basculement du flux de travail entre les projets avec un filtre personnalisé
* &amp;lbrack ; Layers&amp;rbrack ; Désactiver le bouton « Supprimer le calque » lorsqu&#39;aucun calque n&#39;est sélectionné
* &amp;lbrack ; Layers&amp;rbrack ; Crash lors du chargement d&#39;une ressource contenant un patch de Clone
* &amp;lbrack ; Layers&amp;rbrack ; Normal aux crashs de filtre Heights sous MacOs
* crash &lbrack;Application&amp;rbrack ; lors du chargement des maps d&#39;environnement aller-retour
* &amp;lbrack ;Application&amp;rbrack ; Problèmes de performances lorsque le pilote de la tablette graphique est installé
* &amp;lbrack ;Application&amp;rbrack ; Les fichiers EXR 32 bits importés sont noirs
* crashs de &amp;lbrack ;Application&amp;rbrack ; lors du chargement et du déchargement d&#39;actifs
* &lbrack;Application&amp;rbrack ; Crash lors du passage de l&#39;exploration à la création
* &amp;lbrack ;Application&amp;rbrack ; La collection cible lors de l&#39;enregistrement d&#39;un matériau ne provient pas du projet en cours
* &amp;lbrack ; Application&amp;rbrack ; Corriger la sauvegarde et le redémarrage
* &amp;lbrack ;Image Import&amp;rbrack ; Importer correctement les images en niveaux de gris
* &amp;lbrack ; Content&amp;rbrack ; Nouveaux filtres pour la gestion des nouvelles matrices
* &amp;lbrack ; Content&amp;rbrack ; Les filtres personnalisés importés sont visibles dans la barre d&#39;accès rapide
* &amp;lbrack ; Content&amp;rbrack ; Corriger le changement de couleur avec le filtre avancé Créer une mosaïque
* &amp;lbrack ; Performance&amp;rbrack ; L&#39;ouverture d&#39;une boîte de dialogue de couleur est lente et recalcule le calque actuel
* Les raccourcis clavier de &amp;lbrack ; UI&amp;rbrack ; ne fonctionnent pas toujours
* &amp;lbrack ; vue 2D&amp;rbrack ; Content Aware Fill a besoin d&#39;un premier clic inutile pour fonctionner
* Les dossiers &amp;lbrack ; Resources&amp;rbrack ; des disques locaux sont toujours surveillés pour les mises à jour après les avoir supprimés
* &amp;lbrack ; Resources&amp;rbrack ; La suppression d&#39;un dossier lié du système de fichiers ne le supprime pas
* &amp;lbrack ; Export&amp;rbrack ; Les utilisations personnalisées dans les paramètres prédéfinis d&#39;exportation personnalisés ne sont pas exportées
* &amp;lbrack ; Export&amp;rbrack ; L&#39;exportation du fichier .fichier sbsar avec des caractères spéciaux dans le chemin échoue

**Problèmes Connus :**

* Les recalculs répétitifs de Image en Matériau (optimisés par l’IA) peuvent déclencher un crash (mémoire insuffisante)
* Les recalculs répétitifs du Delighter peuvent déclencher un crash (mémoire insuffisante)
* L’utilisation de la fonctionnalité Image vers Matériau (optimisée par l’IA) sur les images haute résolution peut être lente
* L’utilisation de la fonctionnalité Image vers Matériau (optimisée par l’IA) sur un GPU avec un VRAM faible peut déclencher un crash (mémoire insuffisante)
* L’image vers le Matériau (optimisée par l’IA) n’est pas disponible sur PBR Specular/Brillance
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Les filtres Fond basé sur le contenu sont lents en haute résolution
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Impossible d’enregistrer deux fois exactement la même pile de calques de matériau

### 2.1.1 (2020.1.1) Tiramisu

*(Publié Le 1Er Avril 2020)*

**Ajouté :**

* &amp;lbrack ; Project&amp;rbrack ; Exporter et importer des métadonnées
* &amp;lbrack ; Application&amp;rbrack ; Ctrl+S enregistre désormais un paramètre prédéfini dans Explorer
* &amp;lbrack ; Performance&amp;rbrack ; Utilisez le cache de rendu au lieu de recalculer les matériaux enregistrés pour des résolutions allant jusqu&#39;à 2k

**Fixe :**

* &amp;lbrack ; UI&amp;rbrack ; Indicateur de calcul fixe dans le viewport
* &amp;lbrack ; UI&amp;rbrack ; La saisie de valeurs négatives dans les curseurs est corrigée
* &amp;lbrack ; UI&amp;rbrack ; Zones de liste déroulante : les flèches du clavier et la barre de défilement fonctionnent désormais
* &amp;lbrack ; UI&amp;rbrack ; Conserver le canal sélectionné lors du basculement entre les « Sorties Matériau » et les « Entrées calque » dans la Vue 2D
* &amp;lbrack ; Layers&amp;rbrack ; crash fixe lors de l&#39;ajout de couches personnalisées dans Matériau de base
* &amp;lbrack ; Layers&amp;rbrack ; Crash lors de la manipulation des calques
* &amp;lbrack ; Les couches&amp;rbrack ; personnalisées ne s&#39;affichent pas avec un matériau enregistré
* &amp;lbrack ;Application&amp;rbrack ; Correction d’un crash rare lors de l’importation d’une ressource
* &amp;lbrack ; Application&amp;rbrack ; Crash à la fermeture
* Les zones de liste déroulante &amp;lbrack ; Application&amp;rbrack ; affichent désormais des valeurs correctes lors du changement de paramètres prédéfinis
* &amp;lbrack ; Export&amp;rbrack ; Renommé Enscape prédéfini en Enscape Revit
* &amp;lbrack ; Export&amp;rbrack ; L&#39;importation d&#39;un paramètre prédéfini d&#39;exportation après l&#39;avoir supprimé fonctionne
* &amp;lbrack ; Export&amp;rbrack ; Crash à l&#39;exportation
* &amp;lbrack ; Rendu&amp;rbrack ; Rendu fixe lorsque la base color est au format demi-flottant 16 bits
* &amp;lbrack ;Project&amp;rbrack ; Ne pas effectuer de crash lors de l&#39;importation d&#39;un package corrompu
* &amp;lbrack ;Project&amp;rbrack ; Gérer la migration 2019.1.4 vers 2.x.x lorsque Create n&#39;a jamais été ouvert
* &amp;lbrack ;Project&amp;rbrack ; Corriger un crash lors de l&#39;importation du même projet deux fois
* &amp;lbrack ;Project&amp;rbrack ; Corriger un crash lors de l&#39;importation de projets
* Les filtres &amp;lbrack ; Resources&amp;rbrack ; personnalisés importés dans les versions précédentes fonctionnent
* &lbrack;Resources&amp;rbrack ; Les Matériaux portant le même nom ne s&#39;effacent plus
* crash &lbrack;Resources&rbrack; lors de la liaison d&#39;un dossier local
* &amp;lbrack ; Resources&amp;rbrack ; Matériaux pour démarrer les dossiers créés par l&#39;utilisateur ne sont plus supprimés après un redémarrage
* &amp;lbrack ;Inspire&amp;rbrack ; Corriger la zone de dépôt du matériau/de la collection et ajouter un message d&#39;avertissement si vous utilisez un matériau non enregistré

**Problèmes Connus :**

* Les filtres Fond basé sur le contenu sont lents en haute résolution
* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur

### 2.1.0 (2020.1.0) Tiramisu

*(Publié Le 12 Mars 2020)*

**Ajouté :**

* &amp;lbrack ; Export&amp;rbrack ; Export preset selection to pack your textures for renderers and game moteurs
* &amp;lbrack ; Export&amp;rbrack ; Export preset to Unreal Moteur 4
* &amp;lbrack ; Export&amp;rbrack ; Export preset to Unity Standard
* &amp;lbrack ; Export&amp;rbrack ; Export preset to Unity HDRP
* &amp;lbrack ; Export&amp;rbrack ; Export preset to Blender Cycles/Eeve
* &amp;lbrack ; Export&amp;rbrack ; Export preset to Arnold 5
* &amp;lbrack ; Export&amp;rbrack ; Export preset to Corona Renderer
* &amp;lbrack ; Export&amp;rbrack ; Export preset to Enscape
* &amp;lbrack ; Export&amp;rbrack ; Export preset to Keyshot 9
* &amp;lbrack ; Export&amp;rbrack ; Export preset to Redshift
* &amp;lbrack ; Export&amp;rbrack ; Export preset to Vray Next
* &amp;lbrack ; Export&amp;rbrack ; Export preset to Lens Studio
* &amp;lbrack ; Export&amp;rbrack ; Export preset to Spark AR Studio
* &amp;lbrack ; Export&amp;rbrack ; Export preset to PBR Specular Brillance from PBR Métallique rugosité
* &amp;lbrack ; Export&amp;rbrack ; New export UI
* &amp;lbrack ; Export&amp;rbrack ; Memory Export settings
* &amp;lbrack ; Export&amp;rbrack ; Importer et gérer vos paramètres prédéfinis d&#39;exportation personnalisés
* &amp;lbrack ; Export&amp;rbrack ; Supprimez et remplacez vos paramètres prédéfinis d&#39;exportation personnalisés
* &amp;lbrack ; Export&amp;rbrack ; Renommer vos paramètres prédéfinis d&#39;exportation personnalisés
* &amp;lbrack ; Export&amp;rbrack ; Définissez la résolution d&#39;exportation par défaut sur la résolution actuelle
* &amp;lbrack ; Export&amp;rbrack ; Ajouter le choix de créer un sous-dossier à l&#39;emplacement d&#39;exportation
* &amp;lbrack ; Export&amp;rbrack ; Message d&#39;avertissement avant de remplacer des fichiers existants
* &amp;lbrack ; Application&amp;rbrack ; Nouveau modèle de numérotation des versions
* &amp;lbrack ;Application&amp;rbrack ; Ouvrez Créer au lancement et modifiez l&#39;ordre des Lab
* &amp;lbrack ; Écran d&#39;accueil&amp;rbrack ; Nouvelle bannière d&#39;accueil
* &amp;lbrack ; Project&amp;rbrack ; Ouvrir le dernier projet au lancement
* &amp;lbrack ; UI&amp;rbrack ; Nouveau style de zone de liste déroulante
* &amp;lbrack ; Vue 2D&amp;rbrack ; F raccourci pour la mise au point dans la vue 2d
* &amp;lbrack ; Filters&amp;rbrack ; Prise en charge de la balise alchemist::parameterVisibility dans les graphes de Substance
* &amp;lbrack ; Filters&amp;rbrack ; Effectuez un réglage global pour gérer la visibilité des paramètres en fonction de votre workflow
* &amp;lbrack ; Resources&amp;rbrack ; Nouvelle option de ligne de commande pour configurer les ressources et les dossiers liés avec un fichier de configuration
* &amp;lbrack ; Vérificateur de version&amp;rbrack ; Configuration de la vérification de version
* &amp;lbrack ;Content&amp;rbrack ; Nouveaux matériaux de démarrage
* &amp;lbrack ;Content&amp;rbrack ; Bitmap to Matériau - Ajout de la possibilité de définir la couche métallique (uniforme, importation d&#39;image personnalisée, sélection de couleurs)
* &amp;lbrack ;Content&amp;rbrack ; Adjustment : ajoute la prise en charge du workflow specular/brillance PBR
* &amp;lbrack ;Content&amp;rbrack ; Atlas scatter - Nouveaux paramètres

**Fixe :**

* &amp;lbrack ;Project&amp;rbrack ; Crash lors de l&#39;importation du même projet deux fois
* &amp;lbrack ;Project&amp;rbrack ; crash fixe lors de l&#39;importation et de l&#39;ouverture de projets à plusieurs reprises
* crash &lbrack;Application&amp;rbrack ; lors du chargement d&#39;un matériau sans nom
* &amp;lbrack ; Application&amp;rbrack ; Reconnaître les fichiers manquants lors de leur réimportation
* &amp;lbrack ;Application&amp;rbrack ; Corriger le crash aléatoire à l&#39;arrêt
* &amp;lbrack ;Application&amp;rbrack ; Correction d&#39;un crash rare lors du déchargement d&#39;un matériau dans Créer
* &amp;lbrack ;Application&amp;rbrack ; crash aléatoire fixe lors de l&#39;utilisation des contrôles de l&#39;interface utilisateur
* &amp;lbrack ;Application&amp;rbrack ; Exportation fixe des fichiers journaux vers le bureau sous Windows 10
* Le panneau &amp;lbrack ;UI&amp;rbrack ; Export a la mauvaise taille lorsque vous l&#39;ouvrez dans Créer
* &amp;lbrack ; UI&amp;rbrack ; Ouvrir le projet en un seul clic
* &amp;lbrack ; UI&amp;rbrack ; Définissez correctement les valeurs minimum et maximum du curseur
* &amp;lbrack ; UI&amp;rbrack ; Afficher le libellé des utilisations de canal au lieu des id
* &amp;lbrack ;UI&amp;rbrack ; Cliquer sur un matériau ouvre/ferme toujours le panneau de réglage
* &amp;lbrack ; UI&amp;rbrack ; Correction des couleurs des calques masqués
* &amp;lbrack ; UI&amp;rbrack ; Amélioration des boutons de l&#39;écran d&#39;accueil
* &amp;lbrack ; Layers&amp;rbrack ; Moins de recalculs inutiles
* crashs de &amp;lbrack ; Layers&amp;rbrack ; lors de l&#39;utilisation du patch de Clone
* &amp;lbrack ; Layers&amp;rbrack ; La sélection d&#39;un calque d&#39;importation d&#39;image ne déclenche plus l&#39;ordinateur
* &amp;lbrack ; Layers&amp;rbrack ; Clone Patch and Content Aware Calques de remplissage ne sont plus recalculés lorsqu&#39;ils sont sélectionnés
* &amp;lbrack ; Les paramètres de canal&amp;rbrack ; L&#39;activation ou la désactivation des utilisations déclenchent désormais un rendu
* &amp;lbrack ;Resources&amp;rbrack ; Prévenir le gel lorsque l&#39;utilisateur clique en masse sur une pile de la bibliothèque
* &amp;lbrack ; Ressources&amp;rbrack ; Bouton de performance lors de la ré-ajout d&#39;un dossier lié précédemment ajouté
* &amp;lbrack ; Resources&amp;rbrack ; Correction d&#39;un crash lors de la tentative d&#39;ouverture d&#39;un fichier .fichier sbsar supprimé
* &amp;lbrack ; Performance&amp;rbrack ; Éviter de charger les matériaux pour accéder à leurs paramètres
* &amp;lbrack ; Performance&amp;rbrack ; Sauvegarde des ressources uniquement lorsqu&#39;elles sont utilisées dans un projet ou dans un matériau créé
* &amp;lbrack ; Export&amp;rbrack ; Les matériaux fixes de la file d&#39;attente d&#39;exportation sont parfois ignorés ou exportés avec des paramètres incorrects
* &amp;lbrack ; vue 2D&amp;rbrack ; Restauration du panoramique et du zoom
* &amp;lbrack ; Content&amp;rbrack ; Parquet Pattern prend en compte le canal Ambient occlusion
* &amp;lbrack ;Content&amp;rbrack ; Peinture : affiche la saisie du masque lorsque le masque personnalisé est activé
* &amp;lbrack ;Content&amp;rbrack ; Stonewall Pattern - Supprime les effets de bande possibles dans la map normal
* Modulation d&#39;Height &amp;lbrack ; Content&amp;rbrack ; - Corriger les entrées à double base color dans la vue 2d

**Problèmes Connus :**

* Les filtres Fond basé sur le contenu sont lents en haute résolution
* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur

## Version 1

### 1.1.4 (2019.1.4) Sésame

*(Publié Le 30 Janvier 2020)*

**Ajouté :**

* &amp;lbrack ; Resources&amp;rbrack ; Invite de confirmation lors de l&#39;effacement d&#39;un dossier de ressources

**Fixe :**

* &amp;lbrack ; Layers&amp;rbrack ; Déplace les calques vers deux calques ou plus en dessous ou au-dessus
* &amp;lbrack ;Create&amp;rbrack ; Allocation d&#39;un budget VRAM suffisant pour avoir de bonnes performances

**Problèmes Connus :**

* Importer beaucoup de ressources peut vraiment ralentir la Substance Alchemist
* Les filtres Fond basé sur le contenu sont lents en haute résolution
* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Le filtre Normal à l’Height peut effectuer un crash sur MacOS

### 1.1.3 (2019.1.3) Sésame

*(Publié Le 28 Janvier 2020)*

**Ajouté :**

* &amp;lbrack ; Workflow&amp;rbrack ; Prise en charge de plusieurs workflows
* &amp;lbrack ; Workflow&amp;rbrack ; Prise en charge du workflow de Brillance de Specular PBR
* &amp;lbrack ; Workflow&amp;rbrack ; Nouveau panneau Paramètres de canal
* &amp;lbrack ; Workflow&amp;rbrack ; Sélection du workflow lors de la création du projet
* &amp;lbrack ; Channel Settings&amp;rbrack ; Activer/désactiver un calcul de canal spécifique
* &amp;lbrack ; Channel Settings&amp;rbrack ; Affiche la liste des canaux personnalisés disponibles dans le matériau actif
* &amp;lbrack ; Channel Settings&amp;rbrack ; calcul automatique des canaux personnalisés si nécessaire
* &amp;lbrack ; Channel Settings&amp;rbrack ; Force/Bloquer le calcul des canaux personnalisés
* &amp;lbrack ; Layers&amp;rbrack ; Nouvelle interface utilisateur de l&#39;espace réservé d&#39;entrée de matériau dans les filtres Atlas scatter et Éclaboussure
* &amp;lbrack ; Layers&amp;rbrack ; Le Paramètre d&#39;entrée d&#39;image d&#39;un filtre peut être alimenté par les calques sous-jacents
* &amp;lbrack ; Layers&amp;rbrack ; Affiche une notification lorsque certains calques sont obsolètes
* &amp;lbrack ; Layers&amp;rbrack ; Possibilité de mettre à jour vers la dernière version des calques obsolètes via la notification
* &amp;lbrack ;Project&amp;rbrack ; Nouveaux champs de métadonnées lors de la création du projet
* Les variations &amp;lbrack ; générées par Inspire&amp;rbrack ; sont spécifiques à un projet
* &amp;lbrack ; vue 2D&amp;rbrack ; Basculer entre les entrées de calque, les sorties de calque et les sorties de matériau
* &amp;lbrack ; Écran d’accueil&amp;rbrack ; Option Ajouter un projet d’importation (.alch)
* &amp;lbrack ;Preferences&amp;rbrack ; New Preferences window to set cache location and analytics privacy settings
* &amp;lbrack ; UI&amp;rbrack ; Nouveaux boutons d&#39;interface utilisateur
* &amp;lbrack ; Performance&amp;rbrack ; Amélioration globale du système de parallélisation
* &amp;lbrack ; Performance&amp;rbrack ; Optimisation du nombre de calculs de matériau
* &amp;lbrack ; Moteur&amp;rbrack ; mise à jour de la Substance Engine
* &amp;lbrack ;Framework&amp;rbrack ; Mise à niveau vers Qt 5.13
* &amp;lbrack ; MacOS&amp;rbrack ; Améliorations globales de la prise en charge de macOS Catalina
* Filtre de réglage &amp;lbrack ; Content&amp;rbrack ; - Intensité normale et paramètres d&#39;inversion

**Fixe :**

* &amp;lbrack ; Layers&amp;rbrack ; Unset Image Paramètre d&#39;entrée when deleting the layer
* &amp;lbrack ; Layers&amp;rbrack ; Corriger un crash lors de l&#39;ajout d&#39;un calque de patch de duplication
* &amp;lbrack ; Layers&amp;rbrack ; Corrige certains crashs lors de la fusion des matériaux de pile des calques dans d&#39;autres matériaux de pile de calques
* La sélection de canaux &amp;lbrack ; Export&amp;rbrack ; pour l&#39;exportation est maintenant respectée
* &amp;lbrack ; Resources&amp;rbrack ; Ne pas effectuer de crash lors de la navigation dans le panneau Ressources
* &amp;lbrack ; Resources&amp;rbrack ; Corriger le crash lors de l&#39;importation de fichiers de Substance corrompus
* &amp;lbrack ; Resources&amp;rbrack ; Réduisez le nombre de crashs lors du chargement de dossiers volumineux
* &amp;lbrack ; Thumbnail&amp;rbrack ; Thumbnail calcul ne fige pas l&#39;interface
* &amp;lbrack ; Image Import&amp;rbrack ; Uniformisation du type d&#39;image prise en charge dans l&#39;application
* &amp;lbrack ; Preset&amp;rbrack ; Enregistre la description lors de la création d&#39;un paramètre prédéfini à partir d&#39;un SBSAR
* &amp;lbrack ; Inspire&amp;rbrack ; Fix image drag and drop
* &amp;lbrack ; Application&amp;rbrack ; Corriger les crashs à la sortie
* &amp;lbrack ; Application&amp;rbrack ; Corrige les crashs à la sortie lors de l&#39;exportation des matériaux
* &amp;lbrack ; UI&amp;rbrack ; Correctifs et améliorations
* &amp;lbrack ;UI&amp;rbrack ; Renommer la ressource temporaire en « matériau non enregistré »
* &amp;lbrack ; Content&amp;rbrack ; Mise à jour globale et nettoyage de tous les filtres

**Problèmes Connus :**

* Importer beaucoup de ressources peut vraiment ralentir la Substance Alchemist
* Les filtres Fond basé sur le contenu sont lents en haute résolution
* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Le filtre Normal à l’Height peut effectuer un crash sur MacOS

### 1.1.2 (2019.1.2) Sésame

*(Publié Le 11 Décembre 2019)*

**Ajouté :**

* Les options &amp;lbrack ; Layers&amp;rbrack ; Enregistrer et Enregistrer sous sont accessibles via l&#39;interface dans la barre d&#39;outils de la pile de calques
* &amp;lbrack ; Resources&amp;rbrack ; Chemin de navigation plus clair dans le panneau Ressources pour naviguer dans les dossiers
* &amp;lbrack ; Resources&amp;rbrack ; Maintenir le bouton Précédent enfoncé pour accéder à tous les dossiers supérieurs
* &amp;lbrack ;Resources&amp;rbrack ; Ajouter une option de rechargement des matériaux importés pour les mettre à jour vers la dernière version
* &amp;lbrack ; Layers&amp;rbrack ; Possibilité de modifier l&#39;image dans le calque d&#39;importation d&#39;image
* &amp;lbrack ; Layers&amp;rbrack ; Possibilité de définir une image comme couche (base color, normale, height,...) dans le calque d’importation d’image
* &amp;lbrack ;Content&amp;rbrack ; Nouveau Atlas scatter de dispersion des nouveaux éléments de l&#39;atlas à partir de la Substance Source
* &amp;lbrack ;Content&amp;rbrack ; Nouveau filtre Effet Peinture à l&#39;huile
* &amp;lbrack ;Content&amp;rbrack ; Nouveau filtre de génération de canaux pour générer l&#39;height, l&#39;ambient occlusion et la rugosité à partir de la base color et des maps normal

**Fixe :**

* &amp;lbrack ; UI&amp;rbrack ; Réactiver les info-bulles dans la barre d&#39;outils de la pile Calques
* &amp;lbrack ; UI&amp;rbrack ; Résoudre le problème lors de la saisie de deux décimales dans une valeur de curseur
* &amp;lbrack ; Performance&amp;rbrack ; Corriger le crash lors du basculement rapide entre les matériaux
* &amp;lbrack ; Export&amp;rbrack ; Le passage à un autre matériau avant la fin d&#39;une exportation ne crash plus
* Le menu contextuel de &amp;lbrack ;Resources&amp;rbrack ; s&#39;affiche en haut du matériau lorsque vous cliquez dessus avec le bouton droit
* &amp;lbrack ; Layers&amp;rbrack ; Le lien « Cliquer ici » fonctionne lorsque la pile de calques est vide
* &amp;lbrack ; Presets&amp;rbrack ; Remove save button dans le panneau de réglage lorsqu&#39;il s&#39;agit d&#39;un matériau créé dans Alchemist
* &amp;lbrack ;Tweak&amp;rbrack ; Le message d&#39;information s&#39;affiche lorsqu&#39;il s&#39;agit d&#39;un matériau créé dans Alchemist
* &amp;lbrack ;Viewport&amp;rbrack ; La valeur par défaut de la texture du Specular level est corrigée à 0,04
* &amp;lbrack ; File Menu&amp;rbrack ; Fix and rename Save and Save as option
* &amp;lbrack ; Moteur&amp;rbrack ; Mettre à jour la version du moteur de Substance de données pour éviter le crash de certains fichiers SBSAR lors de l&#39;importation.
* &amp;lbrack ;Content&amp;rbrack ; le filtre de Répétition fonctionne sur le canal ambient occlusion
* Le filtre &amp;lbrack ;Content&amp;rbrack ; Crop fonctionne sur la couche ambient occlusion
* Le filtre &amp;lbrack ;Content&amp;rbrack ; Water modifie la map height
* &amp;lbrack ; Content&amp;rbrack ; répétition correcte du matériau supérieur dans le mode de fusion de l&#39;opacité
* &amp;lbrack ;Content&amp;rbrack ; l&#39;Height du matériau supérieur est conservé dans le mode de fusion de l&#39;opacité
* &amp;lbrack ; Content&amp;rbrack ; Possibilité d&#39;ajouter un masque personnalisé, un motif personnalisé ou une carte d&#39;échelle dans le filtre Perforation
* &amp;lbrack ;Content&amp;rbrack ; Height Le filtre Modulation force l&#39;height et les maps normal en 16 bits
* &amp;lbrack ; Content&amp;rbrack ; Adjustment filter force l&#39;height et les maps normal en 16 bits

**Problèmes Connus :**

* Importer beaucoup de ressources peut vraiment ralentir la Substance Alchemist
* Les filtres Fond basé sur le contenu sont lents en haute résolution
* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Le filtre Normal à l’Height peut effectuer un crash sur MacOS

### 1.1.1 (2019.1.1) Sésame

*(Publié Le 26 Novembre 2019)*

**Ajouté :**

* &amp;lbrack ; Fusion&amp;rbrack ; Nouveau mode de Fusion d&#39;opacité
* &amp;lbrack ;Moteur&amp;rbrack ; Nouvelle version de Substance Engine

**Fixe :**

* &amp;lbrack ; Layers&amp;rbrack ; Corriger le crash lors de la suppression d&#39;un calque en cours de calcul
* &amp;lbrack ; Layers&amp;rbrack ; Réparer le crash lors de la suppression du calque inférieur
* &amp;lbrack ; Layers&amp;rbrack ; Corrige le crash lorsque le nom du matériau contient des caractères spéciaux
* &amp;lbrack ; Layers&amp;rbrack ; Arrêter de calculer tous les filtres qui utilisent un widget
* &amp;lbrack ; Layers&amp;rbrack ; Éviter le crash lors de l&#39;utilisation des filtres Pièce de Clone et Remplissage d&#39;après le contenu
* &amp;lbrack ; Layers&amp;rbrack ; Corriger le crash en faisant glisser un filtre dans les emplacements d&#39;entrée des éclaboussures
* &amp;lbrack ; Resources&amp;rbrack ; Corriger le crash lors de la liaison de dossiers locaux ou de l&#39;importation de ressources dans la Substance Alchemist
* &amp;lbrack ; Collection&amp;rbrack ; Corriger le crash lors du basculement rapide entre les matériaux
* &amp;lbrack ; UI&amp;rbrack ; Corriger le crash lorsque la valeur est nulle ou non valide dans la répétition, curseurs de displacement sur le viewport
* &amp;lbrack ; Inspire&amp;rbrack ; Corriger le crash lors de l&#39;accès à l&#39;onglet Inspire
* &amp;lbrack ; Inspire&amp;rbrack ; Corriger le crash tout en inspirant sur un matériau de pile de calques qui vient d&#39;être enregistré
* &amp;lbrack ; Performance&amp;rbrack ; matériaux et filtres de Substance lourde (Répétition) calculent plus rapidement
* &amp;lbrack ; Help&amp;rbrack ; Fix export log file
* Le filtre Aléatoire &amp;lbrack ; Content&amp;rbrack ; fonctionne sur tous les canaux
* Le workflow &amp;lbrack ;Content&amp;rbrack ; Multiangle prend en compte toutes les numérisations
* &amp;lbrack ;Content&amp;rbrack ; AO Fusion de fusion correcte
* &amp;lbrack ;Content&amp;rbrack ; Courbure Fusion fusion correcte
* &amp;lbrack ;Content&amp;rbrack ; Color ID Fusion de fusion correcte
* &amp;lbrack ; Content&amp;rbrack ; Fusion de masque personnalisée fusion correcte
* &amp;lbrack ;Content&amp;rbrack ; Filtre de réglage de correction pour la modification de rugosité
* &amp;lbrack ;Content&amp;rbrack ; Réparer le filtre de Matériau de base pour le téléchargement de canaux normaux personnalisés
* &amp;lbrack ; Content&amp;rbrack ; Fix Custom Import pattern of the Embossing filter

**Problèmes Connus :**

* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Le filtre Normal à l’Height peut effectuer un crash sur MacOS

### 1.1.0 (2019.1.0) Sésame

*(Publié Le 4 Novembre 2019)*

**Ajouté :**

* &amp;lbrack ; Project&amp;rbrack ; Création d&#39;un projet
* &amp;lbrack ; Project&amp;rbrack ; Introduction du format de fichier .alch qui contient les données du projet
* &amp;lbrack ;Project&amp;rbrack ; Export a .alch project contenant les collections et leurs matériaux
* &amp;lbrack ; Project&amp;rbrack ; Importer un projet .alch
* &amp;lbrack ; Project&amp;rbrack ; Ouvrir les projets récents
* &amp;lbrack ; Écran d&#39;accueil&amp;rbrack ; Un écran d&#39;accueil s&#39;affiche au lancement
* &amp;lbrack ;Welcome Screen&amp;rbrack ; Créer un projet à partir de l&#39;écran d&#39;accueil
* &amp;lbrack ;Welcome Screen&amp;rbrack ; Accéder à la liste de tous vos projets dans l’écran d’accueil
* &amp;lbrack ; Écran d’accueil&amp;rbrack ; Liens rapides pour accéder à la documentation, au menu contextuel à propos et à la gestion des licences
* &amp;lbrack ; File Menu&amp;rbrack ; Integration of a file Menu
* &amp;lbrack ;File Menu&amp;rbrack ; Accédez aux commandes du projet à partir de l&#39;onglet Fichier et de l&#39;enregistrement de la pile de calques
* &amp;lbrack ; File Menu&amp;rbrack ; Accédez aux commandes Annuler et Rétablir à partir de l&#39;onglet Edition
* &lbrack;Menu Fichier&amp;rbrack ; Le menu d&#39;aide précédent a été déplacé dans le menu Fichier sous l&#39;onglet Aide
* &amp;lbrack ; Layers&amp;rbrack ; Nouvelle architecture de la pile de calques
* &amp;lbrack ; Layers&amp;rbrack ; Nouvelle interface utilisateur de la pile de calques
* &amp;lbrack ; Layers&amp;rbrack ; Sélectionnez le mode de fusion directement dans la barre d&#39;outils
* &amp;lbrack ; Layers&amp;rbrack ; Accédez séparément aux paramètres de fusion et aux paramètres de matériau
* &amp;lbrack ; Layers&amp;rbrack ; Ajoutez des matériaux directement dans les entrées dédiées du filtre Éclaboussure de la pile de calques
* &amp;lbrack ; Layers&amp;rbrack ; Modifier l&#39;ordre de numérisation directement dans le calque d&#39;importation d&#39;image
* &amp;lbrack ; Viewport&amp;rbrack ; Contrôle du champ de vision de caméra
* &amp;lbrack ; Viewport&amp;rbrack ; Possibilité de basculer entre la caméra orthographique ou perspective
* &amp;lbrack ; Viewport&amp;rbrack ; Affiche la résolution et les informations de nombre de bits par pixel pour chaque canal
* &lbrack;Resources&amp;rbrack ; Matériaux de base ouverts par défaut
* &amp;lbrack ; Cache&amp;rbrack ; Localisez le dossier de cache de vos vignettes
* &amp;lbrack ;Cache&amp;rbrack ; Recherchez votre dossier de cache de rendu
* &amp;lbrack ; Panneaux&amp;rbrack ; Le panneau Paramètres de Matériau est temporairement masqué
* &amp;lbrack ;Workflow&amp;rbrack ; Specular/Brillance temporairement désactivé
* Authentification notariale pour la version du système d’exploitation Catalina &amp;lbrack ; MacOS&amp;rbrack ;
* &amp;lbrack ; Content&amp;rbrack ; Nouvelle version du filtre Delighter
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre Image Fond basé sur le contenu
* &amp;lbrack ;Content&amp;rbrack ; Nouveau Matériau de remplissage d&#39;après le contenu
* Le filtre de Transforme &amp;lbrack ;Content&amp;rbrack ; dispose d&#39;une option de transforme sécurisée

**Fixe :**

* Tous les bugs précédents liés à Créer ne sont pas valides aujourd’hui avec la nouvelle version de l’interface utilisateur et de l’architecture
* Les info-bulles ne masquent pas les icônes de la barre supérieure (3D, 2D, 2D/3D).
* Le filtre &amp;lbrack ; Content&amp;rbrack ; Splatter accepte Atlas avec une map height complète
* &amp;lbrack ;Content&amp;rbrack ; Transforme fonctionne sur les images (scan1, scan2,...)

**Problèmes Connus :**

* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Le filtre Normal à l’Height peut effectuer un crash sur MacOS

## Beta

### 0.8.1-bêta Quinoa

*(Publié Le 19 Août 2019)*

**Ajouté :**

* Possibilité d’envoyer des ressources de Substance Source du lanceur vers la Substance Alchemist Projet

**Fixe :**

* &amp;lbrack ; Create&amp;rbrack ; Certains filtres étaient répertoriés dans l&#39;accesseur rapide mais pas dans le panneau de filtre
* &amp;lbrack ; MacOS&amp;rbrack ; Correction de certains crashs à la sortie

**Problèmes Connus :**

* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Le basculement rapide de visibilité d’une scène Delighter n’est pas recommandé
* Les images Tif ne s’affichent pas dans le panneau Propriétés du calque d’importation d’image
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Le filtre Normal à l’height peut effectuer un crash sur MacOS
* Peut toujours effectuer des crashs aléatoires lors de la fermeture sur MacOS

### 0.8.0-bêta Quinoa

*(Publié Le 8 Août 2019)*

**Ajouté :**

* &amp;lbrack ;Resources&amp;rbrack ; Connectez et mettez en miroir vos dossiers de matériau sur vos disques locaux
* &amp;lbrack ;Resources&amp;rbrack ; Parcourir vos dossiers matériau et leurs sous-dossiers
* &amp;lbrack ;Resources&amp;rbrack ; Dissociez le panneau des ressources matériau dans une fenêtre séparée pour afficher vos ressources en plein écran
* &amp;lbrack ; Ressources&amp;rbrack ; Nouvelle disposition du panneau Ressources pour prendre en charge la navigation dans les dossiers et sous-dossiers
* &amp;lbrack ; Resources&amp;rbrack ; Utilisez le chemin de navigation pour naviguer dans vos dossiers
* &amp;lbrack ; Resources&amp;rbrack ; Force la synchronisation de votre dossier local avec l&#39;option Sync accessible via un clic droit
* &amp;lbrack ; Resources&amp;rbrack ; Déconnectez votre dossier local avec l&#39;option Déconnecter accessible via un clic droit
* &amp;lbrack ; Manage&amp;rbrack ; Affiche les balises incorporées des fichiers de Substance
* &amp;lbrack ; Manage&amp;rbrack ; Ajouter, modifier et supprimer les balises de vos matériaux
* &amp;lbrack ; Manage&amp;rbrack ; Noter vos matériaux
* &amp;lbrack ; Layers&amp;rbrack ; prend en charge la sortie en panorama
* &amp;lbrack ; Layers&amp;rbrack ; Vous pouvez supprimer les entrées d&#39;image dans le calque d&#39;importation d&#39;image
* &amp;lbrack ; Layers&amp;rbrack ; Sélection automatique du nouveau calque ajouté
* &amp;lbrack ; Layers&amp;rbrack ; Sélection automatique du calque en dessous après la suppression d&#39;un calque
* &amp;lbrack ; UX&amp;rbrack ; Conserver la visibilité des panneaux de gauche lors du passage à un autre Lab
* &amp;lbrack ; UX&amp;rbrack ; Ne créez pas de calque de base et n&#39;ouvrez pas la fenêtre contextuelle Matériau Workflow lors de l&#39;importation d&#39;images dans une pile de calques non vide
* &amp;lbrack ; UI&amp;rbrack ; Nouveau style de champ de texte
* &amp;lbrack ; UI&amp;rbrack ; Nouveau style SearchBox
* &amp;lbrack ; UI&amp;rbrack ; Nouveau style d&#39;en-tête de panneau
* &amp;lbrack ; UI&amp;rbrack ; Nouveau style d&#39;indicateur Occupé
* &amp;lbrack ;UI&amp;rbrack ; Nouveau style d&#39;arrière-plan de pile de calques
* &amp;lbrack ; UI&amp;rbrack ; Utiliser la police Adobe Clean
* &amp;lbrack ; UI&amp;rbrack ; Supprimer l’icône de pipette de l’espace réservé au paramètre d&#39;entrée de couleur
* &amp;lbrack ; Performance&amp;rbrack ; Occupé optimisation de l&#39;indicateur
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre du générateur de motifs
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre Flou

**Fixe :**

* &amp;lbrack ; Inspire&amp;rbrack ; Corrige le crash lorsque vous utilisez plus de 10 couleurs
* &amp;lbrack ; vue 2D&amp;rbrack ; Fixe la barre de défilement sur la liste des canaux de la Vue 2D
* &amp;lbrack ;Viewer&amp;rbrack ; Corriger le crash lors de l&#39;importation d&#39;une puissance autre que 2 maps d&#39;environnement
* &amp;lbrack ; Content&amp;rbrack ; Fix PNG import for custom pattern of Embossing and Perforation filters
* &amp;lbrack ; Export&amp;rbrack ; Fix normal et height 16 bits par exportation de canal
* Correction d’une boucle infinie lors de l’importation d’un matériau avec deux paramètres prédéfinis portant le même nom
* Correction de l’affichage du chemin de fichier long dans le calque de Matériau de base

**Problèmes Connus :**

* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Le basculement rapide de visibilité d’une scène Delighter n’est pas recommandé
* Les images Tif ne s’affichent pas dans le panneau Propriétés du calque d’importation d’image
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Le filtre Normal à l’height peut effectuer un crash sur MacOS
* Peut effectuer un crash aléatoire lors de la fermeture sur MacOS

### 0.7.0-beta Pepper

*(Publié Le 13 Juin 2019)*

**Ajouté :**

* &amp;lbrack ; Filters&amp;rbrack ; Accédez rapidement à vos filtres en appuyant sur la barre d&#39;espace
* &amp;lbrack ; Filters&amp;rbrack ; Nouveau panneau dédié pour gérer, parcourir et importer vos filtres
* &amp;lbrack ; Metadata&amp;rbrack ; Cliquez avec le bouton droit de la souris sur un matériau pour voir ses métadonnées
* &amp;lbrack ; Metadata&amp;rbrack ; Cliquez avec le bouton droit de la souris sur un matériau pour voir son emplacement sur votre disque
* &amp;lbrack ; Sliders&amp;rbrack ; Animez les curseurs lorsque vous les survolez en appuyant sur Ctrl
* &amp;lbrack ; Sliders&amp;rbrack ; Arrêtez et redémarrez l&#39;animation de vos curseurs en appuyant sur P
* L&#39;exportation SBSAR &amp;lbrack ; Export&amp;rbrack ; suit les directives de Substance Source
* &amp;lbrack ; License&amp;rbrack ; Activer la Substance Alchemist à l&#39;aide d&#39;une variable d&#39;environnement
* La boîte de dialogue Fichier &amp;lbrack ;UX&amp;rbrack ; mémorise le dernier chemin de fichier sélectionné
* La boîte de dialogue Dossier &amp;lbrack ;UX&amp;rbrack ; mémorise le dernier chemin de dossier sélectionné
* &amp;lbrack ; UI&amp;rbrack ; Mettre à jour l&#39;interface utilisateur du panneau Ressources
* &amp;lbrack ; UI&amp;rbrack ; Mettre à jour l&#39;interface utilisateur de la barre de recherche
* &amp;lbrack ;UI&amp;rbrack ; L&#39;icône Créer un nouveau matériau est mise à jour
* Les URL &amp;lbrack ; Help&amp;rbrack ; sont mises à jour vers le domaine substance3d.com
* &amp;lbrack ; Maillage&amp;rbrack ; Un maillage en tissu est maintenant disponible
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre de corrosion
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre d&#39;oxydation
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre de mousse
* &amp;lbrack ;Content&amp;rbrack ; Nouveau filtre de Dust
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre de motif de mur de briques
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre de motif de mur de pierre
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre de finition du bois
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre de finition métallique
* &amp;lbrack ;Content&amp;rbrack ; Nouveau filtre de Snow
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre aléatoire
* &amp;lbrack ;Content&amp;rbrack ; Vous pouvez désormais importer vos textures directement dans le filtre de Matériau de base

**Fixe :**

* Corriger un crash lors de l’enregistrement de la pile de calques
* Possibilité d’ajouter une valeur supérieure à 1 dans le curseur de rotation de l’environnement
* Ne perdez pas les paramètres de fusion lorsqu’un calque de fusion est transformé d’avant en arrière d’un calque de fusion à un calque de matériau
* Correction des doublons lors de la génération de variations de la même pile de calques plusieurs fois
* Lors de la réouverture d’un matériau, Alchemist mémorise les plages modifiées (min et max) de vos curseurs

**Problèmes Connus :**

* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Le basculement rapide de visibilité d’une scène Delighter n’est pas recommandé
* L’importation d’environnement personnalisée peut devenir noire
* Les images Tif ne s’affichent pas dans le panneau Propriétés du calque d’importation d’image
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* Le filtre Normal à l’height peut effectuer un crash sur MacOS

### 0.6.1-bêta Orange

*(Publié Le 13 Juin 2019)*

**Ajouté :**

* &amp;lbrack ; Moteur&amp;rbrack ; mise à jour de la Substance Engine de données compatible avec la dernière version de la Substance Designer
* &amp;lbrack ; License&amp;rbrack ; Mise à jour du dossier de licence pour les premières installations
* &amp;lbrack ; Layers&amp;rbrack ; Rechargez à tout moment votre pile de calques à mettre à jour vos filtres personnalisés

**Fixe :**

* &amp;lbrack ; Data Compatibility&amp;rbrack ; Correction préventive pour limiter la corruption des données au moment de la mise à niveau

**Problèmes Connus :**

* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Le basculement rapide de visibilité d’une scène Delighter n’est pas recommandé
* L’importation d’environnement personnalisée peut devenir noire
* Les images Tif ne s’affichent pas dans le panneau Propriétés du calque d’importation d’image
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur

### 0.6.0-beta Orange

*(Publié Le 18 Avril 2019)*

**Ajouté :**

* &amp;lbrack ; Metadata&amp;rbrack ; Affichez et remplissez les métadonnées des matériaux dans un onglet dédié
* &amp;lbrack ; Collection&amp;rbrack ; Créer une collection directement à partir des résultats de la recherche
* &amp;lbrack ; Media Publishing&amp;rbrack ; Exportation d&#39;une carte d&#39;une collection
* &amp;lbrack ; UX&amp;rbrack ; Annuler une modification ou une importation d&#39;image en appuyant sur Ctrl+Z
* &amp;lbrack ; UX&amp;rbrack ; Rétablir une modification ou une importation d&#39;image en appuyant sur Ctrl+Maj+Z
* &amp;lbrack ; UI&amp;rbrack ; Nouvelles icônes avec un nouveau style
* &amp;lbrack ; Performance&amp;rbrack ; Nouveau gestionnaire de sessions pour mieux gérer le basculement des onglets
* &amp;lbrack ; Performance&amp;rbrack ; Ouverture plus rapide du calque d&#39;importation d&#39;image
* &amp;lbrack ;Content&amp;rbrack ; New Metal matériau générique
* &amp;lbrack ;Content&amp;rbrack ; Nouveau matériau de Rouille
* &amp;lbrack ;Content&amp;rbrack ; New Stone matériau générique
* &amp;lbrack ; Content&amp;rbrack ; Mise à jour du filtre d’estampage
* &amp;lbrack ; Content&amp;rbrack ; Mise à jour du filtre Broderie
* &amp;lbrack ;Content&amp;rbrack ; Peinture filter update
* &amp;lbrack ;Content&amp;rbrack ; Mise à jour du filtre Delighter

**Fixe :**

* Le filtre &amp;lbrack ; Content&amp;rbrack ; Water fonctionne dans le workflow Specular/Brillance
* Correction du bouton radio Niveaux de gris dans la fenêtre contextuelle d’activation
* Accepter les fichiers contenant un caractère de coma
* Correction des problèmes de petites polices dans les fenêtres contextuelles
* Correction d’un problème d’interface utilisateur de transparence dû à un conflit avec le paramètre FXAA de certaines cartes NVIDIA
* Supprimer le focus du champ après avoir saisi une valeur dans un curseur
* Allouez la quantité minimale de VRAM au délice pour réduire les crashs
* Corriger le blocage de la fenêtre lors du redimensionnement de la fenêtre d’application
* Correction d’un crash lorsque la pile de calques était supprimée lors de l’évaluation

**Problèmes Connus :**

* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Le basculement rapide de visibilité d’une scène Delighter n’est pas recommandé
* L’importation d’environnement personnalisée peut devenir noire
* Les images Tif ne s’affichent pas dans le panneau Propriétés du calque d’importation d’image
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur

### 0.5.4-beta Nacho

*(Publié Le 26 Mars 2019)*

**Fixe :**

* crash &amp;lbrack ; Pile&amp;rbrack ; lors de la suppression d&#39;un calque de projection
* La base de données &amp;lbrack ; Data&amp;rbrack ; Asset est corrompue lors des crashs d&#39;application
* La Substance Alchemist de données &amp;lbrack ; Data&amp;rbrack ; ne peut pas démarrer lorsque la base de données des actifs est endommagée
* Crash aléatoire lors de l’importation de matériaux de Substance

**Problèmes Connus :**

* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Le bouton d’activation/désactivation de la visibilité rapide d’une scène Delighter affecte les performances
* L’importation d’environnement personnalisée peut devenir noire
* Les images Tif ne s’affichent pas dans le panneau Propriétés du calque d’importation d’image
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* La collection par défaut dans laquelle enregistrer peut être vide

### 0.5.3-bêta Nacho

*(Publié Le 19 Mars 2019)*

**Ajouté :**

* Recherche par nom de matériau dans le panneau Ressources
* &amp;lbrack ; UI&amp;rbrack ; Outil de Clone nouvelle interface utilisateur avec visualisation de l&#39;épaisseur du pinceau
* &amp;lbrack ; UI&amp;rbrack ; Sélectionner et supprimer les étapes masquées
* &amp;lbrack ; UI&amp;rbrack ; Nouvelle interface utilisateur de champ de texte
* &amp;lbrack ;Help&amp;rbrack ; Accéder aux sites web des académies de Substance Source, Substance share et Substance
* &amp;lbrack ;Content&amp;rbrack ; Nouveaux matériaux par défaut avec générateurs et atlas
* &amp;lbrack ;Content&amp;rbrack ; Bitmap to Matériau Update
* &amp;lbrack ;Content&amp;rbrack ; Dirt Update
* &amp;lbrack ;Content&amp;rbrack ; Rouille Update
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre d’estampage
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre de broderie
* &amp;lbrack ;Content&amp;rbrack ; Nouveau Filtre Érosion
* &amp;lbrack ; Content&amp;rbrack ; New Gravel Generator
* &amp;lbrack ;Content&amp;rbrack ; Nouveau filtre de Peinture
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre Motif de parquet
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre de motif de chaussée
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre de perforation
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre Effet pointilliste
* &amp;lbrack ; Content&amp;rbrack ; Nouveau filtre d&#39;usure textile
* &amp;lbrack ;Content&amp;rbrack ; Nouveau filtre de Transforme

**Fixe :**

* &amp;lbrack ; Viewport&amp;rbrack ; maillage sphère avec répétition x2 sur X
* &amp;lbrack ; Viewport&amp;rbrack ; Crash lors du chargement de votre propre environnement
* la Map d&#39;environnement &amp;lbrack ; Viewport&amp;rbrack ; utilise désormais également la valeur d&#39;exposition
* &amp;lbrack ; Viewport&amp;rbrack ; F raccourci ne réinitialise pas l&#39;angle de caméra
* L’exportation SBS &amp;lbrack ; Export&amp;rbrack ; fonctionne avec la dernière version de Substance Designer 2018.3.3
* L&#39;exportation SBSAR &amp;lbrack ; Export&amp;rbrack ; respecte les mêmes directives que les matériaux de Substance Source
* &amp;lbrack ; Les barres de défilement de l&#39;interface utilisateur peuvent être déplacées
* Les caractères spéciaux sont pris en charge dans les chemins de dossier et de fichier
* La vignette est régénérée lorsque vous enregistrez votre matériau

**Problèmes Connus :**

* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Le bouton d’activation/désactivation de la visibilité rapide d’une scène Delighter affecte les performances
* L’importation d’environnement personnalisée peut devenir noire
* Les images Tif ne s’affichent pas dans le panneau Propriétés du calque d’importation d’image
* Les virgules ou les points peuvent être ignorés lors de la saisie d’une valeur spécifique dans un curseur
* La collection par défaut dans laquelle enregistrer peut être vide

### 0.5.2-beta Nacho

*(Publié Le 7 Mars 2019)*

**Ajouté :**

* Détection et utilisation du GPU de profil élevé

**Fixe :**

* Le paramètre de rotation a un widget de curseur approprié
* Correction de la visibilité de la ligne bleue lors du glisser-déposer de matériaux
* Correction de la fusion des matériaux lors de la dépose d’un matériau sous le premier calque
* Ne branchez les entrées d’image que si aucun chemin d’image personnalisé n’est défini

**Problèmes Connus :**

* Les caractères spéciaux dans le chemin de fichier empêchent l’enregistrement d’un matériau
* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Le bouton d’activation/désactivation de la visibilité rapide d’une scène Delighter affecte les performances
* Crash lors du chargement de votre propre environnement

### 0.5.1-bêta Nacho

*(Publié Le 4 Mars 2019)*

**Fixe :**

* Résolution des pop-ups de rapport de Crash, de rapport de bogue et de licences

**Problèmes Connus :**

* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Le bouton d’activation/désactivation de la visibilité rapide d’une scène Delighter affecte les performances
* Crash lors du chargement de votre propre environnement

### 0.5.0-beta Nacho

*(Publié Le 28 Février 2019)*

**Ajouté :**

* &amp;lbrack ; Pile de calques&amp;rbrack ; Réorganisation des calques
* &amp;lbrack ; Pile de calques&amp;rbrack ; Supprimer un calque masqué
* &amp;lbrack ; Pile de calques&amp;rbrack ; Importer un matériau directement à la position de votre choix
* &amp;lbrack ; Pile de calques&amp;rbrack ; entrée de Matériau en tant que nouveau type de paramètre de filtre
* &amp;lbrack ; Performance&amp;rbrack ; Le budget de Substance Engine est dynamique pour de meilleures performances
* &amp;lbrack ; Performance&amp;rbrack ; Meilleures performances OpenGL, en particulier sur MacOS
* &amp;lbrack ; Data&amp;rbrack ; Mise à niveau plus rapide des données après la publication d&#39;une nouvelle version
* &amp;lbrack ;Content&amp;rbrack ; AI Delighter disponible sous Windows 7 et Windows 8
* &amp;lbrack ; Content&amp;rbrack ; AI Delighter disponible sur le GPU RTX

**Fixe :**

* Correction des crashs possibles lors de la fermeture de l’application
* La fenêtre contextuelle Exporter s’ouvre plus rapidement lors de l’exportation de grandes collections

**Problèmes Connus :**

* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Le bouton d’activation/désactivation de la visibilité rapide d’une scène Delighter affecte les performances
* Crash lors du chargement de votre propre environnement

### 0.4.0-beta Muffin

*(Publié Le 17 Janvier 2019)*

**Ajouté :**

* &amp;lbrack ; Export&amp;rbrack ; Substance archive (sbsar) export of your collection
* &amp;lbrack ; Export&amp;rbrack ; exportation de votre collection à l&#39;aide d&#39;un fichier de Substance (sbs)
* &amp;lbrack ; Export&amp;rbrack ; File d&#39;attente d&#39;exportation visible dans le panneau Exporter
* &amp;lbrack ; Export&amp;rbrack ; Nommez votre collection ou votre matériau avant l&#39;exportation
* &amp;lbrack ; Data&amp;rbrack ; Enregistrez comme matériau en appuyant sur Ctrl+Maj+S
* &amp;lbrack ; Data&amp;rbrack ; Enregistrez votre matériau en appuyant sur Ctrl+S
* Les collections et les Matériaux de &amp;lbrack ;Data&amp;rbrack ; sont compatibles entre les versions
* &amp;lbrack ; Data&amp;rbrack ; Mettez à jour votre pile de calques de matériau avec des filtres à jour
* &amp;lbrack ; Data&amp;rbrack ; Rechargement à chaud des filtres personnalisés importés
* &amp;lbrack ; UI&amp;rbrack ; Retour visuel dans le viewport pendant l&#39;informatique
* &amp;lbrack ; UI&amp;rbrack ; Nouveau style de bouton
* La fenêtre contextuelle &amp;lbrack ;UI&amp;rbrack ; Save affiche le nom de la collection active
* &amp;lbrack ; UI&amp;rbrack ; Modifier les images sources d&#39;un calque d&#39;importation d&#39;image(s)
* Les utilisations personnalisées de &amp;lbrack ; Content&amp;rbrack ; sont désormais prises en charge
* &amp;lbrack ; Content&amp;rbrack ; Le format Plus d&#39;images est pris en charge dans les paramètres d&#39;entrée d&#39;images
* &amp;lbrack ;Content&amp;rbrack ; Nouveau filtre de Répétition nommé Rendre la mosaïque avancée
* &amp;lbrack ; Content&amp;rbrack ; Mise à jour du filtre Eau

**Fixe :**

* Le bitmap en Matériau gère le workflow Specular/Brillance

**Problèmes Connus :**

* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Delighter n’est pas pris en charge sur la carte GPU RTX
* Le bouton d’activation/désactivation de la visibilité rapide d’une scène Delighter affecte les performances

### 0.3.1-bêta Lasagne

*(Publié Le 17 Décembre 2018)*

**Fixe :**

* Générer une variation de couleur avec 10 crashs extraits de couleur
* Génération d’une variante de couleur avec un crash de pile de calques enregistré récemment
* Liens incorrects dans la fenêtre contextuelle de mise à jour de la version de la Substance Alchemist

**Problèmes Connus :**

* Le bitmap vers le Matériau ne gère pas le workflow Specular/Rugosité
* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Le bouton d’activation/désactivation de la visibilité rapide d’une scène Delighter affecte les performances

### 0.3.0-bêta Lasagne

*(Publié Le 12 Décembre 2018)*

**Ajouté :**

* &amp;lbrack ; Export&amp;rbrack ; New Export pop-up
* &amp;lbrack ; Export&amp;rbrack ; Exporter une collection entière
* &amp;lbrack ; Export&amp;rbrack ; Export Bitmaps at the format of your choice
* &amp;lbrack ; Export&amp;rbrack ; Export Bitmaps at the resolution of your choice
* &amp;lbrack ; Export&amp;rbrack ; Exporte uniquement les canaux de votre choix
* &amp;lbrack ; Export&amp;rbrack ; Prévisualisez la taille estimée de votre exportation
* &amp;lbrack ; Export&amp;rbrack ; Affichez un aperçu de la taille disponible sur votre disque avant l&#39;exportation
* &amp;lbrack ; UX&amp;rbrack ; Actions sur la collection accessibles via un clic droit
* &amp;lbrack ; UX&amp;rbrack ; Permet de désélectionner une image ou une ressource dans Inspire
* La Substance Alchemist &amp;lbrack ;UX&amp;rbrack ; est lancée agrandie
* &amp;lbrack ; Assets&amp;rbrack ; Nouvelle façon d&#39;enregistrer vos matériaux afin de les garder persistants avec les prochaines versions
* &amp;lbrack ;Help&amp;rbrack ; Accès à la documentation en ligne via le menu d&#39;aide
* &amp;lbrack ; Performance&amp;rbrack ; Variations de couleurs plus rapides sur les matériaux complexes créés avec Substance Alchemist
* &amp;lbrack ; Performance&amp;rbrack ; Réduire les fuites de mémoire lors du changement de Lab
* &amp;lbrack ;Content&amp;rbrack ; Scale checker pour diagnostiquer la taille physique de votre matériau
* &amp;lbrack ; Content&amp;rbrack ; Update Italien Venice Mosaic matériau
* &amp;lbrack ; Content&amp;rbrack ; Mettre à jour la dispersion de mousse

**Fixe :**

* Plus de nom par défaut lors de l’enregistrement d’un matériau
* Les paramètres des filtres sont perdus après l’enregistrement d’un matériau et la réouverture de la Substance Alchemist
* &amp;lbrack ; Content&amp;rbrack ; Corriger la logique de bas en haut pour la fusion AO et de courbure

**Problèmes Connus :**

* Les matériaux créés avec une version précédente ne seront pas disponibles dans la nouvelle version.
* Le bitmap vers le Matériau ne gère pas le workflow Specular/Rugosité
* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Le bouton d’activation/désactivation de la visibilité rapide d’une scène Delighter affecte les performances

### 0.2.0-beta Kiwi

*(Publié Le 9 Novembre 2018)*

**Ajouté :**

* Les paramètres de la visionneuse sont enregistrés d’une session à une autre
* Les paramètres de matériau sont enregistrés d’une session à une autre
* Chargement rapide du panneau Propriétés
* &amp;lbrack ; Log&amp;rbrack ; Exporter le fichier journal via le menu Aide
* &amp;lbrack ; UI&amp;rbrack ; New Sliders Style
* &amp;brack ; UI&amp;rbrack ; Les panneaux Paramètres prédéfinis et Réglage sont fusionnés
* &amp;lbrack ; UI&amp;rbrack ; New Thumbnails style
* Paramètres displacement, Répétition et Ombres accessibles directement dans le viewport
* &amp;lbrack ;Content&amp;rbrack ; Nouveaux Matériaux par défaut
* &amp;lbrack ; Content&amp;rbrack ; Moss Splatter update
* &amp;lbrack ; Framework&amp;rbrack ; Update Substance Engine Framework

**Fixe :**

* La suppression de votre pile de calques en changeant de Lab est corrigée
* Les valeurs de temps de chargement affichées dans le viewport sont correctes
* Les canaux par défaut du workflow de matériau sont correctement initialisés
* Désactiver l’importation de Maillage personnalisée
* Exportation de bitmap
* &amp;lbrack ;MacOS&amp;rbrack ; La fermeture de la Substance Alchemist peut nécessiter une action « Forcer à quitter »

**Problèmes Connus :**

* Les matériaux créés avec une version précédente ne seront pas disponibles dans la nouvelle version.
* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Le bouton d’activation/désactivation de la visibilité rapide d’une scène Delighter affecte les performances

### 0.1.1-beta Jam

*(Publié Le 24 Octobre 2018)*

**Ajouté :**

* BaseColor Delighter est maintenant disponible
* Accès aux informations sur les Substances Alchemist via le menu Aide
* Recevoir une notification lorsqu’une nouvelle version de la Substance Alchemist est disponible
* La console n’est plus visible sous Windows
* Nouveau style de vignettes
* La Substance Alchemist de &amp;lbrack ;MacOS&amp;rbrack ; peut être définie en plein écran
* &amp;lbrack ; Filter&amp;rbrack ; Import Custom mask to manage the blending between two matériaux
* &amp;lbrack ; Filter&amp;rbrack ; Control Moss scale
* &amp;lbrack ; Filter&amp;rbrack ; Clone Mise à jour du correctif

**Fixe :**

* Ajouter une image dans une entrée d’image dans la liste de paramètres met à jour les sorties
* Le filtre Importer personnalisé n’ajoute pas d’Ambient occlusion noir ni d’opacité noire

**Problèmes Connus :**

* Les matériaux créés avec une version précédente ne seront pas disponibles dans la nouvelle version.
* &amp;lbrack ;MacOS&amp;rbrack ; La fermeture de la Substance Alchemist peut nécessiter une action « Forcer à quitter »
* Il n’est pas recommandé d’utiliser plusieurs charmes dans un même matériau
* Crashs Delighter avec pilotes NVIDIA plus anciens (moins de 400.x)
* Le bouton d’activation/désactivation de la visibilité rapide d’une scène Delighter affecte les performances
* crash de canette d’exportation de matériau

### Crème glacée 0.1.0-bêta

*(Publié Le 17 Octobre 2018)*

**Ajouté :**

* Fusion matériau avec 4 types de fusion (Fusion Height, Fusion échantillon, Fusion Courbure, Fusion AO)
* Introduire un mécanisme de mise en cache pour optimiser les recalculs de pile de calques
* Sélection automatique d’un matériau dans Inspire s’il est présent dans le viewport
* Format normal centralisé dans le panneau Paramètres de Matériau
* Commandes de widgets de recadrage et de Répétition (-90xB0,+90xB0, créer un carré,...) nettoyage
* Nouveau filtre de Snow

**Fixe :**

* Nettoyage de l’interface utilisateur du panneau
* Le viewport scintille lors du redimensionnement des fenêtres et des panneaux
* Pile de calques non recalculée lors de l’enregistrement
* La dénomination des actifs dans l’interface utilise des libellés au lieu de noms de graphe

**Problèmes Connus :**

* Lissage étiré en changeant rapidement la visibilité du calque
* Le focus réinitialise l’angle de Caméra
