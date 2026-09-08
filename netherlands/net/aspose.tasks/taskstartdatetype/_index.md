---
title: "Enum TaskStartDateType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.TaskStartDateType enum. Specificeert het type van de startdatum van een taak"
type: docs
weight: 2450
url: /nl/net/aspose.tasks/taskstartdatetype/
---
## TaskStartDateType enumeration

Specificeert het type van de startdatum van een taak.

```csharp
public enum TaskStartDateType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Undefined | `-1` | De waarde van het veld was niet gedefinieerd in het oorspronkelijke projectbestand. |
| ProjectStartDate | `0` | Project startdatum |
| CurrentDate | `1` | Huidige datum |

## Opmerkingen

Tijdens het exporteren naar XML worden de Undefined‑waarden uit de resulterende XML verwijderd.

## Voorbeelden

Toont hoe de standaard startdatum van een taak in te stellen als 'CurrentDate'.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


