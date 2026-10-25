---
title: "GanttBarStyle.ShowForTaskUid"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GanttBarStyle 속성. 스타일이 적용되는 작업의 고유 ID를 가져오거나 설정합니다. 간트 차트에서 막대의 작업별 스타일에 적용됩니다. CustomBarStyles를 참조하십시오."
type: docs
weight: 210
url: /ko/net/aspose.tasks.visualization/ganttbarstyle/showfortaskuid/
---
## GanttBarStyle.ShowForTaskUid property

스타일이 적용되는 작업의 고유 ID를 가져오거나 설정합니다. 간트 차트에서 막대의 작업별 스타일에 적용됩니다 (참조 [`CustomBarStyles`](../../../aspose.tasks/ganttchartview/custombarstyles/)).

```csharp
public int? ShowForTaskUid { get; set; }
```

## 예제

ShowFor 카테고리를 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var view = (GanttChartView)project.DefaultView;

var barStyle = this.GetCustomBarStyle();
barStyle.ShowForTaskUid = null;

var showForCategories = new[]
{
    GanttBarShowFor.Active,
    GanttBarShowFor.NotSummary,
    GanttBarShowFor.Milestone,
    GanttBarShowFor.Finished
};

barStyle.ShowForCategories = new List<GanttBarShowFor>(showForCategories);
barStyle.Name = "My common style";
view.BarStyles.Add(barStyle);

// 프로젝트 작업...
```

### 또 보기

* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


