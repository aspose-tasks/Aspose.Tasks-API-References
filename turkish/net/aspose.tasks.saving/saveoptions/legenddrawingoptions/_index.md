---
title: "SaveOptions.LegendDrawingOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Bir lejandı nasıl çizeceğini tanımlayan bir değeri alır veya ayarlar. Varsayılan değer LegendDrawingOptions.OnEveryPage'dir."
type: docs
weight: 80
url: /tr/net/aspose.tasks.saving/saveoptions/legenddrawingoptions/
---
## SaveOptions.LegendDrawingOptions property

Bir lejantın nasıl render edileceğini tanımlayan bir değeri alır veya ayarlar. Varsayılan değer LegendDrawingOptions.OnEveryPage'dir.

```csharp
public LegendDrawingOptions LegendDrawingOptions { get; set; }
```

## Açıklamalar

Yalnızca Gantt şeması görünümü render edildiğinde uygulanır.

## Örnekler

Son sayfada lejandı nasıl yazdırılacağını gösterir

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Lejant çizim seçeneklerini görünümdan al
    LegendDrawingOptions = LegendDrawingOptions.AfterLastPage
};

project.Save(OutDir + "LegendOnSeparatePage_out.pdf", options);
```

Sayfa lejandlarını nasıl gizleyeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Lejantları gizlemek için LegendDrawingOptions.NoLegend belirtin
    LegendDrawingOptions = LegendDrawingOptions.NoLegend
};

project.Save(OutDir + "HideLegendsDuringSave_out.pdf", options);
```

LegendDrawingOptions.DefinedInView seçeneğinin nasıl kullanılacağını gösterir

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var view = project.Views.GetByName("&Gantt Chart");

Console.WriteLine("LegendOn option defined in view '{0}': {1}", view.Name, view.PageInfo.Legend.LegendOn);

SaveOptions options = new PdfSaveOptions
{
    // Lejant çizim seçeneklerini görünümdan al
    LegendDrawingOptions = LegendDrawingOptions.DefinedInView,
    ViewSettings = view
};

project.Save(OutDir + "Legend_DefinedInView.pdf", options);
```

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

* enum [LegendDrawingOptions](../../legenddrawingoptions/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


