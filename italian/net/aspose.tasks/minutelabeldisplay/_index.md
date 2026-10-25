---
title: "Enum MinuteLabelDisplay"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.MinuteLabelDisplay. Specifica come viene visualizzata l'etichetta dei minuti."
type: docs
weight: 1030
url: /it/net/aspose.tasks/minutelabeldisplay/
---
## MinuteLabelDisplay enumeration

Specifica come viene visualizzata l'etichetta dei minuti.

```csharp
public enum MinuteLabelDisplay
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| M | `0` | Imposta l'elenco dei minuti in MS Project come m. |
| Min | `1` | Imposta l'elenco dei minuti in MS Project come min. |
| Minute | `2` | Imposta l'elenco dei minuti in MS Project come minute. |

## Esempi

Mostra come impostare l'etichetta dei minuti nelle opzioni di visualizzazione del progetto (caso 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// imposta come viene visualizzata l'etichetta dei minuti
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.M;

// ...
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


