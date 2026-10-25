---
title: "RecurringTaskInfo 클래스"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.RecurringTaskInfo 클래스. 프로젝트 내 반복 작업의 세부 정보를 나타냅니다."
type: docs
weight: 1720
url: /ko/net/aspose.tasks/recurringtaskinfo/
---
## RecurringTaskInfo class

프로젝트 내 반복 작업의 세부 정보를 나타냅니다.

```csharp
public class RecurringTaskInfo
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [DailyRepetitions](../../aspose.tasks/recurringtaskinfo/dailyrepetitions/) { get; set; } | 일일 반복 패턴에 대한 반복 횟수를 가져오거나 설정합니다. |
| [DailyUseWorkdays](../../aspose.tasks/recurringtaskinfo/dailyuseworkdays/) { get; set; } | 일일 반복 패턴에 근무일을 사용할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Duration](../../aspose.tasks/recurringtaskinfo/duration/) { get; set; } | 반복 작업의 한 발생에 대한 지속 시간을 가져오거나 설정합니다. [`Duration`](./duration/) 클래스의 인스턴스입니다. |
| [EndDate](../../aspose.tasks/recurringtaskinfo/enddate/) { get; set; } | 발생이 종료되는 날짜를 가져오거나 설정합니다. |
| [MonthlyDay](../../aspose.tasks/recurringtaskinfo/monthlyday/) { get; set; } | 월별 반복 패턴의 일 수를 가져오거나 설정합니다. |
| [MonthlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyordinalday/) { get; set; } | 서수 일자를 사용할 때 월별 반복 패턴의 요일을 가져오거나 설정합니다. DayOfWeek 열거형의 값 중 하나일 수 있습니다. |
| [MonthlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/monthlyordinalnumber/) { get; set; } | 월별 반복 패턴의 서수 번호를 가져오거나 설정합니다. [`OrdinalNumber`](../ordinalnumber/) 열거형의 값 중 하나일 수 있습니다. |
| [MonthlyOrdinalRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyordinalrepetitions/) { get; set; } | 서수 일자를 사용할 때 월별 반복 패턴의 반복 횟수를 가져오거나 설정합니다. |
| [MonthlyRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyrepetitions/) { get; set; } | 월별 반복 패턴의 반복 횟수를 가져오거나 설정합니다. |
| [MonthlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyuseordinalday/) { get; set; } | 월별 반복 패턴에 서수 일자를 사용할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Occurrences](../../aspose.tasks/recurringtaskinfo/occurrences/) { get; set; } | 반복 작업의 발생 횟수를 가져오거나 설정합니다. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskinfo/recurrencepattern/) { get; set; } | 반복 작업의 반복 패턴을 가져오거나 설정합니다. [`RecurrencePattern`](./recurrencepattern/) 열거형의 값 중 하나일 수 있습니다. |
| [StartDate](../../aspose.tasks/recurringtaskinfo/startdate/) { get; set; } | 발생이 시작되는 날짜를 가져오거나 설정합니다. |
| [Task](../../aspose.tasks/recurringtaskinfo/task/) { get; } | 이 `RecurringTaskInfo` 클래스 인스턴스의 상위 작업을 가져옵니다. |
| [UseEndDate](../../aspose.tasks/recurringtaskinfo/useenddate/) { get; set; } | 반복 작업에 대해 종료 날짜를 사용할지 발생 횟수를 사용할지 나타내는 값을 가져오거나 설정합니다. |
| [WeeklyDays](../../aspose.tasks/recurringtaskinfo/weeklydays/) { get; set; } | 주간 반복 패턴에 사용되는 요일 컬렉션을 가져오거나 설정합니다. |
| [WeeklyRepetitions](../../aspose.tasks/recurringtaskinfo/weeklyrepetitions/) { get; set; } | 주간 반복 패턴의 반복 횟수를 가져오거나 설정합니다. |
| [YearlyDate](../../aspose.tasks/recurringtaskinfo/yearlydate/) { get; set; } | 연간 반복 패턴의 날짜를 가져오거나 설정합니다. |
| [YearlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyordinalday/) { get; set; } | 서수 일자를 사용할 때 연간 반복 패턴의 요일을 가져오거나 설정합니다. DayOfWeek 열거형의 값 중 하나일 수 있습니다. |
| [YearlyOrdinalMonth](../../aspose.tasks/recurringtaskinfo/yearlyordinalmonth/) { get; set; } | 서수 일자를 사용할 때 연간 반복 패턴의 월을 가져오거나 설정합니다. [`Month`](../month/) 열거형의 값 중 하나일 수 있습니다. |
| [YearlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/yearlyordinalnumber/) { get; set; } | 연간 반복 패턴의 서수 번호를 가져오거나 설정합니다. [`OrdinalNumber`](../ordinalnumber/) 열거형의 값 중 하나일 수 있습니다. |
| [YearlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyuseordinalday/) { get; set; } | 연간 반복 패턴에 서수 일자를 사용할지 여부를 나타내는 값을 가져오거나 설정합니다. |

## 예제

작업의 반복 정보를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

// 작업의 반복 정보를 읽기
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    var info = task.RecurringInfo;
    if (info == null)
    {
        continue;
    }

    Console.WriteLine("Start Date: " + info.StartDate);
    Console.WriteLine("Duration: " + info.Duration);
    Console.WriteLine("End Date: " + info.EndDate);
    Console.WriteLine("Daily Repetitions: " + info.DailyRepetitions);
    Console.WriteLine("Daily Use Workdays: " + info.DailyUseWorkdays);
    Console.WriteLine("Monthly Day: " + info.MonthlyDay);
    Console.WriteLine("Monthly Ordinal Day: " + info.MonthlyOrdinalDay);
    Console.WriteLine("Monthly Ordinal Number: " + info.MonthlyOrdinalNumber);
    Console.WriteLine("Monthly Ordinal Repetitions: " + info.MonthlyOrdinalRepetitions);
    Console.WriteLine("Monthly Repetitions: " + info.MonthlyRepetitions);
    Console.WriteLine("Monthly Use Ordinal Day: " + info.MonthlyUseOrdinalDay);
    Console.WriteLine("Occurrences: " + info.Occurrences);
    Console.WriteLine("Recurrence Pattern: " + info.RecurrencePattern);
    Console.WriteLine("Parent Task: " + info.Task.Get(Tsk.Name));
    Console.WriteLine("Use End Date: " + info.UseEndDate);
    Console.WriteLine("Weekly Days: " + info.WeeklyDays);
    Console.WriteLine("Weekly Repetitions: " + info.WeeklyRepetitions);
    Console.WriteLine("Yearly Date: " + info.YearlyDate);
    Console.WriteLine("Yearly Ordinal Day: " + info.YearlyOrdinalDay);
    Console.WriteLine("Yearly Ordinal Month: " + info.YearlyOrdinalMonth);
    Console.WriteLine("Yearly Ordinal Number: " + info.YearlyOrdinalNumber);
    Console.WriteLine("Yearly Use Ordinal Day: " + info.YearlyUseOrdinalDay);
    Console.WriteLine();
}
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


