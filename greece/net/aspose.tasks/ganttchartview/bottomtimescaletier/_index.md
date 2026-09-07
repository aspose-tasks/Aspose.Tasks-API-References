---
title: "GanttChartView.BottomTimescaleTier"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα GanttChartView. Λαμβάνει ή ορίζει τις ρυθμίσεις του κατώτερου επιπέδου κλίμακας χρόνου της προβολής. TimescaleTier"
type: docs
weight: 60
url: /el/net/aspose.tasks/ganttchartview/bottomtimescaletier/
---
## GanttChartView.BottomTimescaleTier property

Λαμβάνει ή ορίζει τις ρυθμίσεις του κατώτερου επιπέδου κλίμακας χρόνου της προβολής. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/)

```csharp
public TimescaleTier BottomTimescaleTier { get; set; }
```

## Παραδείγματα

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

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


