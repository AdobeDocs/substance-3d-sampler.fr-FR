---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-sampler/scripting-and-development/create-a-plugin-with-python-and-qml.html"
breadcrumb-title: ''
description: Découvrez comment créer des plug-ins avec Python et XML pour Substance 3D Sampler afin de créer des interfaces utilisateur personnalisées et d’étendre les fonctionnalités.
helpx_creative_field: ""
helpx_description: Sampler > Scripting and Development > Create a Plugin with Python and QML
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Création d’un plug-in avec Python et XML
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 0%

---


# Création d’un plug-in avec Python et XML

Ce guide décrit comment créer un plug-in d’enregistrement automatique simple avec Python et XML.

## Structure du plug-in

Les plug-ins Sampler nécessitent au moins un fichier Python et QML pour être importés, mais d’autres fichiers peuvent également être inclus, tels que les images utilisées pour les icônes dans le panneau des plug-ins. Dans l’exemple ci-dessous, il y a 3 fichiers :

* **autosave.py** contient la logique du plug-in et détermine son fonctionnement.
* **autosave.qml** définit l&#39;apparence du plug-in dans Sampler.
* **autosave.svg** est une image vectorielle utilisée comme icône pour le plug-in.

Une fois que vous avez les fichiers nécessaires pour votre plug-in dans un seul dossier, vous pouvez ajouter le plug-in à Sampler via Édition > Préférences > Plug-ins et scripts. Pour en savoir plus sur la gestion des plug-ins, rendez-vous [ici](manage-installed-plugins-and-scripts.md).

## Python

Le code ci-dessous est le fichier python complet pour le plug-in d’enregistrement automatique. Vous trouverez ci-dessous une brève description de ce que fait le code, mais le code inclut également des commentaires avec plus d’informations :

1. Importer les modules pertinents.
   1. Qt est une boîte à outils d’interface utilisateur graphique multiplateforme. Les modules QtcCore, QtQml et QtQuick nous permettent de communiquer entre autosave.py et autosave.qml.
1. Définissez une méthode **save()** qui enregistre le projet toutes les X minutes.
1. Créez une classe d’enregistrement automatique. Cette classe spécifie comment la méthode **save()** se connecte à l&#39;interface utilisateur du plug-in afin que les paramètres puissent modifier le comportement du plug-in
1. Définissez une méthode **register\_qml\_type()** qui effectue la configuration du plug-in.
1. Appelez le plug-in depuis Sampler.

### autosave.py

```
## Import QT & QML modules to create the UI

from PySide2 import QtCore, QtQml, QtQuick 

## Import Sampler API

import substance_sampler as ssa 

## Import other modules for this specific example

import datetime 

import os 

import threading 

 

 

## Save the project every X minutes

def save(interval): 

    global t 

    ssa.save_project() 

    if ssa.save_project(): 

        now = datetime.datetime.now() 

        print("Autosave: %d:%d:%d" % (now.hour, now.minute, now.second)) 

    t = threading.Timer(interval, save, [interval]) 

    t.start() 

 

 

t = None 

 

 

## Declare the API AutoSave

class AutoSave(QtQuick.QQuickItem): 

    def __init__(self, parent=None): 

        super(AutoSave, self).__init__(parent) 

 

## Declare a first API function

## This function can be called from the QML file

## with 2 arguments, one string and one integer

    @QtCore.Slot(str, int) 

    def start_auto_save(self, default_path, interval): 

        if not ssa.save_project(): 

            ssa.save_project_as(os.path.join(default_path, "autosave.ssa")) 

        global t 

        t = threading.Timer(10, save, [interval]) 

        t.start() 

        print("Launch Autosave") 

 

## Second function of the API

## With no argument

    @QtCore.Slot(None) 

    def stop_auto_save(self): 

        global t 

        t.cancel() 

        print("Stop Autosave") 

 

 

## Function to declare the API and the panel

## First argument is Python class of your API

## Second argument is name of the API you will use in the QML file

## Third and fourth is the API version. In this case, 1.0

## Last is the name of the panel in Sampler UI

def register_qml_type(): 

    QtQml.qmlRegisterType(AutoSave, "AutoSave", 1, 0, "AutoSave") 

 

 

## Execute the plugin in Sampler UI thread

ssa.run_in_main_thread(register_qml_type)
```


## QML

