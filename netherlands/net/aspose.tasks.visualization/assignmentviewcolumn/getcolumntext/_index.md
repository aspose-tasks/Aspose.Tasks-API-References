---
title: "AssignmentViewColumn.GetColumnText"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "AssignmentViewColumn methode. Converteert de huidige resource-opdracht naar de kolomtekst"
type: docs
weight: 30
url: /nl/net/aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/
---
## AssignmentViewColumn.GetColumnText method

Converteert de huidige resource‑toewijzing naar de kolomtekst.

```csharp
public string GetColumnText(ResourceAssignment assignment)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| toewijzing | ResourceAssignment | Huidige opdracht. |

### Retourwaarde

De kolomtekst.

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

* class [ResourceAssignment](../../../aspose.tasks/resourceassignment/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


