---
title: "الفئة PageLegendItem"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Visualization.PageLegendItem. تمثل عنصرًا من وسيلة إيضاح الصفحة لمخطط جانت."
type: docs
weight: 3220
url: /ar/net/aspose.tasks.visualization/pagelegenditem/
---
## PageLegendItem class

يمثل عنصرًا من أسطورة الصفحة في مخطط جانت.

```csharp
public sealed class PageLegendItem
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PageLegendItem](pagelegenditem/)(BarItemType, string) | يُنشئ مثيلًا جديدًا للفئة `PageLegendItem`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ItemType](../../aspose.tasks.visualization/pagelegenditem/itemtype/) { get; } | يحصل على نوع العنصر. |
| [Title](../../aspose.tasks.visualization/pagelegenditem/title/) { get; } | يحصل على تسمية النص للعنصر. |

## الأمثلة

يعرض كيفية تخصيص أشرطة المهام في وسيلة إيضاح الصفحة لمخطط جانت.

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

### انظر أيضًا

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


