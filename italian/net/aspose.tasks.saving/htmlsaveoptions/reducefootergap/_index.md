---
title: "HtmlSaveOptions.ReduceFooterGap"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "HtmlSaveOptions property. Ottiene o imposta un valore che indica se lo spazio tra l'ultima attività e il piè di pagina deve essere ridotto"
type: docs
weight: 150
url: /it/net/aspose.tasks.saving/htmlsaveoptions/reducefootergap/
---
## HtmlSaveOptions.ReduceFooterGap property

Ottiene o imposta un valore che indica se lo spazio tra l'ultima attività e il piè di pagina deve essere ridotto.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Esempi

Mostra come impostare un valore che indica se lo spazio tra l'ultima attività e il piè di pagina deve essere ridotto nei file di output HTML.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      ReduceFooterGap = true,
                      IncludeProjectNameInPageHeader = false,
                      IncludeProjectNameInTitle = false,
                      PageSize = PageSize.A0,
                      Timescale = Timescale.Days
                  };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.html", options);
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


