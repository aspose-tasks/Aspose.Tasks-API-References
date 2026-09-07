---
title: "Κλάση WeekDayCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.WeekDayCollection κλάση. Αντιπροσωπεύει μια συλλογή αντικειμένων WeekDay."
type: docs
weight: 3550
url: /el/net/aspose.tasks/weekdaycollection/
---
## WeekDayCollection class

Αντιπροσωπεύει μια συλλογή των [`WeekDay`](../weekday/) αντικειμένων.

```csharp
public class WeekDayCollection : IList<WeekDay>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/weekdaycollection/count/) { get; } | Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο `WeekDayCollection`. |
| [Item](../../aspose.tasks/weekdaycollection/item/) { get; set; } | Λαμβάνει ή ορίζει την τιμή του στοιχείου στο καθορισμένο δείκτη. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/weekdaycollection/add/)(WeekDay) | Προσθέτει μια παρουσία [`WeekDay`](../weekday/) σε αυτό το αντικείμενο. |
| [Clear](../../aspose.tasks/weekdaycollection/clear/)() | Καθαρίζει το αντικείμενο WeekDayCollection. |
| [Contains](../../aspose.tasks/weekdaycollection/contains/)(WeekDay) | Ελέγχει αν η συλλογή περιέχει το καθορισμένο [`WeekDay`](../weekday/). |
| [CopyTo](../../aspose.tasks/weekdaycollection/copyto/)(WeekDay[], int) | Αντιγράφει το περιεχόμενο της συλλογής σε έναν πίνακα στο καθορισμένο δείκτη. |
| [GetEnumerator](../../aspose.tasks/weekdaycollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [IndexOf](../../aspose.tasks/weekdaycollection/indexof/)(WeekDay) | Επιστρέφει το δείκτη του καθορισμένου [`WeekDay`](../weekday/). |
| [Insert](../../aspose.tasks/weekdaycollection/insert/)(int, WeekDay) | Εισάγει το [`WeekDay`](../weekday/) στο καθορισμένο δείκτη. |
| [Remove](../../aspose.tasks/weekdaycollection/remove/)(WeekDay) | Αφαιρεί το καθορισμένο [`WeekDay`](../weekday/), εάν υπάρχει. |
| [RemoveAt](../../aspose.tasks/weekdaycollection/removeat/)(int) | Αφαιρεί ένα στοιχείο στο καθορισμένο δείκτη. |
| [ToList](../../aspose.tasks/weekdaycollection/tolist/)() | Μετατρέπει το αντικείμενο WeekDayCollection σε λίστα αντικειμένων [`WeekDay`](../weekday/). |

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

* class [WeekDay](../weekday/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


