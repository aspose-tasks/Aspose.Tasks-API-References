---
title: "PrimaveraBaseReader"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un lecteur de base pouvant être utilisé pour lire les UID de projet à partir de fichiers Primavera XER ou XML multi-projets."
type: docs
weight: 196
url: /fr/java/com.aspose.tasks/primaverabasereader/
---

**Inheritance:**
java.lang.Object
```
public abstract class PrimaveraBaseReader
```

Représente un lecteur de base pouvant être utilisé pour lire les UID de projet à partir de fichiers Primavera XER ou XML multi-projets.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getProjectInfos()](#getProjectInfos--) | Renvoie une liste des objets d'informations succinctes du projet. |
| [getProjectUids()](#getProjectUids--) | Renvoie une liste des identifiants uniques des projets. |
| [loadProject(int projectUid)](#loadProject-int-) | Charge le projet avec l'identifiant unique spécifié. |
### getProjectInfos() {#getProjectInfos--}
```
public final List<PrimaveraProjectInfo> getProjectInfos()
```


Renvoie une liste des objets d'informations succinctes du projet.

**Returns:**
java.util.List&lt;com.aspose.tasks.PrimaveraProjectInfo&gt; - une liste des objets d'informations succinctes du projet
### getProjectUids() {#getProjectUids--}
```
public final List<Integer> getProjectUids()
```


Renvoie une liste des identifiants uniques des projets.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - Liste des identifiants uniques des projets.
### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


Charge le projet avec l'identifiant unique spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| projectUid | int | Identifiant unique du projet à charger. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier from the specified multi project file. Null if project doesn't exist.
