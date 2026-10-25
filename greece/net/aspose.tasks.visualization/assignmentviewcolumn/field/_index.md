---
title: "AssignmentViewColumn.Field"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα AssignmentViewColumn. Πεδίο στήλης. Field"
type: docs
weight: 20
url: /el/net/aspose.tasks.visualization/assignmentviewcolumn/field/
---
## AssignmentViewColumn.Field property

Πεδίο στήλης. `Field`.

```csharp
public override Field Field { get; set; }
```

## Παραδείγματα

Εμφανίζει πώς να προσθέσετε στήλες για προβολές ανάθεσης.

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

### Δείτε επίσης

* enum [Field](../../../aspose.tasks/field/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


