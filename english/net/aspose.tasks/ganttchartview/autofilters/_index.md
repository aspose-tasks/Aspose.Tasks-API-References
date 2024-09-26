---
title: GanttChartView.AutoFilters
second_title: Aspose.Tasks for .NET API Reference
description: GanttChartView property. Gets a list of auto filters of a Gantt Chart view
type: docs
weight: 20
url: /net/aspose.tasks/ganttchartview/autofilters/
---
## GanttChartView.AutoFilters property

Gets a list of auto filters of a Gantt Chart view.

```csharp
public FilterCollection AutoFilters { get; }
```

## Examples

Shows how to read auto filters of a Gantt chart view.

```csharp
var project = new Project(DataDir + "AutoFilterOnFinishColumn.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.First(v => v.Screen == ViewScreen.Gantt);

// lets iterate over auto filters of the Gantt chart view
foreach (var filter in view.AutoFilters)
{
    Console.WriteLine("Criteria: " + filter.Criteria);

    Console.WriteLine("Criteria field: " + filter.Criteria.Field);
    Console.WriteLine("Criteria test condition: " + filter.Criteria.Test);
    Console.WriteLine("Criteria values: " + string.Join(", ", filter.Criteria.Values.Where(c => c != null)));
    Console.WriteLine();
}

// work with the project...
```

### See Also

* class [FilterCollection](../../filtercollection/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


