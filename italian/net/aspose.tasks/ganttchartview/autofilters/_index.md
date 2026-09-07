---
title: "GanttChartView.AutoFilters"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà GanttChartView. Restituisce un elenco di filtri automatici di una vista Gantt Chart"
type: docs
weight: 20
url: /it/net/aspose.tasks/ganttchartview/autofilters/
---
## GanttChartView.AutoFilters property

Ottiene un elenco di filtri automatici di una vista Gantt Chart.

```csharp
public FilterCollection AutoFilters { get; }
```

## Esempi

Mostra come leggere i filtri automatici della vista Gantt chart.

```csharp
var project = new Project(DataDir + "AutoFilterOnFinishColumn.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.First(v => v.Screen == ViewScreen.Gantt);

// Consente di iterare sui filtri automatici della vista Gantt chart.
foreach (var filter in view.AutoFilters)
{
    Console.WriteLine("Criteria: " + filter.Criteria);

    Console.WriteLine("Criteria field: " + filter.Criteria.Field);
    Console.WriteLine("Criteria test condition: " + filter.Criteria.Test);
    Console.WriteLine("Criteria values: " + string.Join(", ", filter.Criteria.Values.Where(c => c != null)));
    Console.WriteLine();
}

// lavorare con il progetto...
```

### Vedi anche

* class [FilterCollection](../../filtercollection/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


