---
title: "Gridlines.IntervalPattern"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Gridlines 속성. 보조 그리드선의 선 패턴을 가져오거나 설정합니다"
type: docs
weight: 40
url: /ko/net/aspose.tasks.visualization/gridlines/intervalpattern/
---
## Gridlines.IntervalPattern property

보조 격자선의 선 패턴을 가져오거나 설정합니다.

```csharp
public LinePattern IntervalPattern { get; set; }
```

## 예제

격자선을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var view = (GanttChartView)project.Views.ToList()[0];

// 뷰의 첫 번째 격자선을 조정합니다.
var gridlines = view.Gridlines[0];
// 격자선 사이 간격을 지정하는 0부터 99까지의 숫자를 설정합니다.
gridlines.Interval = 2;
// 보조 격자선의 색상을 설정합니다.
gridlines.IntervalColor = Color.Red;
// 보조 격자선의 선 패턴을 설정합니다.
gridlines.IntervalPattern = LinePattern.Solid;
// 일반 격자선의 색상을 설정합니다.
gridlines.NormalColor = Color.Blue;
// 일반 격자선의 선 패턴을 설정합니다.
gridlines.NormalPattern = LinePattern.CloseDot;
// 격자선 유형을 설정합니다.
gridlines.Type = GridlineType.GanttRow;

project.Save(OutDir + "WorkWithGridlines_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* enum [LinePattern](../../linepattern/)
* class [Gridlines](../)
* namespace [Aspose.Tasks.Visualization](../../gridlines/)
* assembly [Aspose.Tasks](../../../)


