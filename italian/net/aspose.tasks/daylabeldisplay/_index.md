---
title: "Enum DayLabelDisplay"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.DayLabelDisplay enum. Specifica come viene visualizzata l'etichetta del giorno"
type: docs
weight: 440
url: /it/net/aspose.tasks/daylabeldisplay/
---
## DayLabelDisplay enumeration

Specifica come viene visualizzata l'etichetta del giorno.

```csharp
public enum DayLabelDisplay
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| D | `0` | Imposta l'elenco dei giorni in MS Project come d. |
| Dy | `1` | Imposta l'elenco dei giorni in MS Project come dy. |
| Day | `2` | Imposta l'elenco dei giorni in MS Project come day. |

## Esempi

Mostra come impostare l'etichetta del giorno nelle opzioni di visualizzazione del progetto (caso 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// imposta come viene visualizzata l'etichetta del giorno
project.DisplayOptions.DayLabel = DayLabelDisplay.D;

// ...
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


