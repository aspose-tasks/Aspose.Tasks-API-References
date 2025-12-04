---
title: PrimaveraDbReader
second_title: Aspose.Tasks for Java API Reference
description: Represents a reader to read Project Info from Primavera DB
type: docs
weight: 199
url: /java/com.aspose.tasks/primaveradbreader/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.PrimaveraBaseReader](../../com.aspose.tasks/primaverabasereader)
```
public final class PrimaveraDbReader extends PrimaveraBaseReader
```

Represents a reader to read Project Info from Primavera DB
## Constructors

| Constructor | Description |
| --- | --- |
| [PrimaveraDbReader(PrimaveraDbSettings dbSettings)](#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-) | Initializes a new instance of the [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader) class. |
## Methods

| Method | Description |
| --- | --- |
| [loadProject(int projectUid)](#loadProject-int-) | Loads the project with the specified unique identifier. |
### PrimaveraDbReader(PrimaveraDbSettings dbSettings) {#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-}
```
public PrimaveraDbReader(PrimaveraDbSettings dbSettings)
```


Initializes a new instance of the [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dbSettings | [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) | Settings that specify how to connect to Primavera DB. |

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
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier read from Primavera DB. Null if project doesn't exist.
