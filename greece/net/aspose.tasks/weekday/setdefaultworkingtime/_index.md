---
title: "WeekDay.SetDefaultWorkingTime"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "WeekDay μέθοδος. Ορίζει προεπιλεγμένες χρονικές περιόδους για την καθορισμένη ημέρα της εβδομάδας"
type: docs
weight: 130
url: /el/net/aspose.tasks/weekday/setdefaultworkingtime/
---
## WeekDay.SetDefaultWorkingTime method

Ορίζει προεπιλεγμένες χρονικές περιόδους για την καθορισμένη ημέρα της εβδομάδας.

```csharp
public static void SetDefaultWorkingTime(WeekDay day)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ημέρα | WeekDay | Η ημέρα της εβδομάδας για την οποία θα οριστεί η προεπιλεγμένη εργάσιμη ημέρα. |

## Παραδείγματα

Δείχνει πώς να ορίσετε προεπιλεγμένο εργάσιμο χρόνο για μια ημέρα.

```csharp
var project = new Project();

// Ορίστε ένα ημερολόγιο
var calendar = project.Calendars.Add("Calendar1");
calendar.WeekDays.Clear();

// Προσθέστε εργάσιμες ημέρες από τη Δευτέρα έως την Πέμπτη με προεπιλεγμένα ωράρια
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

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


