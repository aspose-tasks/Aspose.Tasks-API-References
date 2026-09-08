---
title: "Klasse AssignmentViewColumn"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.AssignmentViewColumn‑klasse. Projectweergave‑klasse"
type: docs
weight: 2930
url: /nl/net/aspose.tasks.visualization/assignmentviewcolumn/
---
## AssignmentViewColumn class

Klasse van projectweergave.

```csharp
public class AssignmentViewColumn : ViewColumn
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [AssignmentViewColumn](assignmentviewcolumn/)(string, int, AssignmentToColumnTextConverter) | Initialiseert een nieuw exemplaar van de AssignmentViewColumn‑klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/assignmentviewcolumn/field/) { get; set; } | Kolomveld. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Haalt de kolomnaam op. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Haalt de uitlijning van de tekst op of stelt deze in (kan een van de waarden van de enumeratie [`HorizontalStringAlignment`](../horizontalstringalignment/) zijn). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Haalt de callback op of stelt deze in die kan worden gebruikt om het uiterlijk van de cellen van de kolom aan te passen. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Haalt de kolombreedte op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/)(ResourceAssignment) | Converteert de huidige resource‑toewijzing naar de kolomtekst. |

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

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


