---
title: "GanttChartView.AutoFilters"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GanttChartView eigenschap. Haalt een lijst op van automatische filters van een Gantt‑diagramweergave"
type: docs
weight: 20
url: /nl/net/aspose.tasks/ganttchartview/autofilters/
---
## GanttChartView.AutoFilters property

Haalt een lijst op van automatische filters van een Gantt Chart-weergave.

```csharp
public FilterCollection AutoFilters { get; }
```

## Voorbeelden

Toont hoe automatische filters van een Gantt-diagramweergave gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "AutoFilterOnFinishColumn.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.First(v => v.Screen == ViewScreen.Gantt);

// Laten we itereren over automatische filters van de Gantt-diagramweergave.
foreach (var filter in view.AutoFilters)
{
    Console.WriteLine("Criteria: " + filter.Criteria);

    Console.WriteLine("Criteria field: " + filter.Criteria.Field);
    Console.WriteLine("Criteria test condition: " + filter.Criteria.Test);
    Console.WriteLine("Criteria values: " + string.Join(", ", filter.Criteria.Values.Where(c => c != null)));
    Console.WriteLine();
}

// werken met het project...
```

### Zie ook

* class [FilterCollection](../../filtercollection/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


