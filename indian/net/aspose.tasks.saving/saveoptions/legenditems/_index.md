---
title: "SaveOptions.LegendItems"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। प्राप्त करता है या सेट करता है PageLegendItem की एक एरे जिसे परिभाषित करता है कि पेज लेजेंड में कौन से बार रेंडर किए जाने चाहिए। यदि null है तो डिफ़ॉल्ट आइटम रेंडर होते हैं।"
type: docs
weight: 90
url: /hi/net/aspose.tasks.saving/saveoptions/legenditems/
---
## SaveOptions.LegendItems property

PageLegendItem की एक एरे प्राप्त करता है या सेट करता है जो निर्धारित करता है कि पेज लेजेंड में कौन से बार रेंडर किए जाएँ। यदि null है, तो डिफ़ॉल्ट आइटम रेंडर होते हैं।

```csharp
public PageLegendItem[] LegendItems { get; set; }
```

## टिप्पणियाँ

केवल तब लागू होता है जब Gantt चार्ट व्यू रेंडर किया जाता है।

## उदाहरण

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

* class [PageLegendItem](../../../aspose.tasks.visualization/pagelegenditem/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


