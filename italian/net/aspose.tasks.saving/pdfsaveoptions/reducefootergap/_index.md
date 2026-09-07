---
title: "PdfSaveOptions.ReduceFooterGap"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PdfSaveOptions. Ottiene o imposta un valore che indica se ridurre lo spazio tra l'ultima attività e il piè di pagina"
type: docs
weight: 80
url: /it/net/aspose.tasks.saving/pdfsaveoptions/reducefootergap/
---
## PdfSaveOptions.ReduceFooterGap property

Ottiene o imposta un valore che indica se lo spazio tra l'ultima attività e il piè di pagina deve essere ridotto.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Esempi

Mostra come impostare un valore che indica se ridurre lo spazio tra l'ultima attività e il piè di pagina nei file PDF di output.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions { ReduceFooterGap = true, PageSize = PageSize.A0, Timescale = Timescale.Days };

project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.pdf", options);
```

### Vedi anche

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


