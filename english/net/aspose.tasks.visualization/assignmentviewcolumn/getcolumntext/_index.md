---
title: AssignmentViewColumn.GetColumnText
second_title: Aspose.Tasks for .NET API Reference
description: AssignmentViewColumn method. Converts current resource assignment to the column text
type: docs
weight: 30
url: /net/aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/
---
## AssignmentViewColumn.GetColumnText method

Converts current resource assignment to the column text.

```csharp
public string GetColumnText(ResourceAssignment assignment)
```

| Parameter | Type | Description |
| --- | --- | --- |
| assignment | ResourceAssignment | Current assignment. |

### Return Value

The column text.

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

* class [ResourceAssignment](../../../aspose.tasks/resourceassignment/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


