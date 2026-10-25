---
title: "SaveOptions.LegendItems"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveOptions. يحصل أو يحدد مصفوفة من PageLegendItem التي تحدد أي الأشرطة يجب عرضها في وسيلة إيضاح الصفحة. إذا كانت null يتم عرض العناصر الافتراضية."
type: docs
weight: 90
url: /ar/net/aspose.tasks.saving/saveoptions/legenditems/
---
## SaveOptions.LegendItems property

يحصل أو يعيّن مصفوفة من PageLegendItem التي تحدد أي الأشرطة يجب عرضها في وسيلة إيضاح الصفحة. إذا كانت null، تُعرض العناصر الافتراضية.

```csharp
public PageLegendItem[] LegendItems { get; set; }
```

## ملاحظات

يُطبق فقط عندما يتم تصوير عرض مخطط Gantt.

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

* class [PageLegendItem](../../../aspose.tasks.visualization/pagelegenditem/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


