---
title: Project.DefaultView
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets or sets default view of the project
type: docs
weight: 360
url: /net/aspose.tasks/project/defaultview/
---
## Project.DefaultView property

Gets or sets default view of the project.

```csharp
public View DefaultView { get; set; }
```

## Examples

Shows how to work with default view of a project.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// Get Default view
UsageView view = (TaskUsageView)project.DefaultView;

// Details header column will not be displayed
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// Display details header column
view.DisplayDetailsHeaderColumn = true;

// Repeat details header on all assignments rows
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

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

### See Also

* class [View](../../view/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


