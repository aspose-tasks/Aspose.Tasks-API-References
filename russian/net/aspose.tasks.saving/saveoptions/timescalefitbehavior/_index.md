---
title: "SaveOptions.TimescaleFitBehavior"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает поведение, определяющее, как выровнять правый конец шкалы времени с концом страницы."
type: docs
weight: 210
url: /ru/net/aspose.tasks.saving/saveoptions/timescalefitbehavior/
---
## SaveOptions.TimescaleFitBehavior property

Получает или задает поведение, определяющее, как выравнивать правый конец шкалы времени с концом страницы.

```csharp
public TimescaleFitBehavior TimescaleFitBehavior { get; set; }
```

## Примеры

Показывает, как использовать TimescaleFitBehavior, чтобы шкала времени диаграммы Ганта соответствовала концу последней страницы.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### См. также

* enum [TimescaleFitBehavior](../../../aspose.tasks.visualization/timescalefitbehavior/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


