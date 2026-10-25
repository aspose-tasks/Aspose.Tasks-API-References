---
title: "枚举 RecurringInterval.DayType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.RecurringIntervalDayType 枚举。表示在进度线中使用的日期类型"
type: docs
weight: 3320
url: /zh/net/aspose.tasks.visualization/recurringinterval.daytype/
---
## RecurringInterval.DayType enumeration

表示在进度线中使用的日期类型。

```csharp
public enum DayType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Sunday | `1` | 表示星期日。 |
| Monday | `2` | 表示星期一。 |
| Tuesday | `3` | 表示星期二。 |
| Wednesday | `4` | 表示星期三。 |
| Thursday | `5` | 表示星期四。 |
| Friday | `6` | 表示星期五。 |
| Saturday | `7` | 表示星期六。 |
| Day | `8` | 表示天。 |
| Workday | `9` | 表示工作日。 |
| NonworkingDay | `10` | 表示非工作日。 |

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

* class [RecurringInterval](../recurringinterval/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


