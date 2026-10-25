---
title: "Enum DayLabelDisplay"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.DayLabelDisplay enum. Specificeert hoe het daglabel wordt weergegeven"
type: docs
weight: 440
url: /nl/net/aspose.tasks/daylabeldisplay/
---
## DayLabelDisplay enumeration

Specificeert hoe het daglabel wordt weergegeven.

```csharp
public enum DayLabelDisplay
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| D | `0` | Stelt de dagenlijst in MS Project in als d. |
| Dy | `1` | Stelt de dagenlijst in MS Project in als dy. |
| Day | `2` | Stelt de dagenlijst in MS Project in als day. |

## Voorbeelden

Toont hoe het daglabel van de weergaveopties van een project in te stellen (case 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// stel in hoe het daglabel wordt weergegeven
project.DisplayOptions.DayLabel = DayLabelDisplay.D;

// ...
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


