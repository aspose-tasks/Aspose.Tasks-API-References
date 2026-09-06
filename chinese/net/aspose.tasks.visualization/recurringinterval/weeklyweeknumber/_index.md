---
title: "RecurringInterval.WeeklyWeekNumber"
second_title: "Aspose.Tasks for .NET API 参考"
description: "RecurringInterval 属性。获取或设置每周进度线的周数"
type: docs
weight: 120
url: /zh/net/aspose.tasks.visualization/recurringinterval/weeklyweeknumber/
---
## RecurringInterval.WeeklyWeekNumber property

获取或设置每周进度线的周编号。

```csharp
public int WeeklyWeekNumber { get; set; }
```

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

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


