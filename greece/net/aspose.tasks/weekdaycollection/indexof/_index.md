---
title: "WeekDayCollection.IndexOf"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος WeekDayCollection. Επιστρέφει το ευρετήριο του καθορισμένου WeekDay"
type: docs
weight: 80
url: /el/net/aspose.tasks/weekdaycollection/indexof/
---
## WeekDayCollection.IndexOf method

Επιστρέφει το ευρετήριο του καθορισμένου [`WeekDay`](../../weekday/).

```csharp
public int IndexOf(WeekDay item)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | WeekDay | Το στοιχείο για σύγκριση. |

### Τιμή Επιστροφής

Μηδενική βάση ευρετηρίου του καθορισμένου [`WeekDay`](../../weekday/), εάν υπάρχει, ή -1 διαφορετικά.

## Παραδείγματα

Δείχνει πώς να εργάζεστε με συλλογές ημερών της εβδομάδας.

```csharp
var project = new Project();
var calendar = project.Calendars.GetByName("Standard");

// καθαρίστε τις ημέρες της εβδομάδας
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

// αφαιρέστε την ημέρα Σάββατο
calendar.WeekDays.RemoveAt(5);

// αφαιρέστε την ημέρα Κυριακή
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

// αντιγράψτε τις ημέρες της εβδομάδας
var weekDaysArray = new WeekDay[calendar.WeekDays.Count];
calendar.WeekDays.CopyTo(weekDaysArray, 0);

foreach (var weekDay in weekDaysArray)
{
    hour24Calendar.WeekDays.Add(weekDay);
}
```

### Δείτε επίσης

* class [WeekDay](../../weekday/)
* class [WeekDayCollection](../)
* namespace [Aspose.Tasks](../../weekdaycollection/)
* assembly [Aspose.Tasks](../../../)


