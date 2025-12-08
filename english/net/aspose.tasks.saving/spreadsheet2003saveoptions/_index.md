---
title: Class Spreadsheet2003SaveOptions
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.Spreadsheet2003SaveOptions class. Allows to specify additional options when rendering project pages to Spreadsheet2003
type: docs
weight: 2190
url: /net/aspose.tasks.saving/spreadsheet2003saveoptions/
---
## Spreadsheet2003SaveOptions class

Allows to specify additional options when rendering project pages to Spreadsheet2003.

```csharp
public class Spreadsheet2003SaveOptions : SimpleSaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [Spreadsheet2003SaveOptions](spreadsheet2003saveoptions/)() | Initializes a new instance of the `Spreadsheet2003SaveOptions` class. |

## Properties

| Name | Description |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/spreadsheet2003saveoptions/assignmentview/) { get; set; } | Gets or sets a list of the assignments view columns to render ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [ResourceView](../../aspose.tasks.saving/spreadsheet2003saveoptions/resourceview/) { get; set; } | Gets or sets a list of the resource view columns to render ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Gets or sets the format in which the document will be saved if this save options object is used. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Gets or sets the comparer to sort tasks on Gantt chart and Task Sheet chart. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Gets or sets the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts. |
| [View](../../aspose.tasks.saving/spreadsheet2003saveoptions/view/) { get; set; } | Gets or sets a list of the view columns ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) to save. If not set then default columns are saved. |

## Examples

Shows how to add columns to be exported during export project into Spreadsheet2003 format.

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


