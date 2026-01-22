---
title: Class TimelineView
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TimelineView class. Represents a timeline view of a project
type: docs
weight: 2550
url: /net/aspose.tasks/timelineview/
---
## TimelineView class

Represents a timeline view of a project.

```csharp
public class TimelineView : View
```

## Constructors

| Name | Description |
| --- | --- |
| [TimelineView](timelineview/)() | Initializes a new instance of the `TimelineView` class. |

## Properties

| Name | Description |
| --- | --- |
| [DateFormat](../../aspose.tasks/timelineview/dateformat/) { get; set; } | Gets or sets a value indicating how to format dates on the Timeline view. |
| [DisplayOverlapped](../../aspose.tasks/timelineview/displayoverlapped/) { get; set; } | Gets or sets a value indicating whether to display overlapped tasks on multiple rows. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Gets or sets a filter used in a single view. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Gets or sets a group of the single view. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Gets or sets a value indicating whether Microsoft Project highlights the filter for a single view. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Gets or sets the name of a View object. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Gets an instance of the [`PageInfo`](../view/pageinfo/) class. Represents page setup data which is present in mpp file format. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Gets the parent of the View object. Read-only [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Gets the screen type for the single view. Read-only [`ViewScreen`](../viewscreen/). |
| [ShowDates](../../aspose.tasks/timelineview/showdates/) { get; } | Gets a value indicating whether to show dates. |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Gets or sets a value indicating whether Microsoft Project shows the single view name in the View or the Other Views drop-down lists in the Ribbon. |
| [ShowPanZoom](../../aspose.tasks/timelineview/showpanzoom/) { get; set; } | Gets or sets a value indicating whether to show pan and zoom control. |
| [ShowTimescale](../../aspose.tasks/timelineview/showtimescale/) { get; set; } | Gets or sets a value indicating whether to show timescale. |
| [ShowToday](../../aspose.tasks/timelineview/showtoday/) { get; set; } | Gets or sets a value indicating whether to display a line representing today. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Gets or sets a table of the single view. |
| [TextLinesCount](../../aspose.tasks/timelineview/textlinescount/) { get; set; } | Gets or sets a value indicating how many lines are used to display task in a timeline. |
| [Type](../../aspose.tasks/view/type/) { get; } | Gets the type of item in the single view, such as tasks or resources. Read-only [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Gets the unique identifier of a view. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Gets a collection of objects representing placement and appearance of [`OleObject`](../oleobject/) in the view. |

## Methods

| Name | Description |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Compares the current instance with another object of the same type and returns an integer that indicates whether the current instance precedes, follows, or occurs in the same position in the sort order as the other object. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Returns a value indicating whether this instance is equal to a specified object. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Returns a hash code value for the instance of the [`Resource`](../resource/) class. |

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

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


