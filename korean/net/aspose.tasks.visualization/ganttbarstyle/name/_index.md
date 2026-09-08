---
title: "GanttBarStyle.Name"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GanttBarStyle 속성. 스타일의 이름을 가져오거나 설정합니다."
type: docs
weight: 150
url: /ko/net/aspose.tasks.visualization/ganttbarstyle/name/
---
## GanttBarStyle.Name property

스타일의 이름을 가져오거나 설정합니다.

```csharp
public string Name { get; set; }
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


