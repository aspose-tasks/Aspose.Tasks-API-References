---
title: "PrimaveraBaseReader"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een basislezer voor die kan worden gebruikt om project-UID's te lezen uit multi-project Primavera XER- of XML-bestanden."
type: docs
weight: 196
url: /nl/java/com.aspose.tasks/primaverabasereader/
---

**Inheritance:**
java.lang.Object
```
public abstract class PrimaveraBaseReader
```

Stelt een basislezer voor die kan worden gebruikt om project-UID's te lezen uit multi-project Primavera XER- of XML-bestanden.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getProjectInfos()](#getProjectInfos--) | Retourneer een lijst met de korte informatieobjecten van het project. |
| [getProjectUids()](#getProjectUids--) | Retourneer een lijst met de unieke identificatoren van de projecten. |
| [loadProject(int projectUid)](#loadProject-int-) | Laadt het project met de opgegeven unieke identifier. |
### getProjectInfos() {#getProjectInfos--}
```
public final List<PrimaveraProjectInfo> getProjectInfos()
```


Retourneer een lijst met de korte informatieobjecten van het project.

**Returns:**
java.util.List&lt;com.aspose.tasks.PrimaveraProjectInfo&gt; - een lijst met de korte informatieobjecten van het project
### getProjectUids() {#getProjectUids--}
```
public final List<Integer> getProjectUids()
```


Retourneer een lijst met de unieke identificatoren van de projecten.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - Lijst met de unieke identificatoren van de projecten.
### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


Laadt het project met de opgegeven unieke identifier.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| projectUid | int | Unieke identifier van het project om te laden. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier from the specified multi project file. Null if project doesn't exist.
