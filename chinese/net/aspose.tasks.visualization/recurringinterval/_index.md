---
title: "类 RecurringInterval"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.RecurringInterval 类。表示在甘特图视图的进度线中使用的循环间隔"
type: docs
weight: 3310
url: /zh/net/aspose.tasks.visualization/recurringinterval/
---
## RecurringInterval class

表示在甘特图视图的进度线中使用的循环间隔。

```csharp
public class RecurringInterval
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [RecurringInterval](recurringinterval/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [DailyDayNumber](../../aspose.tasks.visualization/recurringinterval/dailydaynumber/) { get; set; } | 获取或设置每日的天数。 |
| [DailyWorkday](../../aspose.tasks.visualization/recurringinterval/dailyworkday/) { get; set; } | 获取或设置一个值，指示该天是否为每日进度线的工作日。 |
| [Interval](../../aspose.tasks.visualization/recurringinterval/interval/) { get; set; } | 获取或设置循环间隔。可以是 [`Interval`](./interval/) 类型的任何值。 |
| [MonthlyDay](../../aspose.tasks.visualization/recurringinterval/monthlyday/) { get; set; } | 获取或设置一个值，指示是否按天显示每月进度线。 |
| [MonthlyDayDayNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaydaynumber/) { get; set; } | 获取或设置每月进度线的天数。 |
| [MonthlyDayMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaymonthnumber/) { get; set; } | 获取或设置每月进度线的月份编号。 |
| [MonthlyFirstLast](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlast/) { get; set; } | 获取或设置一个值，指示是否按首个或最后一个预定义日期显示进度线。 |
| [MonthlyFirstLastDay](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastday/) { get; set; } | 获取或设置每月进度线的首日或末日类型。 |
| [MonthlyFirstLastMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastmonthnumber/) { get; set; } | 获取或设置进度线的月份编号，这些进度线按首个或最后一个预定义日期显示。 |
| [WeeklyDays](../../aspose.tasks.visualization/recurringinterval/weeklydays/) { get; } | 获取每周进度线的日期列表。 |
| [WeeklyWeekNumber](../../aspose.tasks.visualization/recurringinterval/weeklyweeknumber/) { get; set; } | 获取或设置每周进度线的周编号。 |

## 示例

展示如何使用进度线的循环间隔。

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

// 读取进度线。
var interval = view.ProgressLines.RecurringInterval;

Console.WriteLine("Interval: " + interval.Interval);
Console.WriteLine("Weekly Week Number: " + interval.WeeklyWeekNumber);
foreach (var day in interval.WeeklyDays)
{
    Console.WriteLine("Week day: " + day);
}

// 重新定义循环间隔。
var newInterval = new RecurringInterval();

// 设置一个值，指示是否按天显示每月进度线。
interval.MonthlyDay = true;
// 设置每月进度线的天数。
interval.MonthlyDayDayNumber = 1;
// 设置每月进度线的月份编号。
interval.MonthlyDayMonthNumber = 1;
// 设置一个值，指示是否按首个或最后一个预定义日显示进度线。
interval.MonthlyFirstLast = true;
// 设置每月进度线的首日或末日类型。
interval.MonthlyFirstLastDay = RecurringInterval.DayType.Day;
// 设置进度线的月份编号，这些进度线按首个或最后一个预定义日显示。
interval.MonthlyFirstLastMonthNumber = 1;

view.ProgressLines.RecurringInterval = newInterval;

project.Save(OutDir + "WorkWithRecurringInterval_out.pdf", SaveFileFormat.Pdf);
```

### 另见

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


