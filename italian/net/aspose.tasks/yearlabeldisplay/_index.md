---
title: "Enum YearLabelDisplay"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.YearLabelDisplay. Specifica come viene visualizzata l'etichetta dell'anno."
type: docs
weight: 3680
url: /it/net/aspose.tasks/yearlabeldisplay/
---
## YearLabelDisplay enumeration

Specifica come viene visualizzata l'etichetta dell'anno.

```csharp
public enum YearLabelDisplay
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Y | `0` | Imposta l'elenco Anni in MS Project come mo. |
| Yr | `1` | Imposta l'elenco Anni in MS Project come mon. |
| Year | `2` | Imposta l'elenco degli anni in MS Project come mese. |

## Esempi

Mostra come impostare l'etichetta dell'anno nelle opzioni di visualizzazione del progetto (caso 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// imposta come viene visualizzata l'etichetta dell'anno
project.DisplayOptions.YearLabel = YearLabelDisplay.Y;

// ...
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


