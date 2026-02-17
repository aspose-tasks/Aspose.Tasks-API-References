---
title: Class View
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.View class. Represents a view in Project
type: docs
weight: 2870
url: /net/aspose.tasks/view/
---
## View class

Represents a view in Project.

```csharp
public class View : IComparable<View>
```

## Constructors

| Name | Description |
| --- | --- |
| [View](view/#constructor)() | Initializes a new instance of the `View` class. |
| [View](view/#constructor_1)(ViewScreen) | Initializes a new instance of the `View` class. |

## Properties

| Name | Description |
| --- | --- |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Gets or sets a filter used in a single view. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Gets or sets a group of the single view. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Gets or sets a value indicating whether Microsoft Project highlights the filter for a single view. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Gets or sets the name of a View object. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Gets an instance of the [`PageInfo`](./pageinfo/) class. Represents page setup data which is present in mpp file format. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Gets the parent of the View object. Read-only [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Gets the screen type for the single view. Read-only [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Gets or sets a value indicating whether Microsoft Project shows the single view name in the View or the Other Views drop-down lists in the Ribbon. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Gets or sets a table of the single view. |
| [Type](../../aspose.tasks/view/type/) { get; } | Gets the type of item in the single view, such as tasks or resources. Read-only [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Gets the unique identifier of a view. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Gets a collection of objects representing placement and appearance of [`OleObject`](../oleobject/) in the view. |

## Methods

| Name | Description |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Compares the current instance with another object of the same type and returns an integer that indicates whether the current instance precedes, follows, or occurs in the same position in the sort order as the other object. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Returns a value indicating whether this instance is equal to a specified object. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Returns a hash code value for the instance of the [`Resource`](../resource/) class. |
| [operator ==](../../aspose.tasks/view/op_equality/) | Returns a value indicating whether this instance is equal to a specified object. |
| [operator &gt;](../../aspose.tasks/view/op_greaterthan/) | Returns a value indicating whether this instance is greater than a specified object. |
| [operator &gt;=](../../aspose.tasks/view/op_greaterthanorequal/) | Returns a value indicating whether this instance is greater than or equal to a specified object. |
| [operator !=](../../aspose.tasks/view/op_inequality/) | Returns a value indicating whether this instance is not equal to a specified object. |
| [operator &lt;](../../aspose.tasks/view/op_lessthan/) | Returns a value indicating whether this instance is less than a specified object. |
| [operator &lt;=](../../aspose.tasks/view/op_lessthanorequal/) | Returns a value indicating whether this instance is less than or equal to a specified object. |

## Examples

Shows how to work with Project's view and add column to the default view (which is shown when MPP file is opened in MS Project).

```csharp
// create an empty project without views 
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// Modify the default view (it's a Gantt chart view).
// Or you can select view by name or by View Screen using project.View collection.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// WriteViewData flag should be used to persist modifications of view's properties.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

Shows how to work with MS Project views.

```csharp
// create an empty project without views 
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// create a standard Gantt chart view
View view = new GanttChartView();

// set some view properties
// set a value indicating whether Microsoft Project shows the single view name in the View or the Other Views drop-down lists in the Ribbon
view.ShowInMenu = true;
// set a value indicating whether Microsoft Project highlights the filter for a single view
view.HighlightFilter = true;

// the writing of the next properties is not supported
// sets the filter used in a single view
view.Filter = null;
// sets the group of the single view
view.Group = null;
// sets the table of the single view
view.Table = null;

// lets tune some view settings
// set the number of first columns to be printed on all pages
view.PageInfo.PageViewSettings.FirstColumnsCount = 4;
// set a value indicating whether to print a specified number of first columns on all pages
view.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

// add the view to the our project
project.Views.Add(view);

// WriteViewData flag should be used to persist modifications of project.Views.
project.Save(OutDir + "WorkWithView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
// lets check some properties of the newly added view
// print the unique identifier of a view
Console.WriteLine("View Uid: " + view.Uid);
// print the screen type for the single view
Console.WriteLine("View Screen: " + view.Screen);
Console.WriteLine("View Type: " + view.Type);
Console.WriteLine("Parent Project of the view: " + view.ParentProject.Get(Prj.Name));
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


