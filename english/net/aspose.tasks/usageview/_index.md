---
title: Class UsageView
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.UsageView class. Represent a usage view in a project
type: docs
weight: 2620
url: /net/aspose.tasks/usageview/
---
## UsageView class

Represent a usage view in a project.

```csharp
public abstract class UsageView : View
```

## Properties

| Name | Description |
| --- | --- |
| [AlignDetailsData](../../aspose.tasks/usageview/aligndetailsdata/) { get; set; } | Gets or sets details data alignment. |
| [BottomTimescaleTier](../../aspose.tasks/usageview/bottomtimescaletier/) { get; set; } | Gets or sets settings of view's bottom timescale tier. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [DisplayDetailsHeaderColumn](../../aspose.tasks/usageview/displaydetailsheadercolumn/) { get; set; } | Gets or sets a value indicating whether to display details header column in the view or not. |
| [DisplayShortDetailHeaderNames](../../aspose.tasks/usageview/displayshortdetailheadernames/) { get; set; } | Gets or sets a value indicating whether to display short detail header names or not. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Gets or sets a filter used in a single view. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Gets or sets a group of the single view. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Gets or sets a value indicating whether Microsoft Project highlights the filter for a single view. |
| [MiddleTimescaleTier](../../aspose.tasks/usageview/middletimescaletier/) { get; set; } | Gets or sets settings of view's middle timescale tier. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Gets or sets the name of a View object. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Gets an instance of the [`PageInfo`](../view/pageinfo/) class. Represents page setup data which is present in mpp file format. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Gets the parent of the View object. Read-only [`Project`](../project/). |
| [RepeatDetailsHeaderOnAllRows](../../aspose.tasks/usageview/repeatdetailsheaderonallrows/) { get; set; } | Gets or sets a value indicating whether to repeat details header on all assignment row or not. |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Gets the screen type for the single view. Read-only [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Gets or sets a value indicating whether Microsoft Project shows the single view name in the View or the Other Views drop-down lists in the Ribbon. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Gets or sets a table of the single view. |
| [TimescaleSizePercentage](../../aspose.tasks/usageview/timescalesizepercentage/) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/usageview/toptimescaletier/) { get; set; } | Gets or sets settings of view's top timescale tier. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
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

Shows how to render task usage view with details.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// get the view
UsageView view = (TaskUsageView)project.DefaultView;

// details header column will not be displayed
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.DisplayShortDetailHeaderNames = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// display details header column
view.DisplayDetailsHeaderColumn = true;

// repeat details header on all assignments rows
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

### See Also

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


