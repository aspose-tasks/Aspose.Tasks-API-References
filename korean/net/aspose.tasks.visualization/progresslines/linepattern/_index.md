---
title: "ProgressLines.LinePattern"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProgressLines 속성. 현재 진행 라인의 선 패턴을 가져오거나 설정합니다. LinePattern"
type: docs
weight: 110
url: /ko/net/aspose.tasks.visualization/progresslines/linepattern/
---
## ProgressLines.LinePattern property

현재 진행 라인의 선 패턴을 가져오거나 설정합니다. `LinePattern`.

```csharp
public LinePattern LinePattern { get; set; }
```

## 예제

진행 라인 작업 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// 진행 라인을 정의합니다.
view.ProgressLines = new ProgressLines();
var progressLines = view.ProgressLines;

// 진행 라인을 표시할 시작 날짜를 설정합니다. 프로젝트의 상태 날짜를 설정해 보겠습니다.
progressLines.BeginAtDate = project.Get(Prj.StatusDate);
// 프로젝트 시작 날짜부터 진행 라인을 표시할지 여부를 나타내는 값을 설정합니다.
progressLines.BeginAtProjectStart = true;
// 날짜 형식을 설정합니다 (<see cref="T:Aspose.Tasks.Visualization.DateLabel" />).
progressLines.DateFormat = DateLabel.DayDddd;
// 현재 날짜에 진행 라인을 표시할지 여부를 나타내는 값을 설정합니다.
progressLines.DisplayAtCurrentDate = true;
// 반복 간격으로 진행 라인을 표시할지 여부를 나타내는 값을 설정합니다.
progressLines.DisplayAtRecurringIntervals = true;
// 선택한 날짜에 진행 라인을 표시할지 여부를 나타내는 값을 설정합니다.
progressLines.DisplaySelected = true;
// 기준선 계획 또는 실제에 대한 진행 라인을 표시할지 여부를 나타내는 값을 설정합니다.
progressLines.IsBaselinePlan = false;
// 진행 라인 레이블에 사용할 글꼴을 설정합니다.
progressLines.Font = new FontDescriptor("Arial", 10);
// 현재 진행 라인의 선 색상을 설정합니다.
progressLines.LineColor = Color.Aquamarine;
// 현재 진행 라인의 선 패턴을 설정합니다.
progressLines.LinePattern = LinePattern.Dashed;
// 다른 진행 라인의 색상을 설정합니다.
progressLines.OtherLineColor = Color.Azure;
// 다른 진행 라인의 선 패턴을 설정합니다.
progressLines.OtherLinePattern = LinePattern.Dotted;
// 다른 진행 포인트의 색상을 설정합니다.
progressLines.OtherProgressPointColor = Color.Red;
// 다른 진행 라인의 진행 포인트 모양을 설정합니다.
progressLines.OtherProgressPointShape = GanttBarEndShape.Circle;
// 진행 포인트의 색상을 설정합니다.
progressLines.ProgressPointColor = Color.Orange;
// 진행 지점 모양을 설정합니다.
progressLines.ProgressPointShape = GanttBarEndShape.Diamond;
// 반복 간격을 설정합니다.
progressLines.RecurringInterval = new RecurringInterval();
// 반복 간격을 설정합니다.
progressLines.RecurringInterval.Interval = Interval.Daily;
// 각 진행 라인에 날짜를 표시할지 여부를 나타내는 값을 설정합니다.
progressLines.RecurringInterval.DailyDayNumber = 1;
// 진행 라인을 확인해 봅시다
progressLines.ShowDate = true;

// 클래스 TimescaleTier
Console.WriteLine("Begin At Date: " + progressLines.BeginAtDate);
Console.WriteLine("Begin At Project Start: " + progressLines.BeginAtProjectStart);
Console.WriteLine("Date Format: " + progressLines.DateFormat);
Console.WriteLine("Display At Current Date: " + progressLines.DisplayAtCurrentDate);
Console.WriteLine("Display At Recurring Intervals: " + progressLines.DisplayAtRecurringIntervals);
Console.WriteLine("Display Selected: " + progressLines.DisplaySelected);
Console.WriteLine("Font: " + progressLines.Font);
Console.WriteLine("Is Baseline Plan: " + progressLines.IsBaselinePlan);
Console.WriteLine("Line Color: " + progressLines.LineColor);
Console.WriteLine("Line Pattern: " + progressLines.LinePattern);
Console.WriteLine("Other Line Color: " + progressLines.OtherLineColor);
Console.WriteLine("Other Line Pattern: " + progressLines.OtherLinePattern);
Console.WriteLine("Other Progress Point Color: " + progressLines.OtherProgressPointColor);
Console.WriteLine("Other Progress Point Shape: " + progressLines.OtherProgressPointShape);
Console.WriteLine("Progress Point Color: " + progressLines.ProgressPointColor);
Console.WriteLine("Progress Point Shape: " + progressLines.ProgressPointShape);
Console.WriteLine("Recurring Interval: " + progressLines.RecurringInterval.Interval);
Console.WriteLine("Recurring Interval DailyDayNumber: " + progressLines.RecurringInterval.DailyDayNumber);
Console.WriteLine("Selected Dates: ");
foreach (var date in progressLines.SelectedDates)
{
    Console.WriteLine("Date: " + date);
}
Console.WriteLine("Show Date: " + progressLines.ShowDate);
Console.WriteLine();

project.Save(OutDir + "WorkWithProgressLines_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* enum [LinePattern](../../linepattern/)
* class [ProgressLines](../)
* namespace [Aspose.Tasks.Visualization](../../progresslines/)
* assembly [Aspose.Tasks](../../../)


