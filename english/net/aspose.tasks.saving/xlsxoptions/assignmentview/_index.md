---
title: XlsxOptions.AssignmentView
second_title: Aspose.Tasks for .NET API Reference
description: XlsxOptions property. Gets or sets a list of the assignments view columns to render AssignmentViewColumn
type: docs
weight: 20
url: /net/aspose.tasks.saving/xlsxoptions/assignmentview/
---
## XlsxOptions.AssignmentView property

Gets or sets a list of the assignments view columns to render ([`AssignmentViewColumn`](../../../aspose.tasks.visualization/assignmentviewcolumn/)).

```csharp
public ProjectView AssignmentView { get; set; }
```

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

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [XlsxOptions](../)
* namespace [Aspose.Tasks.Saving](../../xlsxoptions/)
* assembly [Aspose.Tasks](../../../)


