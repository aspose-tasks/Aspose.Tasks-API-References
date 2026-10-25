---
title: "PrimaveraDbReader"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een lezer voor om projectinformatie uit de Primavera-database te lezen."
type: docs
weight: 200
url: /nl/java/com.aspose.tasks/primaveradbreader/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.PrimaveraBaseReader](../../com.aspose.tasks/primaverabasereader)
```
public final class PrimaveraDbReader extends PrimaveraBaseReader
```

Stelt een lezer voor om projectinformatie uit de Primavera-database te lezen.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [PrimaveraDbReader(PrimaveraDbSettings dbSettings)](#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-) | Initialiseert een nieuw exemplaar van de klasse [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader). |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [loadProject(int projectUid)](#loadProject-int-) | Laadt het project met de opgegeven unieke identifier. |
### PrimaveraDbReader(PrimaveraDbSettings dbSettings) {#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-}
```
public PrimaveraDbReader(PrimaveraDbSettings dbSettings)
```


Initialiseert een nieuw exemplaar van de klasse [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dbSettings | [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) | Instellingen die specificeren hoe verbinding te maken met Primavera DB. |

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
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier read from Primavera DB. Null if project doesn't exist.
