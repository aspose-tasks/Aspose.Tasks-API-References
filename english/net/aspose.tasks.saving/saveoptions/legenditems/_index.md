---
title: SaveOptions.LegendItems
second_title: Aspose.Tasks for .NET API Reference
description: SaveOptions property. Gets or sets an array of PageLegendItem which define which bars should be rendered in page legend. If null the default items are rendered
type: docs
weight: 90
url: /net/aspose.tasks.saving/saveoptions/legenditems/
---
## SaveOptions.LegendItems property

Gets or sets an array of PageLegendItem which define which bars should be rendered in page legend. If null, the default items are rendered.

```csharp
public PageLegendItem[] LegendItems { get; set; }
```

## Remarks

Is only applicable when Gantt chart view is rendered.

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

* class [PageLegendItem](../../../aspose.tasks.visualization/pagelegenditem/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


