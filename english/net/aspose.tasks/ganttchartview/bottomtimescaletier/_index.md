---
title: GanttChartView.BottomTimescaleTier
second_title: Aspose.Tasks for .NET API Reference
description: GanttChartView property. Gets or sets settings of views bottom timescale tier. TimescaleTier
type: docs
weight: 60
url: /net/aspose.tasks/ganttchartview/bottomtimescaletier/
---
## GanttChartView.BottomTimescaleTier property

Gets or sets settings of view's bottom timescale tier. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/)

```csharp
public TimescaleTier BottomTimescaleTier { get; set; }
```

## Examples

Shows how to work with timescale tiers through save options.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

GanttChartView ganttChartView = (GanttChartView) project.Views.ToList()[0];

// set the timescale tiers of the Gantt Chart view
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

// save the project as an image
project.Save(OutDir + "WorkWithTimescaleTier_out.png", options);
```

Shows how to modify timescale tiers.

```csharp
var project = new Project();

// Init Gantt Chart View
var view = new GanttChartView
{
    TopTimescaleTier = new TimescaleTier(),
    MiddleTimescaleTier = new TimescaleTier(),
    BottomTimescaleTier = new TimescaleTier()
};

// set Time Scale count
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

// add Gantt Chart View to project
project.Views.Add(view);

// add some test data to project
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

// Use 'Timescale.DefinedInView' option to render timescales using timescale settings which we have set (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier). 
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    StartDate = DateTime.Now.AddDays(-30),
    EndDate = DateTime.Now.AddDays(30)
};

project.Save(OutDir + "WorkWithTimescaleTier_out.pdf", pdfSaveOptions);
```

### See Also

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


