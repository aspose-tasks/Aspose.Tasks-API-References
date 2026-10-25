---
title: "Enum HourLabelDisplay"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.HourLabelDisplay. Specifica come viene visualizzata l'etichetta dell'ora"
type: docs
weight: 820
url: /it/net/aspose.tasks/hourlabeldisplay/
---
## HourLabelDisplay enumeration

Specifica come viene visualizzata l'etichetta dell'ora.

```csharp
public enum HourLabelDisplay
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| H | `0` | "h" etichetta. |
| Hr | `1` | "hr" etichetta. |
| Hour | `2` | "hour(s)" etichetta. |

## Esempi

Mostra come impostare l'etichetta dell'ora nelle opzioni di visualizzazione del progetto (caso 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// imposta come viene visualizzata l'etichetta dell'ora
project.DisplayOptions.HourLabel = HourLabelDisplay.H;

// ...
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


