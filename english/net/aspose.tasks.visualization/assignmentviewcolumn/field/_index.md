---
title: AssignmentViewColumn.Field
second_title: Aspose.Tasks for .NET API Reference
description: AssignmentViewColumn property. Column field. Field
type: docs
weight: 20
url: /net/aspose.tasks.visualization/assignmentviewcolumn/field/
---
## AssignmentViewColumn.Field property

Column field. `Field`.

```csharp
public override Field Field { get; set; }
```

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

* enum [Field](../../../aspose.tasks/field/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


