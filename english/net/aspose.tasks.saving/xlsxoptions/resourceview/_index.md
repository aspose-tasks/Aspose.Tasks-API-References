---
title: XlsxOptions.ResourceView
second_title: Aspose.Tasks for .NET API Reference
description: XlsxOptions property. Gets or sets a list of the resource view columns to render ResourceViewColumn
type: docs
weight: 40
url: /net/aspose.tasks.saving/xlsxoptions/resourceview/
---
## XlsxOptions.ResourceView property

Gets or sets a list of the resource view columns to render ([`ResourceViewColumn`](../../../aspose.tasks.visualization/resourceviewcolumn/)).

```csharp
public ProjectView ResourceView { get; set; }
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


