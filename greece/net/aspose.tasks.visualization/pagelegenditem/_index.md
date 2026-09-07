---
title: "Κλάση PageLegendItem"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Visualization.PageLegendItem. Αντιπροσωπεύει ένα στοιχείο του υπομνήματος σελίδας του διαγράμματος Gantt"
type: docs
weight: 3220
url: /el/net/aspose.tasks.visualization/pagelegenditem/
---
## PageLegendItem class

Αναπαριστά ένα στοιχείο του υπομνήματος σελίδας του διαγράμματος Gantt.

```csharp
public sealed class PageLegendItem
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [PageLegendItem](pagelegenditem/)(BarItemType, string) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `PageLegendItem`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [ItemType](../../aspose.tasks.visualization/pagelegenditem/itemtype/) { get; } | Λαμβάνει τον τύπο του στοιχείου. |
| [Title](../../aspose.tasks.visualization/pagelegenditem/title/) { get; } | Λαμβάνει την ετικέτα κειμένου του στοιχείου. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


