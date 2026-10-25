---
title: "WorkingTimeCollection 类"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.WorkingTimeCollection 类。表示 WorkingTimeCollection 对象的集合"
type: docs
weight: 3670
url: /zh/net/aspose.tasks/workingtimecollection/
---
## WorkingTimeCollection class

表示 `WorkingTimeCollection` 对象的集合。

```csharp
public class WorkingTimeCollection : IList<WorkingTime>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/workingtimecollection/count/) { get; } | 获取此 `WorkingTimeCollection` 对象中包含的对象数量。 |
| [Item](../../aspose.tasks/workingtimecollection/item/) { get; set; } | 返回指定索引处的元素。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/workingtimecollection/add/)(WorkingTime) | 向此集合添加一个新的 WorkingTime 实例。 |
| [Clear](../../aspose.tasks/workingtimecollection/clear/)() | 从集合中移除所有 [`WorkingTime`](../workingtime/) 项目。 |
| [Contains](../../aspose.tasks/workingtimecollection/contains/)(WorkingTime) | 检查指定元素是否在列表中。执行线性 O(n) 搜索。 |
| [CopyTo](../../aspose.tasks/workingtimecollection/copyto/)(WorkingTime[], int) | 将集合内容复制到 Array 中，从特定索引开始 |
| [GetEnumerator](../../aspose.tasks/workingtimecollection/getenumerator/)() | 返回此集合的枚举器。 |
| [Remove](../../aspose.tasks/workingtimecollection/remove/)(WorkingTime) | 从此集合中移除 [`WorkingTime`](../workingtime/) 实例。 |
| [ToList](../../aspose.tasks/workingtimecollection/tolist/)() | 将 WorkingTimeCollection 对象转换为 [`WorkingTime`](../workingtime/) 对象的列表。 |

## 示例

展示如何使用工作时间集合。

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Custom Calendar");

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));

var saturdayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(8, 12),
    new WorkingTime(13, 15)
};
var saturday = new WeekDay(DayType.Saturday);
foreach (var time in saturdayWorkingTimes)
{
    saturday.WorkingTimes.Add(time);
}

// 打印星期六的工作时间
Console.WriteLine("Saturday working period number: " + saturday.WorkingTimes.Count);
foreach (var time in saturday.WorkingTimes)
{
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

var sundayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(10, 15)
};
var sunday = new WeekDay(DayType.Sunday, sundayWorkingTimes);

// 打印星期日的工作时间
List<WorkingTime> workingTimes = sunday.WorkingTimes.ToList();
Console.WriteLine("Sunday working period number: " + workingTimes.Count);
for (var index = 0; index < workingTimes.Count; index++)
{
    var time = workingTimes[index];
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType + ": ");

    // 您可以进一步遍历工作时间并显示它们。
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine(workingTime.From);
        Console.WriteLine(workingTime.To);
    }

    Console.WriteLine();
}
```

### 另见

* class [WorkingTime](../workingtime/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


