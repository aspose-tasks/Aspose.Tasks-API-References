---
title: "HtmlSaveOptions.ReduceFooterGap"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство HtmlSaveOptions. Получает или задает значение, указывающее, следует ли уменьшить зазор между последней задачей и нижним колонтитулом."
type: docs
weight: 150
url: /ru/net/aspose.tasks.saving/htmlsaveoptions/reducefootergap/
---
## HtmlSaveOptions.ReduceFooterGap property

Получает или задает значение, указывающее, следует ли уменьшить зазор между последней задачей и нижним колонтитулом.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Примеры

Показывает, как установить значение, указывающее, следует ли уменьшить зазор между последней задачей и нижним колонтитулом в файлах HTML‑вывода.

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

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


