---
title: "PrimaveraDbReader"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en läsare för att läsa projektinformation från Primavera DB"
type: docs
weight: 200
url: /sv/java/com.aspose.tasks/primaveradbreader/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.PrimaveraBaseReader](../../com.aspose.tasks/primaverabasereader)
```
public final class PrimaveraDbReader extends PrimaveraBaseReader
```

Representerar en läsare för att läsa projektinformation från Primavera DB
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [PrimaveraDbReader(PrimaveraDbSettings dbSettings)](#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-) | Initierar en ny instans av klassen [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [loadProject(int projectUid)](#loadProject-int-) | Laddar projektet med den angivna unika identifieraren. |
### PrimaveraDbReader(PrimaveraDbSettings dbSettings) {#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-}
```
public PrimaveraDbReader(PrimaveraDbSettings dbSettings)
```


Initierar en ny instans av klassen [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dbSettings | [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) | Inställningar som anger hur man ansluter till Primavera DB. |

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
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier read from Primavera DB. Null if project doesn't exist.
