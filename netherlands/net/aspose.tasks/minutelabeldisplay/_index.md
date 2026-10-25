---
title: "Enum MinuteLabelDisplay"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.MinuteLabelDisplay enum. Specificeert hoe het minutenlabel wordt weergegeven."
type: docs
weight: 1030
url: /nl/net/aspose.tasks/minutelabeldisplay/
---
## MinuteLabelDisplay enumeration

Specificeert hoe het minutenlabel wordt weergegeven.

```csharp
public enum MinuteLabelDisplay
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| M | `0` | Stelt de Minuten‑lijst in MS Project in op m. |
| Min | `1` | Stelt de Minuten‑lijst in MS Project in op min. |
| Minute | `2` | Stelt de Minuten‑lijst in MS Project in op minute. |

## Voorbeelden

Toont hoe het minutenlabel van de weergave‑opties van het project in te stellen (case 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// stel in hoe het minutenlabel wordt weergegeven
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.M;

// ...
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


