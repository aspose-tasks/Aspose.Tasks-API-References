---
title: "AssignmentViewColumn.AssignmentViewColumn"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "AssignmentViewColumn-constructeur. Initialiseert een nieuw exemplaar van de AssignmentViewColumn-klasse."
type: docs
weight: 10
url: /nl/net/aspose.tasks.visualization/assignmentviewcolumn/assignmentviewcolumn/
---
## AssignmentViewColumn constructor

Initialiseert een nieuw exemplaar van de AssignmentViewColumn‑klasse.

```csharp
public AssignmentViewColumn(string name, int width, AssignmentToColumnTextConverter converter)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | Naam van kolom. |
| breedte | Int32 | Breedte van kolom in pixels. |
| converter | AssignmentToColumnTextConverter | Converter voor opdrachtgegevens naar kolomtekst. |

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

* delegate [AssignmentToColumnTextConverter](../../assignmenttocolumntextconverter/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


