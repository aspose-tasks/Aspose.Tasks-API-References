---
title: WeekDay.SetDefaultWorkingTime
second_title: Aspose.Tasks for .NET API Reference
description: WeekDay method. Sets default time periods for the specified week day
type: docs
weight: 130
url: /net/aspose.tasks/weekday/setdefaultworkingtime/
---
## WeekDay.SetDefaultWorkingTime method

Sets default time periods for the specified week day.

```csharp
public static void SetDefaultWorkingTime(WeekDay day)
```

| Parameter | Type | Description |
| --- | --- | --- |
| day | WeekDay | The week day to set default working day on. |

## Examples

Shows how to set a default working time for a day.

```csharp
var project = new Project();

// Define a calendar
var calendar = project.Calendars.Add("Calendar1");
calendar.WeekDays.Clear();

// Add working days monday through thursday with default timings
var monday = new WeekDay(DayType.Monday);
WeekDay.SetDefaultWorkingTime(monday);
calendar.WeekDays.Add(monday);
var tuesday = new WeekDay(DayType.Tuesday);
WeekDay.SetDefaultWorkingTime(tuesday);
calendar.WeekDays.Add(tuesday);
var wednesday = new WeekDay(DayType.Wednesday);
WeekDay.SetDefaultWorkingTime(wednesday);
calendar.WeekDays.Add(wednesday);
var thursday = new WeekDay(DayType.Thursday);
WeekDay.SetDefaultWorkingTime(thursday);
calendar.WeekDays.Add(thursday);
var friday = new WeekDay(DayType.Friday);
WeekDay.SetDefaultWorkingTime(friday);
calendar.WeekDays.Add(friday);

var saturday = new WeekDay(DayType.Saturday);
saturday.DayWorking = false;
calendar.WeekDays.Add(saturday);
var sunday = new WeekDay(DayType.Sunday);
sunday.DayWorking = false;
calendar.WeekDays.Add(sunday);

// lets print all working times
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### See Also

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


