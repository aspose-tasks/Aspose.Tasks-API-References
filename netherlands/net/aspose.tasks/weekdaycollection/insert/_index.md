---
title: "WeekDayCollection.Insert"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "WeekDayCollection-methode. Voegt WeekDay in op de opgegeven index"
type: docs
weight: 90
url: /nl/net/aspose.tasks/weekdaycollection/insert/
---
## WeekDayCollection.Insert method

Voegt [`WeekDay`](../../weekday/) in op de opgegeven index.

```csharp
public void Insert(int index, WeekDay item)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | Int32 | Index om in te voegen. |
| item | WeekDay | Het item om in te voegen. |

## Voorbeelden

Toont hoe weekdagcollecties te gebruiken.

```csharp
var project = new Project();
var calendar = project.Calendars.GetByName("Standard");

// wis weekdagen
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

// verwijder zaterdag weekdag
calendar.WeekDays.RemoveAt(5);

// verwijder zondag weekdag
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

// kopieer weekdagen
var weekDaysArray = new WeekDay[calendar.WeekDays.Count];
calendar.WeekDays.CopyTo(weekDaysArray, 0);

foreach (var weekDay in weekDaysArray)
{
    hour24Calendar.WeekDays.Add(weekDay);
}
```

### Zie ook

* class [WeekDay](../../weekday/)
* class [WeekDayCollection](../)
* namespace [Aspose.Tasks](../../weekdaycollection/)
* assembly [Aspose.Tasks](../../../)


