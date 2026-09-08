---
title: "SaveOptions.CustomPageSize"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает пользовательский размер страницы в пунктах (1 пункт = 1/72 дюйма)."
type: docs
weight: 20
url: /ru/net/aspose.tasks.saving/saveoptions/custompagesize/
---
## SaveOptions.CustomPageSize property

Получает или задает пользовательский размер страницы в пунктах (1 пункт = 1/72 дюйма).

```csharp
public SizeF CustomPageSize { get; set; }
```

## Примеры

Показано, как задать пользовательский размер страницы при сохранении проекта в PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
options.PresentationFormat = PresentationFormat.GanttChart;
options.CustomPageSize = new SizeF(5.8F * 72, 8.3F * 72);

project.Save(OutDir + "WorkWithCustomPageSize_out.pdf", options);
```

### См. также

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


