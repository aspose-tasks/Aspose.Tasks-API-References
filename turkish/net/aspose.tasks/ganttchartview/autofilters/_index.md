---
title: "GanttChartView.AutoFilters"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "GanttChartView özelliği. Gantt Chart görünümünün otomatik filtrelerinin bir listesini alır"
type: docs
weight: 20
url: /tr/net/aspose.tasks/ganttchartview/autofilters/
---
## GanttChartView.AutoFilters property

Bir Gantt Chart görünümünün otomatik filtreler listesini alır.

```csharp
public FilterCollection AutoFilters { get; }
```

## Örnekler

Bir Gantt şeması görünümünün otomatik filtrelerini nasıl okuyacağını gösterir.

```csharp
var project = new Project(DataDir + "AutoFilterOnFinishColumn.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.First(v => v.Screen == ViewScreen.Gantt);

// Gantt şeması görünümünün otomatik filtreleri üzerinde yineleme yapar
foreach (var filter in view.AutoFilters)
{
    Console.WriteLine("Criteria: " + filter.Criteria);

    Console.WriteLine("Criteria field: " + filter.Criteria.Field);
    Console.WriteLine("Criteria test condition: " + filter.Criteria.Test);
    Console.WriteLine("Criteria values: " + string.Join(", ", filter.Criteria.Values.Where(c => c != null)));
    Console.WriteLine();
}

// projeyle çalış...
```

### Ayrıca Bakınız

* class [FilterCollection](../../filtercollection/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


