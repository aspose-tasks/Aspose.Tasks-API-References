---
title: Class XlsxOptions
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.XlsxOptions class. Allows to specify additional options when rendering project pages to XLSX
type: docs
weight: 2240
url: /net/aspose.tasks.saving/xlsxoptions/
---
## XlsxOptions class

Allows to specify additional options when rendering project pages to XLSX.

```csharp
public class XlsxOptions : SimpleSaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [XlsxOptions](xlsxoptions/)() | Initializes a new instance of the `XlsxOptions` class that can be used to save project in XLSX format. |

## Properties

| Name | Description |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/xlsxoptions/assignmentview/) { get; set; } | Gets or sets a list of the assignments view columns to render ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [Encoding](../../aspose.tasks.saving/xlsxoptions/encoding/) { get; set; } | Gets or sets the encoding of the resulting XLSX file. The default value is UTF8. |
| [ResourceView](../../aspose.tasks.saving/xlsxoptions/resourceview/) { get; set; } | Gets or sets a list of the resource view columns to render ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Gets or sets the format in which the document will be saved if this save options object is used. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Gets or sets the comparer to sort tasks on Gantt chart and Task Sheet chart. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Gets or sets the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts. |
| [View](../../aspose.tasks.saving/xlsxoptions/view/) { get; set; } | Gets or sets a list of the view columns ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) to save to XLSX format. If not set then default columns are saved. |

## Examples

Shows how to save a project into XLSX file by using &lt;see cref="P:Aspose.Tasks.Saving.XlsxOptions"&gt;Days&lt;/see&gt; options.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new XlsxOptions();

// Add desired Gantt Chart columns
var col = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(col);

// Add desired resource view columns
var rscCol = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(rscCol);

// Add desired assignment view columns
var assnCol = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assnCol);

// set encoding
options.Encoding = Encoding.Unicode;

project.Save(OutDir + "UsingXlsxOptions_out.xlsx", options);
```

### See Also

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


