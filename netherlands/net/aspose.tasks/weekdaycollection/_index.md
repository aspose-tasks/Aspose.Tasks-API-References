---
title: "Klasse WeekDayCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.WeekDayCollection klasse. Vertegenwoordigt een verzameling van WeekDay-objecten"
type: docs
weight: 3550
url: /nl/net/aspose.tasks/weekdaycollection/
---
## WeekDayCollection class

Vertegenwoordigt een verzameling van [`WeekDay`](../weekday/) objecten.

```csharp
public class WeekDayCollection : IList<WeekDay>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/weekdaycollection/count/) { get; } | Haalt het aantal objecten op dat in dit `WeekDayCollection` object is opgenomen. |
| [Item](../../aspose.tasks/weekdaycollection/item/) { get; set; } | Haalt of stelt de itemwaarde in op de opgegeven index. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/weekdaycollection/add/)(WeekDay) | Voegt een [`WeekDay`](../weekday/) instantie toe aan dit object. |
| [Clear](../../aspose.tasks/weekdaycollection/clear/)() | Maak het WeekDayCollection-object leeg. |
| [Contains](../../aspose.tasks/weekdaycollection/contains/)(WeekDay) | Controleert of de collectie [`WeekDay`](../weekday/) bevat. |
| [CopyTo](../../aspose.tasks/weekdaycollection/copyto/)(WeekDay[], int) | Kopieert de inhoud van de collectie naar een array op de opgegeven index. |
| [GetEnumerator](../../aspose.tasks/weekdaycollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [IndexOf](../../aspose.tasks/weekdaycollection/indexof/)(WeekDay) | Retourneert de index van de opgegeven [`WeekDay`](../weekday/). |
| [Insert](../../aspose.tasks/weekdaycollection/insert/)(int, WeekDay) | Voegt [`WeekDay`](../weekday/) in op de opgegeven index. |
| [Remove](../../aspose.tasks/weekdaycollection/remove/)(WeekDay) | Verwijdert de opgegeven [`WeekDay`](../weekday/), indien aanwezig. |
| [RemoveAt](../../aspose.tasks/weekdaycollection/removeat/)(int) | Verwijdert een item op de opgegeven index. |
| [ToList](../../aspose.tasks/weekdaycollection/tolist/)() | Converteert het WeekDayCollection-object naar een lijst van [`WeekDay`](../weekday/) objecten. |

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

* class [WeekDay](../weekday/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


