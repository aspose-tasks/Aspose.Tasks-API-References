---
title: "SaveOptions.LegendItems"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει έναν πίνακα PageLegendItem που καθορίζει ποια μπαρ πρέπει να αποδοθούν στο υπόμνημα της σελίδας. Εάν είναι null, αποδίδονται τα προεπιλεγμένα στοιχεία."
type: docs
weight: 90
url: /el/net/aspose.tasks.saving/saveoptions/legenditems/
---
## SaveOptions.LegendItems property

Αποκτά ή ορίζει έναν πίνακα των PageLegendItem που καθορίζουν ποιες μπάρες πρέπει να αποδοθούν στο υπόμνημα της σελίδας. Εάν είναι null, αποδίδονται τα προεπιλεγμένα στοιχεία.

```csharp
public PageLegendItem[] LegendItems { get; set; }
```

## Παρατηρήσεις

Ισχύει μόνο όταν η προβολή Gantt chart αποδίδεται.

## Παραδείγματα

Δείχνει πώς να προσαρμόσετε τις μπάρες εργασιών στο υπόμνημα σελίδας του διαγράμματος Gantt.

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

### Δείτε επίσης

* class [PageLegendItem](../../../aspose.tasks.visualization/pagelegenditem/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


