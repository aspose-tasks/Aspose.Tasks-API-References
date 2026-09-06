---
title: "类 PageLegendItem"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.PageLegendItem 类。表示甘特图页面图例的一个项目。"
type: docs
weight: 3220
url: /zh/net/aspose.tasks.visualization/pagelegenditem/
---
## PageLegendItem class

表示甘特图页面图例的一个项目。

```csharp
public sealed class PageLegendItem
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PageLegendItem](pagelegenditem/)(BarItemType, string) | 初始化 `PageLegendItem` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [ItemType](../../aspose.tasks.visualization/pagelegenditem/itemtype/) { get; } | 获取项目的类型。 |
| [Title](../../aspose.tasks.visualization/pagelegenditem/title/) { get; } | 获取项目的文本标签。 |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


