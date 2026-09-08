---
title: "GanttChartView.AutoFilters"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GanttChartView 속성. Gantt Chart 보기의 자동 필터 목록을 가져옵니다"
type: docs
weight: 20
url: /ko/net/aspose.tasks/ganttchartview/autofilters/
---
## GanttChartView.AutoFilters property

Gantt 차트 뷰의 자동 필터 목록을 가져옵니다.

```csharp
public FilterCollection AutoFilters { get; }
```

## 예제

Gantt 차트 보기의 자동 필터를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "AutoFilterOnFinishColumn.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.First(v => v.Screen == ViewScreen.Gantt);

// Gantt 차트 보기의 자동 필터를 반복합니다.
foreach (var filter in view.AutoFilters)
{
    Console.WriteLine("Criteria: " + filter.Criteria);

    Console.WriteLine("Criteria field: " + filter.Criteria.Field);
    Console.WriteLine("Criteria test condition: " + filter.Criteria.Test);
    Console.WriteLine("Criteria values: " + string.Join(", ", filter.Criteria.Values.Where(c => c != null)));
    Console.WriteLine();
}

// 프로젝트와 작업...
```

### 또 보기

* class [FilterCollection](../../filtercollection/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


