---
title: "열거형 OrdinalNumber"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.OrdinalNumber 열거형. RecurringTaskInfo 클래스 인스턴스에서 서수 번호를 나타냅니다."
type: docs
weight: 1140
url: /ko/net/aspose.tasks/ordinalnumber/
---
## OrdinalNumber enumeration

[`RecurringTaskInfo`](../recurringtaskinfo/) 클래스 인스턴스에서 서수 번호를 나타냅니다.

```csharp
public enum OrdinalNumber
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| First | `1` | 첫 번째 요소입니다. |
| Second | `2` | 두 번째 요소입니다. |
| Third | `3` | 세 번째 요소. |
| Fourth | `4` | 네 번째 요소. |
| Last | `5` | 마지막 요소. |

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


