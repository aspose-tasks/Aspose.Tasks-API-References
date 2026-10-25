---
title: "SaveOptions.LegendItems"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Sayfa başlığı içinde hangi çubukların render edileceğini tanımlayan PageLegendItem dizisini alır veya ayarlar. Null ise varsayılan öğeler render edilir."
type: docs
weight: 90
url: /tr/net/aspose.tasks.saving/saveoptions/legenditems/
---
## SaveOptions.LegendItems property

Sayfa lejantında hangi çubukların render edileceğini tanımlayan bir PageLegendItem dizisini alır veya ayarlar. Null ise, varsayılan öğeler render edilir.

```csharp
public PageLegendItem[] LegendItems { get; set; }
```

## Açıklamalar

Yalnızca Gantt şeması görünümü render edildiğinde uygulanır.

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

* class [PageLegendItem](../../../aspose.tasks.visualization/pagelegenditem/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


