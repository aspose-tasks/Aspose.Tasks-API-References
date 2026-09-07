---
title: "AssignmentViewColumn.GetColumnText"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo AssignmentViewColumn. Converte l'assegnazione della risorsa corrente nel testo della colonna"
type: docs
weight: 30
url: /it/net/aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/
---
## AssignmentViewColumn.GetColumnText method

Converte l'assegnazione della risorsa corrente nel testo della colonna.

```csharp
public string GetColumnText(ResourceAssignment assignment)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| assegnazione | ResourceAssignment | Assegnazione corrente. |

### Valore di ritorno

Il testo della colonna.

## Esempi

Mostra come aggiungere colonne per le visualizzazioni delle assegnazioni.

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

### Vedi anche

* class [ResourceAssignment](../../../aspose.tasks/resourceassignment/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


