---
title: "WeekDayCollection.CopyTo"
second_title: "Aspose.Tasks for .NET API 参考"
description: "WeekDayCollection 方法。将集合内容复制到指定索引处的数组。"
type: docs
weight: 60
url: /zh/net/aspose.tasks/weekdaycollection/copyto/
---
## WeekDayCollection.CopyTo method

将集合内容复制到指定索引处的数组。

```csharp
public void CopyTo(WeekDay[] array, int arrayIndex)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| array | WeekDay[] | 要复制到的 [`WeekDay`](../../weekday/) 目标数组 |
| arrayIndex | Int32 | 复制操作的起始索引。 |

## 示例

展示如何使用工作日集合。

```csharp
var project = new Project();
var calendar = project.Calendars.GetByName("Standard");

// 清除工作日
calendar.WeekDays.Clear();

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
var saturday = WeekDay.CreateDefaultWorkingDay(DayType.Saturday);
var sunday = WeekDay.CreateDefaultWorkingDay(DayType.Sunday);

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

var fridayWorkingTimes = new List<WorkingTime> { new WorkingTime(new DateTime(2020, 4, 13, 8, 0, 0), new DateTime(2020, 4, 13, 12, 0, 0)) };

var friday = new WeekDay(DayType.Friday, fridayWorkingTimes);
if (calendar.WeekDays.Contains(friday))
{
    calendar.WeekDays.Insert(4, friday);
}

Console.WriteLine("Calendar: " + calendar.Name);
Console.WriteLine("Week days count: " + calendar.WeekDays.Count);
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

// 移除星期六工作日
calendar.WeekDays.RemoveAt(5);

// 移除星期日工作日
if (calendar.WeekDays.IndexOf(saturday) > 0)
{
    calendar.WeekDays.Remove(sunday);
}

Console.WriteLine("Working times after weekend was removed: ");
List<WeekDay> weekDays = calendar.WeekDays.ToList();
foreach (var day in weekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

var hour24Calendar = project.Calendars.Add("24 Hours");
Calendar.Make24HourCalendar(hour24Calendar);

// 复制工作日
var weekDaysArray = new WeekDay[calendar.WeekDays.Count];
calendar.WeekDays.CopyTo(weekDaysArray, 0);

foreach (var weekDay in weekDaysArray)
{
    hour24Calendar.WeekDays.Add(weekDay);
}
```

### 另见

* class [WeekDay](../../weekday/)
* class [WeekDayCollection](../)
* namespace [Aspose.Tasks](../../weekdaycollection/)
* assembly [Aspose.Tasks](../../../)


