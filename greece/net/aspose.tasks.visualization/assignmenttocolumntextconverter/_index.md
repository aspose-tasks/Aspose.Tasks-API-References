---
title: "Αντιπρόσωπος AssignmentToColumnTextConverter"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μετατροπέας δεδομένων ResourceAssignment σε συμβολοσειρά στήλων"
type: docs
weight: 2920
url: /el/net/aspose.tasks.visualization/assignmenttocolumntextconverter/
---
## AssignmentToColumnTextConverter delegate

Μετατροπέας δεδομένων ResourceAssignment σε συμβολοσειρά στήλης.

```csharp
public delegate string AssignmentToColumnTextConverter(ResourceAssignment assignment);
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ανάθεση | ResourceAssignment | Η ανάθεση για μετατροπή. |

### Τιμή Επιστροφής

Συμβολοσειρά δεδομένων για τη στήλη.

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

* class [ResourceAssignment](../../aspose.tasks/resourceassignment/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


