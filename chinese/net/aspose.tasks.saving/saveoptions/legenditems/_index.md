---
title: "SaveOptions.LegendItems"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SaveOptions 属性。获取或设置一个 PageLegendItem 数组，用于定义哪些条形应在页面图例中渲染。如果为 null，则渲染默认项。"
type: docs
weight: 90
url: /zh/net/aspose.tasks.saving/saveoptions/legenditems/
---
## SaveOptions.LegendItems property

获取或设置 PageLegendItem 数组，定义哪些条形应在页面图例中渲染。如果为 null，则渲染默认项。

```csharp
public PageLegendItem[] LegendItems { get; set; }
```

## 备注

仅在渲染甘特图视图时适用。

## 示例

展示如何在甘特图页面图例中自定义任务条。

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

### 另见

* class [PageLegendItem](../../../aspose.tasks.visualization/pagelegenditem/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


