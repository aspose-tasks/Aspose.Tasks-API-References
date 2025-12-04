---
title: PrimaveraBaseReader
second_title: Aspose.Tasks for Java API Reference
description: Represents a base reader which can be used to read Project UIDs from multi project Primavera XER or XML files.
type: docs
weight: 195
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
| [getProjectInfos()](#getProjectInfos--) | Return a list of the project's short info objects. |
| [getProjectUids()](#getProjectUids--) | Return a list of the projects' unique identifiers. |
| [loadProject(int projectUid)](#loadProject-int-) | Loads the project with the specified unique identifier. |
### getProjectInfos() {#getProjectInfos--}
```
public final List<PrimaveraProjectInfo> getProjectInfos()
```


Return a list of the project's short info objects.

**Returns:**
java.util.List&lt;com.aspose.tasks.PrimaveraProjectInfo&gt; - a list of the project's short info objects
### getProjectUids() {#getProjectUids--}
```
public final List<Integer> getProjectUids()
```


Return a list of the projects' unique identifiers.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - List of projects' unique identifiers.
### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


Loads the project with the specified unique identifier.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| projectUid | int | Unique identifier of the project to load. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier from the specified multi project file. Null if project doesn't exist.
