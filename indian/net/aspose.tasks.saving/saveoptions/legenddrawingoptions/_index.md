---
title: "SaveOptions.LegendDrawingOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। मान प्राप्त करता है या सेट करता है जो यह निर्धारित करता है कि लेजेंड कैसे रेंडर किया जाए। डिफ़ॉल्ट मान है LegendDrawingOptions.OnEveryPage"
type: docs
weight: 80
url: /hi/net/aspose.tasks.saving/saveoptions/legenddrawingoptions/
---
## SaveOptions.LegendDrawingOptions property

एक मान प्राप्त करता है या सेट करता है जो परिभाषित करता है कि लेजेंड कैसे रेंडर किया जाए। डिफ़ॉल्ट मान LegendDrawingOptions.OnEveryPage है।

```csharp
public LegendDrawingOptions LegendDrawingOptions { get; set; }
```

## टिप्पणियाँ

केवल तब लागू होता है जब Gantt चार्ट व्यू रेंडर किया जाता है।

## उदाहरण

दिखाता है कि अंतिम पृष्ठ पर लेजेंड कैसे प्रिंट करें

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // व्यू से लेजेंड ड्रॉइंग विकल्प लें
    LegendDrawingOptions = LegendDrawingOptions.AfterLastPage
};

project.Save(OutDir + "LegendOnSeparatePage_out.pdf", options);
```

दिखाता है कि पृष्ठ लेजेंड को कैसे छिपाएँ।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // लेजेंड को छिपाने के लिए LegendDrawingOptions.NoLegend निर्दिष्ट करें
    LegendDrawingOptions = LegendDrawingOptions.NoLegend
};

project.Save(OutDir + "HideLegendsDuringSave_out.pdf", options);
```

दिखाता है कि LegendDrawingOptions.DefinedInView विकल्प का उपयोग कैसे करें।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var view = project.Views.GetByName("&Gantt Chart");

Console.WriteLine("LegendOn option defined in view '{0}': {1}", view.Name, view.PageInfo.Legend.LegendOn);

SaveOptions options = new PdfSaveOptions
{
    // व्यू से लेजेंड ड्रॉइंग विकल्प लें
    LegendDrawingOptions = LegendDrawingOptions.DefinedInView,
    ViewSettings = view
};

project.Save(OutDir + "Legend_DefinedInView.pdf", options);
```

गैंट चार्ट के पेज लेजेंड में टास्क बार को कस्टमाइज़ करने का तरीका दिखाता है।

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

### संबंधित देखें

* enum [LegendDrawingOptions](../../legenddrawingoptions/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


