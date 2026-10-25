---
title: "ImageSaveOptions.ReduceFooterGap"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ImageSaveOptions. Ottiene o imposta un valore che indica se lo spazio tra l'ultimo compito e il piè di pagina deve essere ridotto"
type: docs
weight: 80
url: /it/net/aspose.tasks.saving/imagesaveoptions/reducefootergap/
---
## ImageSaveOptions.ReduceFooterGap property

Ottiene o imposta un valore che indica se lo spazio tra l'ultima attività e il piè di pagina deve essere ridotto.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Esempi

Mostra come impostare un valore che indica se lo spazio tra l'ultimo compito e il piè di pagina deve essere ridotto.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// Usa la proprietà ReduceFooterGap per ridurre lo spazio tra l'elenco dei compiti e il piè di pagina
var imageSaveOptions = new ImageSaveOptions(SaveFileFormat.Png)
                           {
                               ReduceFooterGap = true, /* set to true */ 
                               RenderToSinglePage = false,
                               PageSize = PageSize.A0,
                               Timescale = Timescale.Days
                           };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.png", imageSaveOptions);
```

### Vedi anche

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


