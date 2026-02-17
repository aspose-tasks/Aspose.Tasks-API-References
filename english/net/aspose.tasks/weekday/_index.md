---
title: Class WeekDay
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.WeekDay class. Represents a weekday which either defines regular days of a week or exception days in a calendar
type: docs
weight: 3520
url: /net/aspose.tasks/weekday/
---
## WeekDay class

Represents a weekday which either defines regular days of a week or exception days in a calendar.

```csharp
public class WeekDay
```

## Constructors

| Name | Description |
| --- | --- |
| [WeekDay](weekday/#constructor)() | Initializes a new instance of the `WeekDay` class. |
| [WeekDay](weekday/#constructor_1)(DayType) | Initializes a new instance of the `WeekDay` class with the specified day type. |
| [WeekDay](weekday/#constructor_3)(DayType, IEnumerable&lt;WorkingTime&gt;) | Initializes a new instance of the `WeekDay` class with the specified day type and list of working time periods. |
| [WeekDay](weekday/#constructor_2)(DayType, params WorkingTime[]) | Initializes a new instance of the `WeekDay` class with the specified day type and working time periods. |

## Properties

| Name | Description |
| --- | --- |
| [DayType](../../aspose.tasks/weekday/daytype/) { get; } | Gets the type of a day. |
| [DayWorking](../../aspose.tasks/weekday/dayworking/) { get; set; } | Gets or sets a value indicating whether the specified date or day type is working. |
| [FromDate](../../aspose.tasks/weekday/fromdate/) { get; set; } | Gets or sets the beginning of an exception time. |
| [ToDate](../../aspose.tasks/weekday/todate/) { get; set; } | Gets or sets the end of an exception time. |
| [WorkingTimes](../../aspose.tasks/weekday/workingtimes/) { get; } | Gets WorkingTimeCollection for this WeekDay instance. The collection of working times that define the time worked on the weekday. |

## Methods

| Name | Description |
| --- | --- |
| static [CreateDefaultWorkingDay](../../aspose.tasks/weekday/createdefaultworkingday/)(DayType) | Creates default working day. |
| [Clone](../../aspose.tasks/weekday/clone/)() | Returns a deep copy of the week day. |
| override [Equals](../../aspose.tasks/weekday/equals/)(object) | Returns a value indicating whether this instance is equal to a specified object. |
| override [GetHashCode](../../aspose.tasks/weekday/gethashcode/)() | Returns a hash code value for the instance of the `WeekDay` class. |
| [GetWorkingTime](../../aspose.tasks/weekday/getworkingtime/)() | Returns the working time for a week day. |
| static [CastToDayType](../../aspose.tasks/weekday/casttodaytype/)(DayOfWeek) | Casts .Net's DayOfWeek to [`DayType`](./daytype/). |
| static [SetDefaultWorkingTime](../../aspose.tasks/weekday/setdefaultworkingtime/)(WeekDay) | Sets default time periods for the specified week day. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


