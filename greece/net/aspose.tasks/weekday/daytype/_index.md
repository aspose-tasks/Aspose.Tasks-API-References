---
title: "WeekDay.DayType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "WeekDay property. Λαμβάνει τον τύπο μιας ημέρας"
type: docs
weight: 30
url: /el/net/aspose.tasks/weekday/daytype/
---
## WeekDay.DayType property

Λαμβάνει τον τύπο μιας ημέρας.

```csharp
public DayType DayType { get; }
```

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε ένα νέο ημερολόγιο ορίζοντας τις ημέρες της εβδομάδας.

```csharp
var project = new Project();

// Ορίστε ένα ημερολόγιο
var calendar = project.Calendars.Add("Calendar1");

// Προσθέστε εργάσιμες ημέρες από τη Δευτέρα έως την Πέμπτη με προεπιλεγμένα ωράρια
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// ελέγξτε τις ημερομηνίες από και έως της ημέρας εξαίρεσης
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Ορίστε την Παρασκευή ως σύντομη εργάσιμη ημέρα

// Ορίζει χρόνο εργασίας.
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// υπάρχει τρόπος να μετατρέψετε το <see cref=\"DayOfWeek\" /> σε <see cref=\"Aspose.Tasks.DayType\" />.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

// ας εκτυπώσουμε όλους τους χρόνους εργασίας
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### Δείτε επίσης

* enum [DayType](../../daytype/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


