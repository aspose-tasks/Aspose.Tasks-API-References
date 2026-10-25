---
title: "Κλάση AssignmentViewColumn"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Visualization.AssignmentViewColumn. Κλάση προβολής έργων"
type: docs
weight: 2930
url: /el/net/aspose.tasks.visualization/assignmentviewcolumn/
---
## AssignmentViewColumn class

Κλάση προβολής του έργου.

```csharp
public class AssignmentViewColumn : ViewColumn
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [AssignmentViewColumn](assignmentviewcolumn/)(string, int, AssignmentToColumnTextConverter) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης AssignmentViewColumn. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/assignmentviewcolumn/field/) { get; set; } | Πεδίο στήλης. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Λαμβάνει το όνομα της στήλης. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Λαμβάνει ή ορίζει την ευθυγράμμιση του κειμένου (μπορεί να είναι μία από τις τιμές της απαρίθμησης [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Λαμβάνει ή ορίζει την κλήση επιστροφής (callback) που μπορεί να χρησιμοποιηθεί για την προσαρμογή της εμφάνισης των κελιών της στήλης. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Λαμβάνει το πλάτος της στήλης. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/)(ResourceAssignment) | Μετατρέπει την τρέχουσα ανάθεση πόρων σε κείμενο στήλης. |

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

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


