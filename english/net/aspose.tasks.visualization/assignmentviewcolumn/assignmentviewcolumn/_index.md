---
title: AssignmentViewColumn.AssignmentViewColumn
second_title: Aspose.Tasks for .NET API Reference
description: AssignmentViewColumn constructor. Initializes a new instance of the AssignmentViewColumn class
type: docs
weight: 10
url: /net/aspose.tasks.visualization/assignmentviewcolumn/assignmentviewcolumn/
---
## AssignmentViewColumn constructor

Initializes a new instance of the AssignmentViewColumn class.

```csharp
public AssignmentViewColumn(string name, int width, AssignmentToColumnTextConverter converter)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | Column's name. |
| width | Int32 | Column's width in pixels. |
| converter | AssignmentToColumnTextConverter | Assignment data to column text converter. |

## Examples

Shows how to add columns for assignment views.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new Spreadsheet2003SaveOptions();

var column = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(column);

foreach (var assignment in project.ResourceAssignments)
{
    foreach (var col in options.AssignmentView.Columns)
    {
        var assnCol = (AssignmentViewColumn)col;
        Console.WriteLine("Column Field: " + assnCol.Field);
        Console.WriteLine("Column Text ( converted ): " + assnCol.GetColumnText(assignment));
        Console.WriteLine();
    }
}

project.Save(OutDir + "UsingSpreadsheet2003SaveOptions_out.xml", options);
```

### See Also

* delegate [AssignmentToColumnTextConverter](../../assignmenttocolumntextconverter/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


