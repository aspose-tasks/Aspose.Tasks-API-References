---
title: Class PageLegendItem
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.PageLegendItem class. Represents an item of page legend of Gantt chart
type: docs
weight: 3170
url: /net/aspose.tasks.visualization/pagelegenditem/
---
## PageLegendItem class

Represents an item of page legend of Gantt chart.

```csharp
public sealed class PageLegendItem
```

## Constructors

| Name | Description |
| --- | --- |
| [PageLegendItem](pagelegenditem/)(BarItemType, string) | Initializes a new instance of the `PageLegendItem` class. |

## Properties

| Name | Description |
| --- | --- |
| [ItemType](../../aspose.tasks.visualization/pagelegenditem/itemtype/) { get; } | Gets type of the item. |
| [Title](../../aspose.tasks.visualization/pagelegenditem/title/) { get; } | Gets text label of the item. |

## Examples

Shows how to customize task bars in page legend of Gantt chart.

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

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


