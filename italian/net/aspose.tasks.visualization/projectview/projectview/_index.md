---
title: "ProjectView.ProjectView"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore ProjectView. Inizializza una nuova istanza della classe ProjectView"
type: docs
weight: 10
url: /it/net/aspose.tasks.visualization/projectview/projectview/
---
## ProjectView constructor

Inizializza una nuova istanza della classe [`ProjectView`](../).

```csharp
public ProjectView(IEnumerable<ViewColumn> columns)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonne | IEnumerable`1 | Un elenco delle colonne della vista. |

## Esempi

Mostra come salvare un progetto con una vista con un set personalizzato di colonne.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new GanttChartColumn("Name", 100, Field.TaskName),
    new GanttChartColumn("Start", 100, Field.TaskStart),
    new GanttChartColumn("Finish", 100, Field.TaskFinish),
    new GanttChartColumn("Cost2", 80, Field.TaskCost2),
    new GanttChartColumn("Number6", 80, Field.TaskNumber6),
    new GanttChartColumn("Date6", 80, Field.TaskDate6),
    new GanttChartColumn("Flag6", 80, Field.TaskFlag6),
    new GanttChartColumn("Flag18", 80, Field.TaskFlag18),
    new GanttChartColumn("Duration6", 80, Field.TaskDuration6)
};
options.View = new ProjectView(columns);

// itera sulle colonne della vista
foreach (var column in options.View.Columns)
{
    Console.WriteLine("Column Name: " + column.Name);
}

options.PresentationFormat = PresentationFormat.TaskUsage;
project.Save(OutDir + "TaskUsageProjectView_Columns.pdf", options);
```

### Vedi anche

* class [ViewColumn](../../viewcolumn/)
* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


