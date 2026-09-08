---
title: "Класс PageLegendItem"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.PageLegendItem класс. Представляет элемент легенды страницы диаграммы Ганта"
type: docs
weight: 3220
url: /ru/net/aspose.tasks.visualization/pagelegenditem/
---
## PageLegendItem class

Представляет элемент легенды страницы диаграммы Ганта.

```csharp
public sealed class PageLegendItem
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PageLegendItem](pagelegenditem/)(BarItemType, string) | Инициализирует новый экземпляр класса `PageLegendItem`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ItemType](../../aspose.tasks.visualization/pagelegenditem/itemtype/) { get; } | Получает тип элемента. |
| [Title](../../aspose.tasks.visualization/pagelegenditem/title/) { get; } | Получает текстовую метку элемента. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


