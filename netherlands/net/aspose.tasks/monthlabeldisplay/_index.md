---
title: "Enum MonthLabelDisplay"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.MonthLabelDisplay enum. Geeft aan hoe het maandlabel wordt weergegeven"
type: docs
weight: 1060
url: /nl/net/aspose.tasks/monthlabeldisplay/
---
## MonthLabelDisplay enumeration

Specificeert hoe het maandlabel wordt weergegeven.

```csharp
public enum MonthLabelDisplay
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Mo | `0` | Stelt de lijst Maanden in MS Project in als mo. |
| Mon | `1` | Stelt de lijst Maanden in MS Project in als mon. |
| Month | `2` | Stelt de lijst Maanden in MS Project in als month. |

## Voorbeelden

Toont hoe het maandlabel van de weergaveopties van het project in te stellen (case 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// stel in hoe het maandlabel wordt weergegeven
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mo;

// ...
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


