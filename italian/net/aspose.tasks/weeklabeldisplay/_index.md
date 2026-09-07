---
title: "Enum WeekLabelDisplay"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.WeekLabelDisplay enum. Specifica come viene visualizzata l'etichetta della settimana"
type: docs
weight: 3560
url: /it/net/aspose.tasks/weeklabeldisplay/
---
## WeekLabelDisplay enumeration

Specifica come viene visualizzata l'etichetta della settimana.

```csharp
public enum WeekLabelDisplay
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| W | `0` | \"w\" etichetta. |
| Wk | `1` | \"wk\" etichetta. |
| Week | `2` | \"week\" etichetta. |

## Esempi

Mostra come impostare l'etichetta della settimana nelle opzioni di visualizzazione del progetto (caso 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// imposta come viene visualizzata l'etichetta della settimana
project.DisplayOptions.WeekLabel = WeekLabelDisplay.W;

// ...
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


