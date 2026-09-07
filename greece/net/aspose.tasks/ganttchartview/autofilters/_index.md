---
title: "GanttChartView.AutoFilters"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "GanttChartView ιδιότητα. Λαμβάνει μια λίστα αυτόματων φίλτρων μιας προβολής Gantt Chart"
type: docs
weight: 20
url: /el/net/aspose.tasks/ganttchartview/autofilters/
---
## GanttChartView.AutoFilters property

Λαμβάνει μια λίστα αυτόματων φίλτρων μιας προβολής Gantt Chart.

```csharp
public FilterCollection AutoFilters { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τα αυτόματα φίλτρα μιας προβολής διαγράμματος Gantt.

```csharp
var project = new Project(DataDir + "AutoFilterOnFinishColumn.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.First(v => v.Screen == ViewScreen.Gantt);

// επιτρέπει την επανάληψη στα αυτόματα φίλτρα της προβολής διαγράμματος Gantt
foreach (var filter in view.AutoFilters)
{
    Console.WriteLine("Criteria: " + filter.Criteria);

    Console.WriteLine("Criteria field: " + filter.Criteria.Field);
    Console.WriteLine("Criteria test condition: " + filter.Criteria.Test);
    Console.WriteLine("Criteria values: " + string.Join(", ", filter.Criteria.Values.Where(c => c != null)));
    Console.WriteLine();
}

// εργαστείτε με το έργο...
```

### Δείτε επίσης

* class [FilterCollection](../../filtercollection/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


