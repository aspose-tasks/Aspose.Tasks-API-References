---
title: "GanttChartView.AutoFilters"
second_title: "Aspose.Tasks for .NET API 参考"
description: "GanttChartView 属性。获取 Gantt Chart 视图的自动过滤器列表"
type: docs
weight: 20
url: /zh/net/aspose.tasks/ganttchartview/autofilters/
---
## GanttChartView.AutoFilters property

获取甘特图视图的自动过滤器列表。

```csharp
public FilterCollection AutoFilters { get; }
```

## 示例

展示如何读取甘特图视图的自动筛选。

```csharp
var project = new Project(DataDir + "AutoFilterOnFinishColumn.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.First(v => v.Screen == ViewScreen.Gantt);

// 让我们遍历甘特图视图的自动筛选。
foreach (var filter in view.AutoFilters)
{
    Console.WriteLine("Criteria: " + filter.Criteria);

    Console.WriteLine("Criteria field: " + filter.Criteria.Field);
    Console.WriteLine("Criteria test condition: " + filter.Criteria.Test);
    Console.WriteLine("Criteria values: " + string.Join(", ", filter.Criteria.Values.Where(c => c != null)));
    Console.WriteLine();
}

// 处理项目...
```

### 另见

* class [FilterCollection](../../filtercollection/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


