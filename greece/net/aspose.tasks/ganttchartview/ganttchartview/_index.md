---
title: "GanttChartView.GanttChartView"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής GanttChartView. Αρχικοποιεί μια νέα παρουσία της κλάσης GanttChartView"
type: docs
weight: 10
url: /el/net/aspose.tasks/ganttchartview/ganttchartview/
---
## GanttChartView constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`GanttChartView`](../).

```csharp
public GanttChartView()
```

## Παραδείγματα

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

* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


