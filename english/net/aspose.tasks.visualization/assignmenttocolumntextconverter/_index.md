---
title: Delegate AssignmentToColumnTextConverter
second_title: Aspose.Tasks for .NET API Reference
description: ResourceAssignment data to columns string converter
type: docs
weight: 2840
url: /net/aspose.tasks.visualization/assignmenttocolumntextconverter/
---
## AssignmentToColumnTextConverter delegate

ResourceAssignment data to column's string converter.

```csharp
public delegate string AssignmentToColumnTextConverter(ResourceAssignment assignment);
```

| Parameter | Type | Description |
| --- | --- | --- |
| assignment | ResourceAssignment | The assignment to convert. |

### Return Value

String data for the column.

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

* class [ResourceAssignment](../../aspose.tasks/resourceassignment/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


