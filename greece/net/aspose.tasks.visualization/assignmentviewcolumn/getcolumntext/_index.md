---
title: "AssignmentViewColumn.GetColumnText"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος AssignmentViewColumn. Μετατρέπει την τρέχουσα ανάθεση πόρου σε κείμενο στήλης"
type: docs
weight: 30
url: /el/net/aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/
---
## AssignmentViewColumn.GetColumnText method

Μετατρέπει την τρέχουσα ανάθεση πόρων σε κείμενο στήλης.

```csharp
public string GetColumnText(ResourceAssignment assignment)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ανάθεση | ResourceAssignment | Τρέχουσα ανάθεση. |

### Τιμή Επιστροφής

Το κείμενο στήλης.

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

* class [ResourceAssignment](../../../aspose.tasks/resourceassignment/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


