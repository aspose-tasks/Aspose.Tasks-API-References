---
title: "类 DayTypeCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.DayTypeCollection 类。表示 DayType 对象的集合"
type: docs
weight: 460
url: /zh/net/aspose.tasks/daytypecollection/
---
## DayTypeCollection class

表示一个 [`DayType`](../daytype/) 对象的集合。

```csharp
public class DayTypeCollection : IList<DayType>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/daytypecollection/count/) { get; } | 获取此集合中包含的元素数量。 |
| [IsReadOnly](../../aspose.tasks/daytypecollection/isreadonly/) { get; } | 获取一个值，指示此集合是否为只读；否则为 false。 |
| [Item](../../aspose.tasks/daytypecollection/item/) { get; set; } | 返回或设置指定索引处的元素。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/daytypecollection/add/)(DayType) | 将指定项添加到此集合中。 |
| [Clear](../../aspose.tasks/daytypecollection/clear/)() | 从此集合中移除所有项。 |
| [Contains](../../aspose.tasks/daytypecollection/contains/)(DayType) | 如果在此集合中找到指定项则返回 true；否则返回 false。 |
| [CopyTo](../../aspose.tasks/daytypecollection/copyto/)(DayType[], int) | 将此集合的元素复制到指定数组中，从指定的数组索引开始。 |
| [GetEnumerator](../../aspose.tasks/daytypecollection/getenumerator/)() | 返回此集合的枚举器。 |
| [IndexOf](../../aspose.tasks/daytypecollection/indexof/)(DayType) | 确定此集合中指定项的索引。 |
| [Insert](../../aspose.tasks/daytypecollection/insert/)(int, DayType) | 在指定索引处插入指定项。 |
| [Remove](../../aspose.tasks/daytypecollection/remove/)(DayType) | 从此集合中移除特定对象的第一次出现。 |
| [RemoveAt](../../aspose.tasks/daytypecollection/removeat/)(int) | 在指定索引处移除一项。 |

## 示例

展示如何使用工作日集合来定义每周日历例外。

```csharp
var project = new Project(DataDir + "WeeklyDayTypeException.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Exception Name: " + calendarException.Name);
    Console.WriteLine("Days of week count: " + calendarException.DaysOfWeek.Count);
    foreach (var dayType in calendarException.DaysOfWeek)
    {
        Console.WriteLine("Day type: " + dayType);
    }

    Console.WriteLine();
}

var exc1 = calendar.Exceptions.ToList()[0];
if (!exc1.DaysOfWeek.IsReadOnly && exc1.DaysOfWeek.IndexOf(DayType.Monday) < 0)
{
    exc1.DaysOfWeek.Insert(0, DayType.Wednesday);
}

var exc2 = calendar.Exceptions.ToList()[1];
if (exc2.DaysOfWeek.Contains(DayType.Sunday))
{
    // 通过日类型从 "Exception 2" 删除一个日类型
    exc2.DaysOfWeek.Remove(DayType.Sunday);
}

// 通过索引从 "Exception 2" 删除一个日类型
Console.WriteLine("Remove " + exc2.DaysOfWeek[0] + " day type from exception by index...");
exc2.DaysOfWeek.RemoveAt(0);

// 更改例外（初始项目数据中没有例外）
var exc4 = new CalendarException
               {
                   Name = "Weekly Exception 2",
                   FromDate = new DateTime(2020, 4, 13),
                   ToDate = new DateTime(2020, 4, 18),
                   Occurrences = 3,
                   Type = CalendarExceptionType.Weekly
               };
exc4.DaysOfWeek.Add(DayType.Monday);
exc4.DaysOfWeek.Add(DayType.Thursday);

calendar.Exceptions.Add(exc4);

var exc3 = calendar.Exceptions.ToList()[2];

// 删除 "Exception 3" 的所有星期天
exc3.DaysOfWeek.Clear();

var dayTypes = new DayType[exc4.DaysOfWeek.Count];
exc4.DaysOfWeek.CopyTo(dayTypes, 0);

foreach (var dayType in dayTypes)
{
    exc3.DaysOfWeek.Add(dayType);
}

Console.WriteLine("Days of week for exception: " + exc3.Name);
foreach (var dayType in exc3.DaysOfWeek)
{
    Console.WriteLine("Day type: " + dayType);
}
```

### 另见

* enum [DayType](../daytype/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


