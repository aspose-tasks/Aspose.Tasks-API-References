---
title: "GanttChartView.ShowBarSplits"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GanttChartView 속성. Gantt Chart에서 작업 분할을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다"
type: docs
weight: 140
url: /ko/net/aspose.tasks/ganttchartview/showbarsplits/
---
## GanttChartView.ShowBarSplits property

Gantt 차트의 작업 분할을 표시해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool ShowBarSplits { get; set; }
```

## 예제

Gantt 차트 보기의 몇 가지 유용한 속성을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// 바가 가장 가까운 날로 반올림되는지 여부를 나타내는 값을 설정합니다.
view.BarRounding = false;
// Gantt 차트에서 Gantt 바의 높이를 포인트 단위로 설정합니다.
view.BarSize = GanttBarSize.BarSize24;
// 요약 작업을 확장할 때 롤업 바가 숨겨지는지 여부를 나타내는 값을 설정합니다.
view.HideRollupBarsWhenSummaryExpanded = true;
// 비작업 시간 색상을 설정합니다.
view.NonWorkingTimeColor = Color.Azure;
// Gantt 차트의 바를 롤업해야 하는지 여부를 나타내는 값을 설정합니다.
view.RollUpGanttBars = true;
// Gantt 차트에서 작업 분할을 표시해야 하는지 여부를 나타내는 값을 설정합니다.
view.ShowBarSplits = true;
// Gantt 차트에서 도면을 표시해야 하는지 여부를 나타내는 값을 설정합니다.
view.ShowDrawings = true;
// 시간 눈금 단계의 단위 사이 간격을 줄이거나 확대하는 비율을 설정합니다.
view.TimescaleSizePercentage = 10;

project.Save(OutDir + "WorkWithGanttChartViews_out.pdf", SaveFileFormat.Pdf);
```

### 또 보기

* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


