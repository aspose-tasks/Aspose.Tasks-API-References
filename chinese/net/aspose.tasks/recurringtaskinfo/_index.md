---
title: "类 RecurringTaskInfo"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.RecurringTaskInfo 类。表示项目中循环任务的详细信息。"
type: docs
weight: 1720
url: /zh/net/aspose.tasks/recurringtaskinfo/
---
## RecurringTaskInfo class

表示项目中循环任务的详细信息。

```csharp
public class RecurringTaskInfo
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [DailyRepetitions](../../aspose.tasks/recurringtaskinfo/dailyrepetitions/) { get; set; } | 获取或设置每日循环模式的重复次数。 |
| [DailyUseWorkdays](../../aspose.tasks/recurringtaskinfo/dailyuseworkdays/) { get; set; } | 获取或设置指示是否在每日循环模式中使用工作日的值。 |
| [Duration](../../aspose.tasks/recurringtaskinfo/duration/) { get; set; } | 获取或设置循环任务一次出现的持续时间。[`Duration`](./duration/) 类的实例。 |
| [EndDate](../../aspose.tasks/recurringtaskinfo/enddate/) { get; set; } | 获取或设置事件结束的日期。 |
| [MonthlyDay](../../aspose.tasks/recurringtaskinfo/monthlyday/) { get; set; } | 获取或设置每月循环模式的天数。 |
| [MonthlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyordinalday/) { get; set; } | 获取或设置使用序数日时每月循环模式的某一天。可以是 DayOfWeek 枚举的值之一。 |
| [MonthlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/monthlyordinalnumber/) { get; set; } | 获取或设置每月循环模式的序数。可以是 [`OrdinalNumber`](../ordinalnumber/) 枚举的值之一。 |
| [MonthlyOrdinalRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyordinalrepetitions/) { get; set; } | 获取或设置使用序数日时每月循环模式的重复次数。 |
| [MonthlyRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyrepetitions/) { get; set; } | 获取或设置每月循环模式的重复次数。 |
| [MonthlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyuseordinalday/) { get; set; } | 获取或设置指示是否在每月循环模式中使用序数日的值。 |
| [Occurrences](../../aspose.tasks/recurringtaskinfo/occurrences/) { get; set; } | 获取或设置循环任务的出现次数。 |
| [RecurrencePattern](../../aspose.tasks/recurringtaskinfo/recurrencepattern/) { get; set; } | 获取或设置循环任务的重复模式。可以是 [`RecurrencePattern`](./recurrencepattern/) 枚举的值之一。 |
| [StartDate](../../aspose.tasks/recurringtaskinfo/startdate/) { get; set; } | 获取或设置事件开始的日期。 |
| [Task](../../aspose.tasks/recurringtaskinfo/task/) { get; } | 获取此 `RecurringTaskInfo` 类实例的父任务。 |
| [UseEndDate](../../aspose.tasks/recurringtaskinfo/useenddate/) { get; set; } | 获取或设置一个值，指示是否对循环任务使用结束日期或出现次数。 |
| [WeeklyDays](../../aspose.tasks/recurringtaskinfo/weeklydays/) { get; set; } | 获取或设置在每周循环模式中使用的天集合。 |
| [WeeklyRepetitions](../../aspose.tasks/recurringtaskinfo/weeklyrepetitions/) { get; set; } | 获取或设置每周循环模式的重复次数。 |
| [YearlyDate](../../aspose.tasks/recurringtaskinfo/yearlydate/) { get; set; } | 获取或设置年度循环模式的日期。 |
| [YearlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyordinalday/) { get; set; } | 获取或设置使用序数日时的年度循环模式的工作日。可以是 DayOfWeek 枚举的其中一个值。 |
| [YearlyOrdinalMonth](../../aspose.tasks/recurringtaskinfo/yearlyordinalmonth/) { get; set; } | 获取或设置使用序数日时的年度循环模式的月份。可以是 [`Month`](../month/) 枚举的其中一个值。 |
| [YearlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/yearlyordinalnumber/) { get; set; } | 获取或设置年度循环模式的序数。可以是 [`OrdinalNumber`](../ordinalnumber/) 枚举的其中一个值。 |
| [YearlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyuseordinalday/) { get; set; } | 获取或设置一个值，指示是否对年度循环模式使用序数日。 |

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


