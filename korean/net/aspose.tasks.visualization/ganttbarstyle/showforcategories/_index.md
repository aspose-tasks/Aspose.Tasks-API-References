---
title: "GanttBarStyle.ShowForCategories"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GanttBarStyle 속성. 스타일이 적용되는 작업 카테고리를 가져오거나 설정합니다. 간트 차트의 막대에 대한 상위 또는 공통 스타일에 적용됩니다. BarStyles를 참조하십시오."
type: docs
weight: 200
url: /ko/net/aspose.tasks.visualization/ganttbarstyle/showforcategories/
---
## GanttBarStyle.ShowForCategories property

스타일이 적용되는 작업 카테고리를 가져오거나 설정합니다. 간트 차트의 막대에 대한 상위(또는 공통) 스타일에 적용됩니다([`BarStyles`](../../../aspose.tasks/ganttchartview/barstyles/)를 참조).

```csharp
public IList<GanttBarShowFor> ShowForCategories { get; set; }
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

* enum [GanttBarShowFor](../../ganttbarshowfor/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


