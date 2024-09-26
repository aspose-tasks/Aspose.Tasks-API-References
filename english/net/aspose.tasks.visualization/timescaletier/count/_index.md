---
title: TimescaleTier.Count
second_title: Aspose.Tasks for .NET API Reference
description: TimescaleTier property. Gets or sets the time unit interval in which to show labels for the tier. The default value is 1
type: docs
weight: 30
url: /net/aspose.tasks.visualization/timescaletier/count/
---
## TimescaleTier.Count property

Gets or sets the time unit interval in which to show labels for the tier. The default value is 1.

```csharp
public int Count { get; set; }
```

## Examples

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

* class [TimescaleTier](../)
* namespace [Aspose.Tasks.Visualization](../../timescaletier/)
* assembly [Aspose.Tasks](../../../)


