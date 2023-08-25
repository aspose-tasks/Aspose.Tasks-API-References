---
title: PrimaveraBaseReader
second_title: Aspose.Tasks for Java API Reference
description: Represents a base reader which can be used to read Project UIDs from multi project Primavera XER or XML files.
type: docs
weight: 185
url: /java/com.aspose.tasks/primaverabasereader/
---

**Inheritance:**
java.lang.Object
```
public abstract class PrimaveraBaseReader
```

Represents a base reader which can be used to read Project UIDs from multi project Primavera XER or XML files.
## Methods

| Method | Description |
| --- | --- |
| [getProjectUids()](#getProjectUids--) | Return a list of the projects' unique identifiers. |
| [loadProject(int projectUid)](#loadProject-int-) | Loads the project with the specified unique identifier. |
### getProjectUids() {#getProjectUids--}
```
public final List<Integer> getProjectUids()
```


Return a list of the projects' unique identifiers.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - List of projects' unique identifiers.
### loadProject(int projectUid) {#loadProject-int-}
```
public final Project loadProject(int projectUid)
```


Loads the project with the specified unique identifier.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| projectUid | int | Unique identifier of the project to load. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier from the specified multi project file. Null if project doesn't exist.
