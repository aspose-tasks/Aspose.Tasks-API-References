---
title: SaveOptions.View
second_title: Aspose.Tasks for .NET API Reference
description: SaveOptions property. Gets or sets a list of the view columns to render GanttChartColumn. If not set then task ids task names start and finish are rendered only. If both View and ViewSettings properties are set columns from View overrides columns from ViewSettings
type: docs
weight: 230
url: /net/aspose.tasks.saving/saveoptions/view/
---
## SaveOptions.View property

Gets or sets a list of the view columns to render ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)). If not set then task ids, task names, start and finish are rendered only. If both View and [`ViewSettings`](../viewsettings/) properties are set, columns from View overrides columns from ViewSettings.

```csharp
public ProjectView View { get; set; }
```

## Examples

Shows how to add columns of view to be exported during export project.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new Spreadsheet2003SaveOptions();
var ganttChartColumn = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(ganttChartColumn);

var resourceViewColumn = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(resourceViewColumn);

var assignmentViewColumn = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assignmentViewColumn);

project.Save(OutDir + "UsingSpreadsheet2003SaveOptions_out.xml", options);
```

### See Also

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


