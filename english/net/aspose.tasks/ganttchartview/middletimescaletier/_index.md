---
title: GanttChartView.MiddleTimescaleTier
second_title: Aspose.Tasks for .NET API Reference
description: GanttChartView property. Gets or sets settings of views middle timescale tier. TimescaleTier
type: docs
weight: 100
url: /net/aspose.tasks/ganttchartview/middletimescaletier/
---
## GanttChartView.MiddleTimescaleTier property

Gets or sets settings of view's middle timescale tier. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/).

```csharp
public TimescaleTier MiddleTimescaleTier { get; set; }
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

Shows how to customize timescale tier labels.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// Add task links
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// tune timescale tiers

// tune the top tier
// set the top timescale tier of the Gantt Chart view.
view.MiddleTimescaleTier = new TimescaleTier();
// set timescale unit <see cref="T:Aspose.Tasks.Visualization.TimescaleUnit" /> for the timescale tier.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// set the time unit interval in which to show labels for the tier.
view.MiddleTimescaleTier.Count = 1;
// set date label <see cref="T:Aspose.Tasks.Visualization.DateLabel" /> for the timescale tier.
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// set how to align labels within each time period of the tier (<see cref="T:System.Drawing.StringAlignment" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// set a value indicating whether whether to show tick marks that separate time periods in the tier.
view.MiddleTimescaleTier.ShowTicks = true;
// set a value indicating whether to base the tier labels on the fiscal year.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// added for better visualization
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// customize middle tier dates
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Use 'Timescale.DefinedInView' option to render timescales using timescale settings defined in view (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier). 
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### See Also

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


