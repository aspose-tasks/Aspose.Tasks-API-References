---
title: "WorkWeekCollection.Add"
second_title: "Aspose.Tasks for .NET API 参考"
description: "WorkWeekCollection 方法。向此集合对象添加 WorkWeek 实例。"
type: docs
weight: 40
url: /zh/net/aspose.tasks/workweekcollection/add/
---
## WorkWeekCollection.Add method

向此集合对象添加 WorkWeek 实例。

```csharp
public void Add(WorkWeek item)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | WorkWeek | 要添加的项。 |

## 示例

展示如何为日历创建自定义工作周。

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Standard");
Calendar.MakeStandardCalendar(calendar);

var item = new WorkWeek();
item.Name = "My Work Week";
item.FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
item.ToDate = new DateTime(2020, 4, 17, 17, 0, 0);
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
item.WeekDays.Add(new WeekDay(DayType.Saturday));
item.WeekDays.Add(new WeekDay(DayType.Sunday));
calendar.WorkWeeks.Add(item);

Console.WriteLine("Work Weeks Count: " + calendar.WorkWeeks.Count);
foreach (var workWeek in calendar.WorkWeeks)
{
    // 显示工作周名称、父日历名称、起始和结束日期
    Console.WriteLine("Name: " + workWeek.Name);
    Console.WriteLine("Parent calendar name: " + calendar.Name);
    Console.WriteLine("From Date: " + workWeek.FromDate);
    Console.WriteLine("To Date: " + workWeek.ToDate);
    Console.WriteLine();

    // 此数据全部关于 "Details." 按钮，您可以为特定的 WeekDay 设置特殊工作时间，甚至将其设为非工作日。
    List<WeekDay> weekDays = workWeek.WeekDays.ToList();
    foreach (var day in weekDays)
    {
        Console.WriteLine(day.DayType.ToString());

        // 您可以进一步遍历工作时间并显示它们。
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }

    Console.WriteLine();
}
```

### 另见

* class [WorkWeek](../../workweek/)
* class [WorkWeekCollection](../)
* namespace [Aspose.Tasks](../../workweekcollection/)
* assembly [Aspose.Tasks](../../../)


