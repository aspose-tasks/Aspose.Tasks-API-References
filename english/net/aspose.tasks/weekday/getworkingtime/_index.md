---
title: WeekDay.GetWorkingTime
second_title: Aspose.Tasks for .NET API Reference
description: WeekDay method. Returns the working time for a week day
type: docs
weight: 110
url: /net/aspose.tasks/weekday/getworkingtime/
---
## WeekDay.GetWorkingTime method

Returns the working time for a week day.

```csharp
public TimeSpan GetWorkingTime()
```

### Return Value

Working time.

## Examples

Shows how to create a new calendar by defining of week days.

```csharp
var project = new Project();

// Define a calendar
var calendar = project.Calendars.Add("Calendar1");

// Add working days monday through thursday with default timings
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// check from and to dates of the exception day
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Set friday as short working day

// Sets working time. 
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// there is a way to convert <see cref="DayOfWeek" /> to <see cref="Aspose.Tasks.DayType" />.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

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


