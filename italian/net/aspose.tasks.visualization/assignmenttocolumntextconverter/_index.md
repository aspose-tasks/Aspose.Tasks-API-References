---
title: "Delegato AssignmentToColumnTextConverter"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Convertitore di stringhe dei dati ResourceAssignment in colonne"
type: docs
weight: 2920
url: /it/net/aspose.tasks.visualization/assignmenttocolumntextconverter/
---
## AssignmentToColumnTextConverter delegate

Convertitore da dati ResourceAssignment a stringa della colonna.

```csharp
public delegate string AssignmentToColumnTextConverter(ResourceAssignment assignment);
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| assegnazione | ResourceAssignment | L'assegnazione da convertire. |

### Valore di ritorno

Dati stringa per la colonna.

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

* class [ResourceAssignment](../../aspose.tasks/resourceassignment/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


