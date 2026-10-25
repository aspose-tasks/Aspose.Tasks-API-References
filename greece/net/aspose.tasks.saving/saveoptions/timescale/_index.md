---
title: "SaveOptions.Timescale"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει την τιμή Timescale που χρησιμοποιείται για τον έλεγχο του τρόπου απόδοσης της κλίμακας χρόνου, εάν υπάρχει, όταν το έργο αποθηκεύεται σε γραφική μορφή."
type: docs
weight: 200
url: /el/net/aspose.tasks.saving/saveoptions/timescale/
---
## SaveOptions.Timescale property

Λαμβάνει ή ορίζει την τιμή `Timescale` που χρησιμοποιείται για τον έλεγχο του τρόπου απόδοσης της κλίμακας χρόνου (εάν υπάρχει) όταν το έργο αποθηκεύεται σε γραφική μορφή.

```csharp
public Timescale Timescale { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε την ελάχιστη χρονική περίοδο για απόδοση. Η προεπιλεγμένη τιμή είναι <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.Timescale\">Days</see>.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Αποθήκευση σε εικόνα μίας σελίδας (Timescale.days ως προεπιλογή)
project.Save(OutDir + "NewProductDevDays_out.jpeg", new ImageSaveOptions(SaveFileFormat.Jpeg));

// Αποθήκευση σε εικόνα μίας σελίδας (Timescale.ThirdsOfMonths)
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    Timescale = Timescale.ThirdsOfMonths
};

project.Save(OutDir + "NewProductDevThirdsOfMonths_out.jpeg", options);

// Αποθήκευση σε εικόνα μίας σελίδας (Timescale.Months)
options.Timescale = Timescale.Months;
project.Save(OutDir + "NewProductDevMonths_out.jpeg", options);
```

Δείχνει πώς να εργαστείτε με τα επίπεδα κλίμακας χρόνου μέσω των επιλογών αποθήκευσης.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

GanttChartView ganttChartView = (GanttChartView) project.Views.ToList()[0];

// ορίστε τα επίπεδα κλίμακας χρόνου της προβολής Gantt Chart
ganttChartView.MiddleTimescaleTier.Unit = TimescaleUnit.Months;
ganttChartView.MiddleTimescaleTier.Count = 1;
ganttChartView.MiddleTimescaleTier.Label = DateLabel.MonthMmmm;

ganttChartView.BottomTimescaleTier.Unit = TimescaleUnit.Days;
ganttChartView.BottomTimescaleTier.Count = 1;
ganttChartView.BottomTimescaleTier.Label = DateLabel.DayDddDd;

// ...
var options = new ImageSaveOptions(SaveFileFormat.Png)
{
    Timescale = Timescale.DefinedInView
};

// ...

// αποθηκεύστε το έργο ως εικόνα
project.Save(OutDir + "WorkWithTimescaleTier_out.png", options);
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

Δείχνει πώς να τροποποιήσετε τα επίπεδα κλίμακας χρόνου.

```csharp
var project = new Project();

// Αρχικοποίηση προβολής Gantt Chart
var view = new GanttChartView
{
    TopTimescaleTier = new TimescaleTier(),
    MiddleTimescaleTier = new TimescaleTier(),
    BottomTimescaleTier = new TimescaleTier()
};

// ορίστε τον αριθμό κλίμακας χρόνου
view.TopTimescaleTier.Count = 2;
view.TopTimescaleTier.Unit = TimescaleUnit.Quarters;
view.TopTimescaleTier.Label = DateLabel.QuarterQQyy;
view.TopTimescaleTier.ShowTicks = false;

view.MiddleTimescaleTier.Count = 2;
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
view.MiddleTimescaleTier.ShowTicks = false;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayDdd;
view.BottomTimescaleTier.Count = 2;
view.BottomTimescaleTier.ShowTicks = false;

// προσθέστε την προβολή Gantt Chart στο έργο
project.Views.Add(view);

// προσθέστε κάποια δεδομένα δοκιμής στο έργο
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

// Χρησιμοποιήστε την επιλογή 'Timescale.DefinedInView' για να αποδώσετε τις κλίμακες χρόνου χρησιμοποιώντας τις ρυθμίσεις κλίμακας χρόνου που έχουμε ορίσει (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    StartDate = DateTime.Now.AddDays(-30),
    EndDate = DateTime.Now.AddDays(30)
};

project.Save(OutDir + "WorkWithTimescaleTier_out.pdf", pdfSaveOptions);
```

### Δείτε επίσης

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


