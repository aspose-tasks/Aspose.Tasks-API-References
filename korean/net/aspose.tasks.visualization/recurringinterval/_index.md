---
title: "클래스 RecurringInterval"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.RecurringInterval 클래스. 간트 차트 보기의 진행 라인에 사용되는 반복 간격을 나타냅니다"
type: docs
weight: 3310
url: /ko/net/aspose.tasks.visualization/recurringinterval/
---
## RecurringInterval class

Gantt 차트 보기의 진행 라인에 사용되는 반복 간격을 나타냅니다.

```csharp
public class RecurringInterval
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [RecurringInterval](recurringinterval/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [DailyDayNumber](../../aspose.tasks.visualization/recurringinterval/dailydaynumber/) { get; set; } | 일일 날짜 번호를 가져오거나 설정합니다. |
| [DailyWorkday](../../aspose.tasks.visualization/recurringinterval/dailyworkday/) { get; set; } | 일일 진행 라인에서 해당 날짜가 근무일인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Interval](../../aspose.tasks.visualization/recurringinterval/interval/) { get; set; } | 반복 간격을 가져오거나 설정합니다. [`Interval`](./interval/) 유형의 모든 값을 사용할 수 있습니다. |
| [MonthlyDay](../../aspose.tasks.visualization/recurringinterval/monthlyday/) { get; set; } | 월별 진행 라인을 일별로 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [MonthlyDayDayNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaydaynumber/) { get; set; } | 월별 진행 라인의 일 번호를 가져오거나 설정합니다. |
| [MonthlyDayMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaymonthnumber/) { get; set; } | 월별 진행 라인의 월 번호를 가져오거나 설정합니다. |
| [MonthlyFirstLast](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlast/) { get; set; } | 첫 번째 또는 마지막 미리 정의된 일에 따라 진행 라인을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [MonthlyFirstLastDay](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastday/) { get; set; } | 월별 진행 라인의 첫 번째 또는 마지막 일 유형을 가져오거나 설정합니다. |
| [MonthlyFirstLastMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastmonthnumber/) { get; set; } | 첫 번째 또는 마지막 미리 정의된 일에 따라 표시되는 진행 라인의 월 번호를 가져오거나 설정합니다. |
| [WeeklyDays](../../aspose.tasks.visualization/recurringinterval/weeklydays/) { get; } | 주간 진행 라인을 위한 일 목록을 가져옵니다. |
| [WeeklyWeekNumber](../../aspose.tasks.visualization/recurringinterval/weeklyweeknumber/) { get; set; } | 주간 진행 라인의 주 번호를 가져오거나 설정합니다. |

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


