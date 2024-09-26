---
title: View.PageInfo
second_title: Aspose.Tasks for .NET API Reference
description: View property. Gets an instance of the PageInfo class. Represents page setup data which is present in mpp file format
type: docs
weight: 60
url: /net/aspose.tasks/view/pageinfo/
---
## View.PageInfo property

Gets an instance of the `PageInfo` class. Represents page setup data which is present in mpp file format.

```csharp
public PageInfo PageInfo { get; }
```

## Examples

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

* class [PageInfo](../../../aspose.tasks.visualization/pageinfo/)
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


