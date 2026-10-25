---
title: "क्लास PageLegendItem"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.PageLegendItem क्लास। गैंट चार्ट के पेज लेजेंड का एक आइटम दर्शाता है"
type: docs
weight: 3220
url: /hi/net/aspose.tasks.visualization/pagelegenditem/
---
## PageLegendItem class

गैंट चार्ट के पेज लेजेंड का एक आइटम दर्शाता है।

```csharp
public sealed class PageLegendItem
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PageLegendItem](pagelegenditem/)(BarItemType, string) | `PageLegendItem` क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [ItemType](../../aspose.tasks.visualization/pagelegenditem/itemtype/) { get; } | आइटम का प्रकार प्राप्त करता है। |
| [Title](../../aspose.tasks.visualization/pagelegenditem/title/) { get; } | आइटम का टेक्स्ट लेबल प्राप्त करता है। |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


