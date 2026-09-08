---
title: "WeekDay.WorkingTimes"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "WeekDay-eigenschap. Haalt WorkingTimeCollection op voor deze WeekDay-instantie. De verzameling werktijden die de gewerkte tijd op de weekdag definiëren."
type: docs
weight: 70
url: /nl/net/aspose.tasks/weekday/workingtimes/
---
## WeekDay.WorkingTimes property

Haalt de WorkingTimeCollection op voor dit WeekDay‑exemplaar. De collectie werkuren die de gewerkte tijd op de weekdag definiëren.

```csharp
public WorkingTimeCollection WorkingTimes { get; }
```

## Voorbeelden

Toont hoe een nieuwe kalender te maken door weekdagen te definiëren.

```csharp
var project = new Project();

// Definieer een kalender
var calendar = project.Calendars.Add("Calendar1");

// Voeg werkdagen toe van maandag tot en met donderdag met standaardtijden
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// controleer van‑ en tot‑datums van de uitzonderingsdag
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Stel vrijdag in als korte werkdag

// Stelt werktijd in. 
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// er is een manier om <see cref=\"DayOfWeek\" /> te converteren naar <see cref=\"Aspose.Tasks.DayType\" />.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

// laten we alle werktijden afdrukken
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### Zie ook

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


