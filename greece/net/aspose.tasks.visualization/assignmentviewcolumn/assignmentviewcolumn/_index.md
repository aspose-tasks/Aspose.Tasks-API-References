---
title: "AssignmentViewColumn.AssignmentViewColumn"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής AssignmentViewColumn. Αρχικοποιεί μια νέα παρουσία της κλάσης AssignmentViewColumn"
type: docs
weight: 10
url: /el/net/aspose.tasks.visualization/assignmentviewcolumn/assignmentviewcolumn/
---
## AssignmentViewColumn constructor

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης AssignmentViewColumn.

```csharp
public AssignmentViewColumn(string name, int width, AssignmentToColumnTextConverter converter)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Όνομα στήλης. |
| πλάτος | Int32 | Πλάτος στήλης σε εικονοστοιχεία. |
| μετατροπέας | AssignmentToColumnTextConverter | Μετατροπέας δεδομένων ανάθεσης σε κείμενο στήλης. |

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

* delegate [AssignmentToColumnTextConverter](../../assignmenttocolumntextconverter/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


