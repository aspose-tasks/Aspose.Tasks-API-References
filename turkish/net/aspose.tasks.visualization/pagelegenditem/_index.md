---
title: "Sınıf PageLegendItem"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.PageLegendItem sınıfı. Gantt şemasının sayfa açıklama öğesini temsil eder"
type: docs
weight: 3220
url: /tr/net/aspose.tasks.visualization/pagelegenditem/
---
## PageLegendItem class

Gantt çizelgesinin sayfa lejandının bir öğesini temsil eder.

```csharp
public sealed class PageLegendItem
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PageLegendItem](pagelegenditem/)(BarItemType, string) | `PageLegendItem` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ItemType](../../aspose.tasks.visualization/pagelegenditem/itemtype/) { get; } | Öğenin tipini alır. |
| [Title](../../aspose.tasks.visualization/pagelegenditem/title/) { get; } | Öğenin metin etiketini alır. |

## Örnekler

Gantt şemasının sayfa açıklamasındaki görev çubuklarını nasıl özelleştireceğinizi gösterir.

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

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


