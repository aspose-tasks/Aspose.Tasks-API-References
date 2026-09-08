---
title: "Delegate AssignmentToColumnTextConverter"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceAssignment-gegevens naar kolommen tekenreeksconverter"
type: docs
weight: 2920
url: /nl/net/aspose.tasks.visualization/assignmenttocolumntextconverter/
---
## AssignmentToColumnTextConverter delegate

ResourceAssignment-gegevens naar kolomstringconverter.

```csharp
public delegate string AssignmentToColumnTextConverter(ResourceAssignment assignment);
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| toewijzing | ResourceAssignment | De toewijzing om te converteren. |

### Retourwaarde

Stringgegevens voor de kolom.

## Voorbeelden

Toont hoe kolommen toe te voegen voor toewijzingsweergaven.

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

### Zie ook

* class [ResourceAssignment](../../aspose.tasks/resourceassignment/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


