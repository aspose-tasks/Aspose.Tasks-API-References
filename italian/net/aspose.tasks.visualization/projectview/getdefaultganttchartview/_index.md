---
title: "ProjectView.GetDefaultGanttChartView"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ProjectView. Include gli indicatori id, nome, durata, inizio e fine delle colonne delle attività"
type: docs
weight: 30
url: /it/net/aspose.tasks.visualization/projectview/getdefaultganttchartview/
---
## ProjectView.GetDefaultGanttChartView method

Include le colonne id, indicatori, nome, durata, inizio e fine attività.

```csharp
public static ProjectView GetDefaultGanttChartView()
```

### Valore di ritorno

una vista che contiene un elenco di [`GanttChartColumn`](../../ganttchartcolumn/).

## Esempi

Mostra come salvare un progetto con la vista Gantt chart.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultGanttChartView()
};

project.Save(OutDir + "WorkWithProjectView_GanttChartView_out.pdf", options);
```

### Vedi anche

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


