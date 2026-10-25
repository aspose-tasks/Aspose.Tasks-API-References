---
title: "WorkingTime.WorkingTime"
second_title: "Aspose.Tasks for .NET API 参考"
description: "WorkingTime 构造函数。使用指定的开始和结束时间的间隔来初始化 WorkingTime 类的一个新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

使用指定的开始和结束时间的间隔来初始化 [`WorkingTime`](../) 类的一个新实例。

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fromTime | DateTime | 间隔开始时间 |
| toTime | DateTime | 间隔结束时间 |

## 示例

展示如何使用工作时间信息。

```csharp
public void WorkWithWorkingTime()
{
    var project = new Project();
    var calendar = CreateCalendar(project);
    project.Set(Prj.Calendar, calendar);

    Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);

    // 此数据全部关于 "Details." 按钮，您可以为特定的 WeekDay 设置特殊工作时间，甚至将其设为非工作日。
    List<WeekDay> weekDays = calendar.WeekDays.ToList();
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
}

public static Calendar CreateCalendar(Project project)
{
    var calendar = project.Calendars.Add("MyCalendar", project.Calendars.GetByName("Standard"));
    var workingTimes = new List<WorkingTime>
                           {
                               new WorkingTime(new DateTime(1, 1, 1, 9, 0, 0), new DateTime(1, 1, 1, 12, 0, 0)),
                               new WorkingTime(new DateTime(1, 1, 1, 13, 0, 0), new DateTime(1, 1, 1, 18, 0, 0))
                           };

    calendar.WeekDays.Add(new WeekDay(DayType.Monday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Wednesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Thursday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Friday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
    calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

    return calendar;
}
```

### 另见

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

使用指定的开始和结束时间的间隔项来初始化 [`WorkingTime`](../) 类的一个新实例。

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fromTime | TimeSpan | 间隔的开始时间由 TimeSpan 结构表示。 |
| toTime | TimeSpan | 间隔的结束时间由 TimeSpan 结构表示。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentException | 当 toTime 小于或等于 toTime 参数，或当 fromTime 与 toTime 之间的间隔大于 24 小时时。 |

## 示例

可以使用 WorkingTime ctor 的重载来使用 TimeSpans 初始化区间的开始和结束：

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### 另见

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

使用指定的开始和结束时间的间隔项来初始化 [`WorkingTime`](../) 类的一个新实例。

```csharp
public WorkingTime(int fromHours, int toHours)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fromHours | Int32 | Interval 的开始时间以整数小时表示 (0-24)。 |
| toHours | Int32 | Interval 的结束时间以整数小时表示 (0-24)。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentException | 当 toTime 小于或等于 toTime 参数，或当 fromTime 与 toTime 之间的间隔大于 24 小时时。 |

## 示例

可以使用 WorkingTime ctor 的重载来使用整数小时初始化区间的开始和结束：

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

展示如何检查工作时间相等性。

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// 日历的相等性是根据工作时间的起始和结束日期进行检查的。
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### 另见

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


