---
title: "GanttChartView.AutoFilters"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad de GanttChartView. Obtiene una lista de filtros automáticos de una vista de diagrama de Gantt"
type: docs
weight: 20
url: /es/net/aspose.tasks/ganttchartview/autofilters/
---
## GanttChartView.AutoFilters property

Obtiene una lista de filtros automáticos de una vista Gantt Chart.

```csharp
public FilterCollection AutoFilters { get; }
```

## Ejemplos

Muestra cómo leer los filtros automáticos de una vista de diagrama de Gantt.

```csharp
var project = new Project(DataDir + "AutoFilterOnFinishColumn.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.First(v => v.Screen == ViewScreen.Gantt);

// Permite iterar sobre los filtros automáticos de la vista de diagrama de Gantt
foreach (var filter in view.AutoFilters)
{
    Console.WriteLine("Criteria: " + filter.Criteria);

    Console.WriteLine("Criteria field: " + filter.Criteria.Field);
    Console.WriteLine("Criteria test condition: " + filter.Criteria.Test);
    Console.WriteLine("Criteria values: " + string.Join(", ", filter.Criteria.Values.Where(c => c != null)));
    Console.WriteLine();
}

// trabajar con el proyecto...
```

### Ver también

* class [FilterCollection](../../filtercollection/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


