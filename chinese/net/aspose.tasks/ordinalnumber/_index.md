---
title: "枚举 OrdinalNumber"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.OrdinalNumber 枚举。表示 RecurringTaskInfo 类实例中的序数。"
type: docs
weight: 1140
url: /zh/net/aspose.tasks/ordinalnumber/
---
## OrdinalNumber enumeration

表示在 [`RecurringTaskInfo`](../recurringtaskinfo/) 类实例中的序数。

```csharp
public enum OrdinalNumber
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| First | `1` | 第一个元素。 |
| Second | `2` | 第二个元素。 |
| Third | `3` | 第三个元素。 |
| Fourth | `4` | 第四个元素。 |
| Last | `5` | 最后一个元素。 |

## 示例

展示如何读取任务的循环信息。

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

// 读取任务的循环信息
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

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


