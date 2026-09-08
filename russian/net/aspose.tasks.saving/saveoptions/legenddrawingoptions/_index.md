---
title: "SaveOptions.LegendDrawingOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает значение, определяющее, как отрисовывать легенду. Значение по умолчанию — LegendDrawingOptions.OnEveryPage"
type: docs
weight: 80
url: /ru/net/aspose.tasks.saving/saveoptions/legenddrawingoptions/
---
## SaveOptions.LegendDrawingOptions property

Получает или задает значение, определяющее, как отрисовывать легенду. Значение по умолчанию — LegendDrawingOptions.OnEveryPage.

```csharp
public LegendDrawingOptions LegendDrawingOptions { get; set; }
```

## Примечания

Применяется только при рендеринге представления диаграммы Ганта.

## Примеры

Показывает, как напечатать легенду на последней странице

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Получить параметры отрисовки легенды из представления
    LegendDrawingOptions = LegendDrawingOptions.AfterLastPage
};

project.Save(OutDir + "LegendOnSeparatePage_out.pdf", options);
```

Показывает, как скрыть легенды страниц.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Укажите LegendDrawingOptions.NoLegend, чтобы скрыть легенды
    LegendDrawingOptions = LegendDrawingOptions.NoLegend
};

project.Save(OutDir + "HideLegendsDuringSave_out.pdf", options);
```

Показывает, как использовать параметр LegendDrawingOptions.DefinedInView.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var view = project.Views.GetByName("&Gantt Chart");

Console.WriteLine("LegendOn option defined in view '{0}': {1}", view.Name, view.PageInfo.Legend.LegendOn);

SaveOptions options = new PdfSaveOptions
{
    // Получить параметры отрисовки легенды из представления
    LegendDrawingOptions = LegendDrawingOptions.DefinedInView,
    ViewSettings = view
};

project.Save(OutDir + "Legend_DefinedInView.pdf", options);
```

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

* enum [LegendDrawingOptions](../../legenddrawingoptions/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


