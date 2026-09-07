---
title: "PrimaveraSaveOptions.ActivityIdIncrement"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PrimaveraSaveOptions. Ottiene o imposta l'incremento utilizzato nella rinumerazione degli ID attività"
type: docs
weight: 20
url: /it/net/aspose.tasks.saving/primaverasaveoptions/activityidincrement/
---
## PrimaveraSaveOptions.ActivityIdIncrement property

Ottiene o imposta l'incremento utilizzato nella ridenominazione degli ID delle attività.

```csharp
public int ActivityIdIncrement { get; set; }
```

## Esempi

Mostra come lavorare con &lt;see cref="Aspose.Tasks.Saving.PrimaveraSaveOptions" /&gt;.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// crea le opzioni di salvataggio Primavera e personalizzale
var options = new PrimaveraSaveOptions
                  {
                      // definisci prefisso e suffisso di un'attività
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // controlla la ridenominazione delle attività
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### Vedi anche

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)


