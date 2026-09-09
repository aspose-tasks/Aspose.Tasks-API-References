---
title: "Enum OrdinalNumber"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.OrdinalNumber enum. RecurringTaskInfo sınıfının örneğinde bir sıra numarasını temsil eder"
type: docs
weight: 1140
url: /tr/net/aspose.tasks/ordinalnumber/
---
## OrdinalNumber enumeration

[`RecurringTaskInfo`](../recurringtaskinfo/) sınıfının örneğinde bir sıra numarasını temsil eder.

```csharp
public enum OrdinalNumber
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| First | `1` | İlk öğe. |
| Second | `2` | İkinci öğe. |
| Third | `3` | Üçüncü öğe. |
| Fourth | `4` | Dördüncü öğe. |
| Last | `5` | Son öğe. |

## Örnekler

Görevlerin yinelenen bilgilerini nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

// görevlerin yinelenen bilgilerini oku
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

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


