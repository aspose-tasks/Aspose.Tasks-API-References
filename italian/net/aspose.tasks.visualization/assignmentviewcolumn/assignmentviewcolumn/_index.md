---
title: "AssignmentViewColumn.AssignmentViewColumn"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore AssignmentViewColumn. Inizializza una nuova istanza della classe AssignmentViewColumn"
type: docs
weight: 10
url: /it/net/aspose.tasks.visualization/assignmentviewcolumn/assignmentviewcolumn/
---
## AssignmentViewColumn constructor

Inizializza una nuova istanza della classe AssignmentViewColumn.

```csharp
public AssignmentViewColumn(string name, int width, AssignmentToColumnTextConverter converter)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | Stringa | Nome della colonna. |
| larghezza | Int32 | Larghezza della colonna in pixel. |
| convertitore | AssignmentToColumnTextConverter | Convertitore di dati di assegnazione in testo di colonna. |

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

* delegate [AssignmentToColumnTextConverter](../../assignmenttocolumntextconverter/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


