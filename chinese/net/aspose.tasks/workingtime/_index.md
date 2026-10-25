---
title: "类 WorkingTime"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.WorkingTime 类。表示工作日内的工作时间。"
type: docs
weight: 3660
url: /zh/net/aspose.tasks/workingtime/
---
## WorkingTime class

表示工作日内的工作时间。

```csharp
public class WorkingTime
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [WorkingTime](workingtime/#constructor_1)(DateTime, DateTime) | 使用指定的开始和结束时间初始化 `WorkingTime` 类的新实例（一个区间）。 |
| [WorkingTime](workingtime/#constructor)(int, int) | 使用指定的开始和结束时间初始化 `WorkingTime` 类的新实例（一个区间项）。 |
| [WorkingTime](workingtime/#constructor_2)(TimeSpan, TimeSpan) | 使用指定的开始和结束时间初始化 `WorkingTime` 类的新实例（一个区间项）。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [From](../../aspose.tasks/workingtime/from/) { get; } | 获取工作时间的开始。 |
| [To](../../aspose.tasks/workingtime/to/) { get; } | 获取工作时间的结束。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [Equals](../../aspose.tasks/workingtime/equals/)(object) | 检查对象是否相等。 |
| override [GetHashCode](../../aspose.tasks/workingtime/gethashcode/)() | 返回 `WorkingTime` 类实例的哈希码值。 |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


