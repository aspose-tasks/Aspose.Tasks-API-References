---
title: "Enum HourLabelDisplay"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.HourLabelDisplay enum. Specificeert hoe het uurlabel wordt weergegeven"
type: docs
weight: 820
url: /nl/net/aspose.tasks/hourlabeldisplay/
---
## HourLabelDisplay enumeration

Specificeert hoe het uurlabel wordt weergegeven.

```csharp
public enum HourLabelDisplay
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| H | `0` | "h" label. |
| Hr | `1` | "hr" label. |
| Hour | `2` | "hour(s)" label. |

## Voorbeelden

Toont hoe het uurlabel van de weergaveopties van een project ingesteld wordt (case 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// stel in hoe het uurlabel wordt weergegeven
project.DisplayOptions.HourLabel = HourLabelDisplay.H;

// ...
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


