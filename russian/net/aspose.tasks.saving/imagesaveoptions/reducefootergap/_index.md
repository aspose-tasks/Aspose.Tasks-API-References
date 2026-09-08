---
title: "ImageSaveOptions.ReduceFooterGap"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ImageSaveOptions. Получает или задает значение, указывающее, следует ли уменьшить зазор между последней задачей и нижним колонтитулом"
type: docs
weight: 80
url: /ru/net/aspose.tasks.saving/imagesaveoptions/reducefootergap/
---
## ImageSaveOptions.ReduceFooterGap property

Получает или задает значение, указывающее, следует ли уменьшить зазор между последней задачей и нижним колонтитулом.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Примеры

Показывает, как установить значение, указывающее, следует ли уменьшить зазор между последней задачей и нижним колонтитулом.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// Используйте свойство ReduceFooterGap, чтобы уменьшить зазор между списком задач и нижним колонтитулом
var imageSaveOptions = new ImageSaveOptions(SaveFileFormat.Png)
                           {
                               ReduceFooterGap = true, /* set to true */ 
                               RenderToSinglePage = false,
                               PageSize = PageSize.A0,
                               Timescale = Timescale.Days
                           };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.png", imageSaveOptions);
```

### См. также

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


