---
title: "GanttChartView.AutoFilters"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية GanttChartView. يحصل على قائمة بالمرشحات التلقائية لعرض مخطط جانت"
type: docs
weight: 20
url: /ar/net/aspose.tasks/ganttchartview/autofilters/
---
## GanttChartView.AutoFilters property

يحصل على قائمة بالمرشحات التلقائية لعرض مخطط جانت.

```csharp
public FilterCollection AutoFilters { get; }
```

## الأمثلة

يعرض كيفية قراءة الفلاتر التلقائية لعرض مخطط جانت.

```csharp
var project = new Project(DataDir + "AutoFilterOnFinishColumn.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.First(v => v.Screen == ViewScreen.Gantt);

// دعنا نكرر عبر الفلاتر التلقائية لعرض مخطط جانت.
foreach (var filter in view.AutoFilters)
{
    Console.WriteLine("Criteria: " + filter.Criteria);

    Console.WriteLine("Criteria field: " + filter.Criteria.Field);
    Console.WriteLine("Criteria test condition: " + filter.Criteria.Test);
    Console.WriteLine("Criteria values: " + string.Join(", ", filter.Criteria.Values.Where(c => c != null)));
    Console.WriteLine();
}

// العمل مع المشروع...
```

### انظر أيضًا

* class [FilterCollection](../../filtercollection/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


