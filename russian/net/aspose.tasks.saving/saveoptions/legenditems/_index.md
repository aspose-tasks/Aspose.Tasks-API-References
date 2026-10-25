---
title: "SaveOptions.LegendItems"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает массив PageLegendItem, определяющий, какие полосы следует рендерить в легенде страницы. Если null, рендерятся элементы по умолчанию."
type: docs
weight: 90
url: /ru/net/aspose.tasks.saving/saveoptions/legenditems/
---
## SaveOptions.LegendItems property

Получает или задает массив PageLegendItem, определяющий, какие полосы должны отображаться в легенде страницы. Если null, отображаются элементы по умолчанию.

```csharp
public PageLegendItem[] LegendItems { get; set; }
```

## Примечания

Применяется только при рендеринге представления диаграммы Ганта.

## Примеры

Показывает, как настроить полосы задач в легенде страницы диаграммы Ганта.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.StartDate = project.StartDate;
pdfSaveOptions.EndDate = project.FinishDate;
pdfSaveOptions.PageSize = PageSize.A4;
pdfSaveOptions.LegendDrawingOptions = LegendDrawingOptions.OnEveryPage;
pdfSaveOptions.ViewSettings = project.Views.GetByName("&Gantt Chart");

pdfSaveOptions.LegendItems = new PageLegendItem[]
{
    new PageLegendItem(BarItemType.Task, "Task"),
    new PageLegendItem(BarItemType.ExternalMilestone, "External Milestone"),
    new PageLegendItem(BarItemType.SummaryRollup, "Summary Rollup"),
    new PageLegendItem(BarItemType.InactiveTask, "Inactive Task"),
    new PageLegendItem(BarItemType.ManualSummary, "Manual Summary")
};

project.Save(OutDir + "CustomizePageLegendItems_out.pdf", pdfSaveOptions);
```

### См. также

* class [PageLegendItem](../../../aspose.tasks.visualization/pagelegenditem/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


