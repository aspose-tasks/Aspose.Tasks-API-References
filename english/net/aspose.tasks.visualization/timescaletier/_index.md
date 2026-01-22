---
title: Class TimescaleTier
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.TimescaleTier class. Represents a single tier of the timescale on a Gantt Chart
type: docs
weight: 3420
url: /net/aspose.tasks.visualization/timescaletier/
---
## TimescaleTier class

Represents a single tier of the timescale on a Gantt Chart.

```csharp
public sealed class TimescaleTier
```

## Constructors

| Name | Description |
| --- | --- |
| [TimescaleTier](timescaletier/#constructor)() | Initializes a new instance of the `TimescaleTier` class. |
| [TimescaleTier](timescaletier/#constructor_1)(TimescaleUnit, int) | Initializes a new instance of the `TimescaleTier` class. |

## Properties

| Name | Description |
| --- | --- |
| [Alignment](../../aspose.tasks.visualization/timescaletier/alignment/) { get; set; } | Gets or sets how to align labels within each time period of the tier ([`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [Count](../../aspose.tasks.visualization/timescaletier/count/) { get; set; } | Gets or sets the time unit interval in which to show labels for the tier. The default value is 1. |
| [DateTimeConverter](../../aspose.tasks.visualization/timescaletier/datetimeconverter/) { get; set; } | Gets or sets a callback function for handling rendering date tick in this tier. |
| [Label](../../aspose.tasks.visualization/timescaletier/label/) { get; set; } | Gets or sets date label [`DateLabel`](../datelabel/) for the timescale tier. |
| [RenderLabelOnEachPage](../../aspose.tasks.visualization/timescaletier/renderlabeloneachpage/) { get; set; } | Gets or sets flag that defines whether date labels should be rendered on each page when a time period spans over several pages. If value is 'true', when time period spans over several pages, date labels for the period are rendered on each page. If values is 'false', date label is rendered only once according to a value of [`Alignment`](./alignment/) property. |
| [ShowTicks](../../aspose.tasks.visualization/timescaletier/showticks/) { get; set; } | Gets or sets a value indicating whether whether to show tick marks that separate time periods in the tier. |
| [Unit](../../aspose.tasks.visualization/timescaletier/unit/) { get; set; } | Gets or sets timescale unit [`TimescaleUnit`](../timescaleunit/) for the timescale tier. The default value is [`Days`](../timescaleunit/). |
| [UsesFiscalYear](../../aspose.tasks.visualization/timescaletier/usesfiscalyear/) { get; set; } | Gets or sets a value indicating whether to base the tier labels on the fiscal year. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


