---
title: "열거형 Interval"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.Interval 열거형. 진행 라인을 표시할 반복 간격을 지정합니다"
type: docs
weight: 3170
url: /ko/net/aspose.tasks.visualization/interval/
---
## Interval enumeration

진행선을 표시할 반복 간격을 지정합니다.

```csharp
public enum Interval
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Daily | `0` | 일일 간격을 나타냅니다. |
| Weekly | `1` | 주간 간격을 나타냅니다. |
| Monthly | `2` | 월간 간격을 나타냅니다. |

## 예제

진행 라인의 반복 간격을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

// 진행 라인을 읽습니다
var interval = view.ProgressLines.RecurringInterval;

Console.WriteLine("Interval: " + interval.Interval);
Console.WriteLine("Weekly Week Number: " + interval.WeeklyWeekNumber);
foreach (var day in interval.WeeklyDays)
{
    Console.WriteLine("Week day: " + day);
}

// 반복 간격을 재정의합니다
var newInterval = new RecurringInterval();

// 월별 진행 라인을 일별로 표시할지 여부를 나타내는 값을 설정합니다.
interval.MonthlyDay = true;
// 월별 진행 라인의 일 번호를 설정합니다.
interval.MonthlyDayDayNumber = 1;
// 월별 진행 라인의 월 번호를 설정합니다.
interval.MonthlyDayMonthNumber = 1;
// 첫 번째 또는 마지막 미리 정의된 일에 따라 진행 라인을 표시할지 여부를 나타내는 값을 설정합니다.
interval.MonthlyFirstLast = true;
// 월별 진행 라인의 첫 번째 또는 마지막 일 유형을 설정합니다.
interval.MonthlyFirstLastDay = RecurringInterval.DayType.Day;
// 첫 번째 또는 마지막 미리 정의된 일에 따라 표시되는 진행 라인의 월 번호를 설정합니다.
interval.MonthlyFirstLastMonthNumber = 1;

view.ProgressLines.RecurringInterval = newInterval;

project.Save(OutDir + "WorkWithRecurringInterval_out.pdf", SaveFileFormat.Pdf);
```

### 또 보기

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


