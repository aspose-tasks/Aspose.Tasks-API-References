---
title: "PrimaveraBaseReader"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en basläsare som kan användas för att läsa projekt-UID:n från multipla Primavera XER- eller XML-filer."
type: docs
weight: 196
url: /sv/java/com.aspose.tasks/primaverabasereader/
---

**Inheritance:**
java.lang.Object
```
public abstract class PrimaveraBaseReader
```

Representerar en basläsare som kan användas för att läsa projekt-UID:n från multipla Primavera XER- eller XML-filer.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getProjectInfos()](#getProjectInfos--) | Returnerar en lista med projektets korta informationsobjekt. |
| [getProjectUids()](#getProjectUids--) | Returnerar en lista med projektens unika identifierare. |
| [loadProject(int projectUid)](#loadProject-int-) | Laddar projektet med den angivna unika identifieraren. |
### getProjectInfos() {#getProjectInfos--}
```
public final List<PrimaveraProjectInfo> getProjectInfos()
```


Returnerar en lista med projektets korta informationsobjekt.

**Returns:**
java.util.List&lt;com.aspose.tasks.PrimaveraProjectInfo&gt; - en lista med projektets korta informationsobjekt
### getProjectUids() {#getProjectUids--}
```
public final List<Integer> getProjectUids()
```


Returnerar en lista med projektens unika identifierare.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - lista med projektens unika identifierare.
### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


Laddar projektet med den angivna unika identifieraren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| projectUid | int | Unik identifierare för projektet som ska laddas. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier from the specified multi project file. Null if project doesn't exist.
