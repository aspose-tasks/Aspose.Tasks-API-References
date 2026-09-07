---
title: "Classe AssignmentViewColumn"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Visualization.AssignmentViewColumn. Classe di visualizzazione dei progetti"
type: docs
weight: 2930
url: /it/net/aspose.tasks.visualization/assignmentviewcolumn/
---
## AssignmentViewColumn class

Classe di visualizzazione del progetto.

```csharp
public class AssignmentViewColumn : ViewColumn
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [AssignmentViewColumn](assignmentviewcolumn/)(string, int, AssignmentToColumnTextConverter) | Inizializza una nuova istanza della classe AssignmentViewColumn. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/assignmentviewcolumn/field/) { get; set; } | Campo colonna. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Ottiene il nome della colonna. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Ottiene o imposta l'allineamento del testo (può essere uno dei valori dell'enumerazione [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Ottiene o imposta il callback che può essere usato per personalizzare l'aspetto delle celle della colonna. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Ottiene la larghezza della colonna. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/)(ResourceAssignment) | Converte l'assegnazione della risorsa corrente nel testo della colonna. |

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

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


