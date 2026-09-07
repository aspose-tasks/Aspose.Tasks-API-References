---
title: "PrimaveraSaveOptions.PrimaveraSaveOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore PrimaveraSaveOptions. Inizializza una nuova istanza della classe PrimaveraSaveOptions"
type: docs
weight: 10
url: /it/net/aspose.tasks.saving/primaverasaveoptions/primaverasaveoptions/
---
## PrimaveraSaveOptions constructor

Inizializza una nuova istanza della classe [`PrimaveraSaveOptions`](../).

```csharp
public PrimaveraSaveOptions()
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


