---
title: "GanttChartView.AutoFilters"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété GanttChartView. Obtient une liste de filtres automatiques d’une vue Gantt Chart"
type: docs
weight: 20
url: /fr/net/aspose.tasks/ganttchartview/autofilters/
---
## GanttChartView.AutoFilters property

Obtient une liste de filtres automatiques d'une vue Gantt Chart.

```csharp
public FilterCollection AutoFilters { get; }
```

## Exemples

Montre comment lire les filtres automatiques d'une vue de diagramme de Gantt.

```csharp
var project = new Project(DataDir + "AutoFilterOnFinishColumn.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.First(v => v.Screen == ViewScreen.Gantt);

// Permet d'itérer sur les filtres automatiques de la vue de diagramme de Gantt
foreach (var filter in view.AutoFilters)
{
    Console.WriteLine("Criteria: " + filter.Criteria);

    Console.WriteLine("Criteria field: " + filter.Criteria.Field);
    Console.WriteLine("Criteria test condition: " + filter.Criteria.Test);
    Console.WriteLine("Criteria values: " + string.Join(", ", filter.Criteria.Values.Where(c => c != null)));
    Console.WriteLine();
}

// travailler avec le projet...
```

### Voir aussi

* class [FilterCollection](../../filtercollection/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


