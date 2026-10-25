---
title: "SaveOptions.LegendDrawingOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει μια τιμή που καθορίζει πώς να αποτυπώσετε ένα υπόμνημα. Η προεπιλεγμένη τιμή είναι LegendDrawingOptions.OnEveryPage"
type: docs
weight: 80
url: /el/net/aspose.tasks.saving/saveoptions/legenddrawingoptions/
---
## SaveOptions.LegendDrawingOptions property

Αποκτά ή ορίζει μια τιμή που καθορίζει πώς θα αποδοθεί ένα υπόμνημα. Η προεπιλεγμένη τιμή είναι LegendDrawingOptions.OnEveryPage.

```csharp
public LegendDrawingOptions LegendDrawingOptions { get; set; }
```

## Παρατηρήσεις

Ισχύει μόνο όταν η προβολή Gantt chart αποδίδεται.

## Παραδείγματα

Δείχνει πώς να εκτυπώσετε το υπόμνημα στην τελευταία σελίδα

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Πάρτε τις επιλογές σχεδίασης υπομνήματος από την προβολή
    LegendDrawingOptions = LegendDrawingOptions.AfterLastPage
};

project.Save(OutDir + "LegendOnSeparatePage_out.pdf", options);
```

Δείχνει πώς να κρύψετε τα υπομνήματα σελίδας.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Καθορίστε LegendDrawingOptions.NoLegend για να κρύψετε τα υπομνήματα
    LegendDrawingOptions = LegendDrawingOptions.NoLegend
};

project.Save(OutDir + "HideLegendsDuringSave_out.pdf", options);
```

Δείχνει πώς να χρησιμοποιήσετε την επιλογή LegendDrawingOptions.DefinedInView.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var view = project.Views.GetByName("&Gantt Chart");

Console.WriteLine("LegendOn option defined in view '{0}': {1}", view.Name, view.PageInfo.Legend.LegendOn);

SaveOptions options = new PdfSaveOptions
{
    // Πάρτε τις επιλογές σχεδίασης υπομνήματος από την προβολή
    LegendDrawingOptions = LegendDrawingOptions.DefinedInView,
    ViewSettings = view
};

project.Save(OutDir + "Legend_DefinedInView.pdf", options);
```

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

* enum [LegendDrawingOptions](../../legenddrawingoptions/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