Le fichier XML définit l’interface utilisateur du plug-in. QML est l’acronyme de Qt Markup Language. Il se comporte de la même manière que d’autres langages de balisage tels que HTML et XML. Vous pouvez [en savoir plus sur QML ici](https://doc.qt.io/qt-6/qmlapplications.html#:~:text=QML%20is%20a%20user%20interface%20specification%20and%20programming,imperative%20JavaScript%20expressions%20combined%20with%20dynamic%20property%20bindings.).

La structure générale du fichier autosave.qml est la suivante :

1. Importer des modules.
   1. Les modules Qt importés sont nécessaires pour les éléments d’interface utilisateur utilisés dans le fichier.
   1. La classe API d&#39;enregistrement automatique créée dans **autosave.py** est également importée. Le fichier QML référence cette classe à la ligne 20.
1. Créez des variables qui doivent être suivies.
   1. **autoSaveFolder** est le dossier dans lequel le fichier Sampler sera enregistré automatiquement.
   1. **durée** correspond au temps en secondes entre les enregistrements automatiques.
   1. **textColor** est utilisé afin que la couleur du texte dans l&#39;interface utilisateur du plug-in puisse être mise à jour en un seul endroit.
1. Instanciation de l’API Python
1. Définissez l’interface utilisateur.
   1. Cela inclut les hooks de l&#39;API Python créés dans **autosave.py**. Par exemple :
      1. La ligne 47 met à jour la valeur de variable **minutage** dans le fichier QML chaque fois que l&#39;élément « Enregistrement automatique toutes les (min) : » est modifié.
      1. La ligne 64 appelle la fonction **start\_auto\_save** à partir de l&#39;API et passe les variables **timing** et **autoSaveFolder** en tant que paramètres.
1. Créez une méthode pour nettoyer le chemin de fichier par défaut.

### autosave.qml

```
/* 

Import Qt modules to design the UI 

https://doc.qt.io/qt-5/qtqml-syntax-basics.html 

*/ 

import QtQuick 2.15 

import QtQuick.Controls 2.15 

import Qt.labs.platform 1.1 

import AutoSave 1.0 // Import API defined in the Python file 

 

Rectangle { 

  id: root 

  anchors.fill: parent 

  color: "#333333" 

 

  property var autoSaveFolder: removeQmlFilePathPrefix(StandardPaths.writableLocation(StandardPaths.DocumentsLocation)) 

  property var timing: 300 

  property var textColor: "#b3b3b3" 

 

  AutoSave { 

      id: api // Instantiate the Python API 

  } 

 

  Column { 

    id: controls 

    anchors.top: parent.top + 10 

    anchors.left: parent.left + 10 

    anchors.right: parent.right 

    width: parent.width 

    spacing: 20 

    leftPadding: 10 

    topPadding: 10 

 

    Column { 

        spacing: 5 

        Text { 

            id: timingTitle 

            text: "Autosave every (min): " 

            color: root.textColor 

        } 

        SpinBox { 

            id: timingControl 

            from: 1 

            to: 10 

            stepSize: 1 

            value: 5 

 

            onValueModified: ()=>{ 

                root.timing = timingControl.value * 60 

            } 

        } 

    } 

    Row { 

        Text { 

            text: "Off" 

            color: root.textColor 

            anchors.verticalCenter: toggle.verticalCenter 

        } 

        Switch { 

            id: toggle 

            checked: false 

 

            onClicked: ()=>{ 

                if (checked === true) { 

                    api.start_auto_save(root.autoSaveFolder, root.timing) // Call a function of the API with 2 arguments 

                } 

                else if (checked === false) { 

                    api.stop_auto_save() // Call a function of the API 

                } 

            } 

        } 

        Text { 

            text: "On" 

            color: root.textColor 

            anchors.verticalCenter: toggle.verticalCenter 

        } 

 

    } 

    Column { 

        spacing: 5 

        Text { 

            text: "Default Autosave Path" 

            color: root.textColor 

            } 

        Row { 

            id: folderInput 

            TextField { 

                id: folderText 

                text: root.autoSaveFolder 

                readOnly: true 

            } 

            Button { 

                id: folderSelection 

                text: qsTr("...") 

                width: 40 

                onClicked: ()=>{ 

                    folderDialog.open() 

                    } 

            } 

        } 

    } 

 

    FolderDialog { 

        id: folderDialog 

 

        onAccepted: ()=>{ 

            root.autoSaveFolder = removeQmlFilePathPrefix(folderDialog.currentFolder) 

        } 

    } 

 

  } 

      function qmlFilePathPrefix() { 

        if (Qt.platform.os === "windows") { 

            return "file:///" 

        } 

        return "file://" 

    } 

    function removeQmlFilePathPrefix(filePath) { 

        var prefix = qmlFilePathPrefix() 

        return filePath.toString().replace(prefix, '') 

    } 

}
```


## SVG

Vous avez peut-être remarqué que **autosave.svg** n&#39;est pas explicitement appelé ou mentionné dans **autosave.py** ou **autosave.qml**. En effet, Sampler recherche un fichier de SVG portant le même nom que le fichier PY et l’utilise automatiquement comme icône de plug-in.

>[!NOTE]
>
> Si votre dossier de plug-in contient un SVG dont le nom de fichier ne correspond pas au fichier PY du plug-in, votre plug-in n’inclut pas d’icône. Cela peut donner l’impression que votre plug-in n’apparaît pas dans l’interface utilisateur de Sampler. Si c’est le cas, déplacez votre curseur sur la barre de droite de Sampler pour mettre en surbrillance votre plug-in.
> 
> Votre navigateur ne prend pas en charge l’élément vidéo HTML5

Si votre dossier de plug-in ne contient pas de fichier de SVG, une icône de plug-in par défaut sera utilisée à la place.

Vous trouverez ci-dessous un exemple de SVG que vous pouvez utiliser pour le plug-in d’enregistrement automatique créé ci-dessus.

[autosave.svg](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/sadoc/files/234455541/234455542/1/1662460696349/autosave.svg)

## Limitations du plug-in d’enregistrement automatique

Le plug-in d’enregistrement automatique créé ci-dessus fonctionne, mais il n’est pas parfait. Par exemple, l’ajustement de l’intervalle d’enregistrement automatique après l’activation de l’enregistrement automatique ne modifie pas réellement le temps entre les enregistrements automatiques. Vous devrez désactiver et réactiver l’enregistrement automatique pour que la valeur de l’interface utilisateur soit envoyée à l’API.

Si vous travaillez avec Python et XML ensemble pour la première fois, corriger ce bogue est un moyen utile de mieux comprendre comment les différentes parties du plug-in communiquent entre elles.
