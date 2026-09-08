---
title: "GanttChartView.AutoFilters"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "GanttChartView свойство. Получает список автофильтров представления диаграммы Ганта"
type: docs
weight: 20
url: /ru/net/aspose.tasks/ganttchartview/autofilters/
---
## GanttChartView.AutoFilters property

Получает список автофильтров представления диаграммы Ганта.

```csharp
public FilterCollection AutoFilters { get; }
```

## Примеры

Показывает, как читать автоматические фильтры представления диаграммы Ганта.

```csharp
var project = new Project(DataDir + "AutoFilterOnFinishColumn.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.First(v => v.Screen == ViewScreen.Gantt);

// позволяет перебрать автоматические фильтры представления диаграммы Ганта
foreach (var filter in view.AutoFilters)
{
    Console.WriteLine("Criteria: " + filter.Criteria);

    Console.WriteLine("Criteria field: " + filter.Criteria.Field);
    Console.WriteLine("Criteria test condition: " + filter.Criteria.Test);
    Console.WriteLine("Criteria values: " + string.Join(", ", filter.Criteria.Values.Where(c => c != null)));
    Console.WriteLine();
}

// работать с проектом...
```

### См. также

* class [FilterCollection](../../filtercollection/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


