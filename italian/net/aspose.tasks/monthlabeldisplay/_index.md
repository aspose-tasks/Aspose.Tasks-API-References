---
title: "Enum MonthLabelDisplay"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.MonthLabelDisplay enum. Specifica come viene visualizzata l'etichetta del mese."
type: docs
weight: 1060
url: /it/net/aspose.tasks/monthlabeldisplay/
---
## MonthLabelDisplay enumeration

Specifica come viene visualizzata l'etichetta del mese.

```csharp
public enum MonthLabelDisplay
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Mo | `0` | Imposta l'elenco dei mesi in MS Project come mo. |
| Mon | `1` | Imposta l'elenco dei mesi in MS Project come mon. |
| Month | `2` | Imposta l'elenco dei mesi in MS Project come month. |

## Esempi

Mostra come impostare l'etichetta del mese nelle opzioni di visualizzazione del progetto (caso 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// imposta come viene visualizzata l'etichetta del mese
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mo;

// ...
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


