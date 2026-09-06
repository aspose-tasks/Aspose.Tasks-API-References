---
title: "类 WorkWeekCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.WorkWeekCollection 类。表示一个 WorkWeek 对象的集合"
type: docs
weight: 3650
url: /zh/net/aspose.tasks/workweekcollection/
---
## WorkWeekCollection class

表示一个 [`WorkWeek`](../workweek/) 对象的集合。

```csharp
public class WorkWeekCollection : IList<WorkWeek>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/workweekcollection/count/) { get; } | 获取此 `WorkWeekCollection` 对象中包含的对象数量。 |
| [Item](../../aspose.tasks/workweekcollection/item/) { get; set; } | 返回指定索引处的元素。 |
| [ParentCalendar](../../aspose.tasks/workweekcollection/parentcalendar/) { get; } | 获取父日历。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/workweekcollection/add/)(WorkWeek) | 向此集合对象添加 WorkWeek 实例。 |
| [GetEnumerator](../../aspose.tasks/workweekcollection/getenumerator/)() | 返回此集合的枚举器。 |
| [ToList](../../aspose.tasks/workweekcollection/tolist/)() | 将 WorkWeekCollection 对象转换为 [`WorkWeek`](../workweek/) 对象列表。 |

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

* class [WorkWeek](../workweek/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


