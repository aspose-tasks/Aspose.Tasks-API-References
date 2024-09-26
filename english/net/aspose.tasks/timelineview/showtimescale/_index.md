---
title: TimelineView.ShowTimescale
second_title: Aspose.Tasks for .NET API Reference
description: TimelineView property. Gets or sets a value indicating whether to show timescale
type: docs
weight: 60
url: /net/aspose.tasks/timelineview/showtimescale/
---
## TimelineView.ShowTimescale property

Gets or sets a value indicating whether to show timescale.

```csharp
public bool ShowTimescale { get; set; }
```

## Examples

Shows how to work with &lt;see cref="Aspose.Tasks.TimelineView" /&gt;.

```csharp
var project = new Project();

// initialize a timeline view
var view = new TimelineView();

// set a value indicating how to format dates on the Timeline view.
view.DateFormat = DateFormat.DateDddDd;
// set a value indicating whether to display overlapped tasks on multiple rows.
view.DisplayOverlapped = true;
// set a value indicating whether to show pan and zoom control.
view.ShowPanZoom = true;
// set a value indicating whether to show timescale.
view.ShowTimescale = true;
// set a value indicating whether to display a line representing today.
view.ShowToday = true;
// set a value indicating how many lines are used to display task in a timeline.
view.TextLinesCount = 2;

// gets a value indicating whether to display overlapped tasks on multiple rows.
Console.WriteLine("Show Dates: " + view.ShowDates);

// add the view to the project
project.Views.Add(view);

// add some test data to project
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

project.Save(OutDir + "SetTimeScaleCount_out.pdf", SaveFileFormat.Pdf);
```

### See Also

* class [TimelineView](../)
* namespace [Aspose.Tasks](../../timelineview/)
* assembly [Aspose.Tasks](../../../)


