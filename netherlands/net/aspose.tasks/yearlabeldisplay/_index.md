---
title: "Enum YearLabelDisplay"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.YearLabelDisplay enum. Specificeert hoe het jaartikett wordt weergegeven"
type: docs
weight: 3680
url: /nl/net/aspose.tasks/yearlabeldisplay/
---
## YearLabelDisplay enumeration

Specificeert hoe het jaartallabel wordt weergegeven.

```csharp
public enum YearLabelDisplay
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Y | `0` | Stelt de jarenlijst in MS Project in als ma. |
| Yr | `1` | Stelt de jarenlijst in MS Project in als ma. |
| Year | `2` | Stelt de jarenlijst in MS Project in als maand. |

## Voorbeelden

Toont hoe je het jaartitel van de weergaveopties van het project instelt (case 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// Stel in hoe het jaartitel wordt weergegeven
project.DisplayOptions.YearLabel = YearLabelDisplay.Y;

// ...
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


