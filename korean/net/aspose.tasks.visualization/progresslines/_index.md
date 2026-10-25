---
title: "클래스 ProgressLines"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.ProgressLines 클래스. Gantt 차트 보기에서 진행 라인을 나타냅니다"
type: docs
weight: 3290
url: /ko/net/aspose.tasks.visualization/progresslines/
---
## ProgressLines class

Gantt 차트 보기의 진행 라인을 나타냅니다.

```csharp
public class ProgressLines
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [ProgressLines](progresslines/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [BeginAtDate](../../aspose.tasks.visualization/progresslines/beginatdate/) { get; set; } | 진행 라인을 표시할 시작 날짜를 가져오거나 설정합니다. |
| [BeginAtProjectStart](../../aspose.tasks.visualization/progresslines/beginatprojectstart/) { get; set; } | 프로젝트 시작 날짜의 시작부터 진행 라인을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [DateFormat](../../aspose.tasks.visualization/progresslines/dateformat/) { get; set; } | 날짜 형식을 가져오거나 설정합니다 ([`DateLabel`](../datelabel/)). |
| [DisplayAtCurrentDate](../../aspose.tasks.visualization/progresslines/displayatcurrentdate/) { get; set; } | 현재 날짜에 진행 라인을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [DisplayAtRecurringIntervals](../../aspose.tasks.visualization/progresslines/displayatrecurringintervals/) { get; set; } | 반복 간격에 진행 라인을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [DisplaySelected](../../aspose.tasks.visualization/progresslines/displayselected/) { get; set; } | 선택된 날짜에 진행 라인을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Font](../../aspose.tasks.visualization/progresslines/font/) { get; set; } | 진행 라인 레이블에 사용되는 글꼴을 가져오거나 설정합니다. |
| [IsBaselinePlan](../../aspose.tasks.visualization/progresslines/isbaselineplan/) { get; set; } | 기준 계획 또는 실제에 대한 진행 라인을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [LineColor](../../aspose.tasks.visualization/progresslines/linecolor/) { get; set; } | 현재 진행 라인의 선 색상을 가져오거나 설정합니다. |
| [LinePattern](../../aspose.tasks.visualization/progresslines/linepattern/) { get; set; } | 현재 진행 라인의 선 패턴을 가져오거나 설정합니다. [`LinePattern`](./linepattern/). |
| [OtherLineColor](../../aspose.tasks.visualization/progresslines/otherlinecolor/) { get; set; } | 다른 진행 라인의 색상을 가져오거나 설정합니다. |
| [OtherLinePattern](../../aspose.tasks.visualization/progresslines/otherlinepattern/) { get; set; } | 다른 진행 라인의 선 패턴을 가져오거나 설정합니다. |
| [OtherProgressPointColor](../../aspose.tasks.visualization/progresslines/otherprogresspointcolor/) { get; set; } | 다른 진행 점의 색상을 가져오거나 설정합니다. |
| [OtherProgressPointShape](../../aspose.tasks.visualization/progresslines/otherprogresspointshape/) { get; set; } | 다른 진행 라인의 진행 점 모양을 가져오거나 설정합니다. |
| [ProgressPointColor](../../aspose.tasks.visualization/progresslines/progresspointcolor/) { get; set; } | 진행 점의 색상을 가져오거나 설정합니다. |
| [ProgressPointShape](../../aspose.tasks.visualization/progresslines/progresspointshape/) { get; set; } | 진행 점 모양을 가져오거나 설정합니다. [`GanttBarEndShape`](../ganttbarendshape/). |
| [RecurringInterval](../../aspose.tasks.visualization/progresslines/recurringinterval/) { get; set; } | 반복 간격을 가져오거나 설정합니다. [`RecurringInterval`](./recurringinterval/). |
| [SelectedDates](../../aspose.tasks.visualization/progresslines/selecteddates/) { get; } | 진행 라인을 표시할 선택된 날짜 목록을 가져옵니다. |
| [ShowDate](../../aspose.tasks.visualization/progresslines/showdate/) { get; set; } | 각 진행 라인에 날짜를 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


