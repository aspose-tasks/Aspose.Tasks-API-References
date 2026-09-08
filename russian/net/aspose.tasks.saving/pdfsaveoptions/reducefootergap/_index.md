---
title: "PdfSaveOptions.ReduceFooterGap"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PdfSaveOptions. Получает или задает значение, указывающее, следует ли уменьшить зазор между последней задачей и нижним колонтитулом."
type: docs
weight: 80
url: /ru/net/aspose.tasks.saving/pdfsaveoptions/reducefootergap/
---
## PdfSaveOptions.ReduceFooterGap property

Получает или задает значение, указывающее, следует ли уменьшить зазор между последней задачей и нижним колонтитулом.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Примеры

Показывает, как задать значение, указывающее, следует ли уменьшить зазор между последней задачей и нижним колонтитулом в PDF‑файлах.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions { ReduceFooterGap = true, PageSize = PageSize.A0, Timescale = Timescale.Days };

project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.pdf", options);
```

### См. также

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


