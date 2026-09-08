---
title: "클래스 Gridlines"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.Gridlines 클래스. GanttChart 보기에서 표시되는 그리드 라인을 나타냅니다."
type: docs
weight: 3120
url: /ko/net/aspose.tasks.visualization/gridlines/
---
## Gridlines class

GanttChart 보기에서 나타나는 격자선을 나타냅니다.

```csharp
public class Gridlines
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Gridlines](gridlines/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Interval](../../aspose.tasks.visualization/gridlines/interval/) { get; set; } | 그리드 라인 사이의 간격을 지정하는 0에서 99 사이의 값을 가져오거나 설정합니다. |
| [IntervalColor](../../aspose.tasks.visualization/gridlines/intervalcolor/) { get; set; } | 보조 그리드 라인의 색상을 가져오거나 설정합니다. |
| [IntervalPattern](../../aspose.tasks.visualization/gridlines/intervalpattern/) { get; set; } | 보조 격자선의 선 패턴을 가져오거나 설정합니다. |
| [NormalColor](../../aspose.tasks.visualization/gridlines/normalcolor/) { get; set; } | 일반 격자선의 색상을 가져오거나 설정합니다. |
| [NormalPattern](../../aspose.tasks.visualization/gridlines/normalpattern/) { get; set; } | 일반 격자선의 선 패턴을 가져오거나 설정합니다. |
| [Type](../../aspose.tasks.visualization/gridlines/type/) { get; set; } | 격자선 유형을 가져오거나 설정합니다. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


