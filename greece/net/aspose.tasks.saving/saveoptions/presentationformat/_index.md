---
title: "SaveOptions.PresentationFormat"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει το PresentationFormat στο οποίο θα αποθηκευτεί το έγγραφο."
type: docs
weight: 140
url: /el/net/aspose.tasks.saving/saveoptions/presentationformat/
---
## SaveOptions.PresentationFormat property

Λαμβάνει ή ορίζει το `PresentationFormat` στο οποίο θα αποθηκευτεί το έγγραφο.

```csharp
public PresentationFormat PresentationFormat { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε μια τιμή που υποδεικνύει ότι οι υποεργασίες στη γραμμή σύνοψης εργασίας πρέπει να συγκεντρωθούν.

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // Ή
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

Δείχνει πώς να αποδώσετε την προβολή χρήσης εργασίας με τις ρυθμίσεις χρονικής κλίμακας που ορίζονται στις ρυθμίσεις προβολής.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// Ορίστε τις SaveOptions και καθορίστε ότι πρέπει να χρησιμοποιηθούν οι ρυθμίσεις κλίμακας χρόνου TaskUsageView.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

### Δείτε επίσης

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


