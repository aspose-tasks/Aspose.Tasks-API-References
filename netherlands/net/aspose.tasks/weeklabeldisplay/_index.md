---
title: "Enum WeekLabelDisplay"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.WeekLabelDisplay enum. Specificeert hoe het weeklabel wordt weergegeven"
type: docs
weight: 3560
url: /nl/net/aspose.tasks/weeklabeldisplay/
---
## WeekLabelDisplay enumeration

Specificeert hoe het weeklabel wordt weergegeven.

```csharp
public enum WeekLabelDisplay
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| W | `0` | "w" label. |
| Wk | `1` | "wk" label. |
| Week | `2` | "week" label. |

## Voorbeelden

Toont hoe het weeklabel van de weergaveopties van een project in te stellen (case 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// stel in hoe het weeklabel wordt weergegeven
project.DisplayOptions.WeekLabel = WeekLabelDisplay.W;

// ...
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


