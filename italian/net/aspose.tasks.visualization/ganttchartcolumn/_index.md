---
title: "Classe GanttChartColumn"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Visualization.GanttChartColumn. Classe di visualizzazione dei progetti"
type: docs
weight: 3090
url: /it/net/aspose.tasks.visualization/ganttchartcolumn/
---
## GanttChartColumn class

Classe di visualizzazione del progetto

```csharp
public sealed class GanttChartColumn : ViewColumn
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GanttChartColumn](ganttchartcolumn/#constructor)(int, Field) | Inizializza una nuova istanza della classe GanttChartColumn. |
| [GanttChartColumn](ganttchartcolumn/#constructor_1)(string, int, Field) | Inizializza una nuova istanza della classe GanttChartColumn. |
| [GanttChartColumn](ganttchartcolumn/#constructor_2)(string, int, TaskToColumnTextConverter) | Inizializza una nuova istanza della classe GanttChartColumn. |
| [GanttChartColumn](ganttchartcolumn/#constructor_3)(string, int, TaskToColumnTextConverter, Field) | Inizializza una nuova istanza della classe GanttChartColumn. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/ganttchartcolumn/field/) { get; set; } | Campo colonna. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Ottiene il nome della colonna. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Ottiene o imposta l'allineamento del testo (può essere uno dei valori dell'enumerazione [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Ottiene o imposta il callback che può essere usato per personalizzare l'aspetto delle celle della colonna. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Ottiene la larghezza della colonna. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/ganttchartcolumn/getcolumntext/)(Task) | Converte l'attività corrente nel testo della colonna. |

## Esempi

Mostra come aggiungere colonne della vista Gantt chart da esportare.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.GetById(1);

var columns = new List<ViewColumn>
{
    new GanttChartColumn(20, Field.TaskUniqueID),
    new GanttChartColumn("Name", 150, Field.TaskName),
    new GanttChartColumn("Start", 100, Field.TaskStart),
    new GanttChartColumn("End", 100, Field.TaskFinish),
    new GanttChartColumn("R-Initials", 100, Field.TaskResourceInitials),
    new GanttChartColumn("R-Names", 100, Field.TaskResourceNames),
    new GanttChartColumn("Work", 50, Field.TaskWork),
    new GanttChartColumn(
        "Cost", 
        80,
        delegate(Task t)
        {
            return t.Get(Tsk.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new GanttChartColumn(
        "Actual Cost", 
        80,
        delegate(Task t)
        {
            return t.Get(Tsk.ActualCost).ToString(CultureInfo.InvariantCulture);
        },
        Field.TaskActualCost)
};

// itera sulle colonne
foreach (var column in columns)
{
    var col = (GanttChartColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(task));
    Console.WriteLine();
}

var options = new CsvOptions
{
    View = new ProjectView(columns)
};

project.Save(OutDir + "WorkWithGanttChartColumn_out.csv", options);
```

### Vedi anche

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


