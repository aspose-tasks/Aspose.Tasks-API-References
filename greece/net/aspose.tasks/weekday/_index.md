---
title: "Κλάση WeekDay"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.WeekDay. Αντιπροσωπεύει μια ημέρα της εβδομάδας που είτε ορίζει κανονικές ημέρες της εβδομάδας είτε ημέρες εξαίρεσης σε ένα ημερολόγιο."
type: docs
weight: 3540
url: /el/net/aspose.tasks/weekday/
---
## WeekDay class

Αντιπροσωπεύει μια ημέρα της εβδομάδας που είτε ορίζει κανονικές ημέρες της εβδομάδας είτε ημέρες εξαίρεσης σε ένα ημερολόγιο.

```csharp
public class WeekDay
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [WeekDay](weekday/#constructor)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `WeekDay`. |
| [WeekDay](weekday/#constructor_1)(DayType) | Αρχικοποιεί μια νέα παρουσία της κλάσης `WeekDay` με τον καθορισμένο τύπο ημέρας. |
| [WeekDay](weekday/#constructor_3)(DayType, IEnumerable&lt;WorkingTime&gt;) | Αρχικοποιεί μια νέα παρουσία της κλάσης `WeekDay` με τον καθορισμένο τύπο ημέρας και λίστα περιόδων εργασίας. |
| [WeekDay](weekday/#constructor_2)(DayType, params WorkingTime[]) | Αρχικοποιεί μια νέα παρουσία της κλάσης `WeekDay` με τον καθορισμένο τύπο ημέρας και περιόδους εργασίας. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [DayType](../../aspose.tasks/weekday/daytype/) { get; } | Λαμβάνει τον τύπο μιας ημέρας. |
| [DayWorking](../../aspose.tasks/weekday/dayworking/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η καθορισμένη ημερομηνία ή τύπος ημέρας είναι εργάσιμη. |
| [FromDate](../../aspose.tasks/weekday/fromdate/) { get; set; } | Λαμβάνει ή ορίζει την αρχή μιας χρονικής εξαίρεσης. |
| [ToDate](../../aspose.tasks/weekday/todate/) { get; set; } | Λαμβάνει ή ορίζει το τέλος μιας χρονικής εξαίρεσης. |
| [WorkingTimes](../../aspose.tasks/weekday/workingtimes/) { get; } | Λαμβάνει το WorkingTimeCollection για αυτήν την παρουσία WeekDay. Η συλλογή των ωρών εργασίας που ορίζουν τον χρόνο εργασίας στην ημέρα της εβδομάδας. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| static [CreateDefaultWorkingDay](../../aspose.tasks/weekday/createdefaultworkingday/)(DayType) | Δημιουργεί προεπιλεγμένη εργάσιμη ημέρα. |
| [Clone](../../aspose.tasks/weekday/clone/)() | Επιστρέφει ένα βαθύ αντίγραφο της ημέρας της εβδομάδας. |
| override [Equals](../../aspose.tasks/weekday/equals/)(object) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| override [GetHashCode](../../aspose.tasks/weekday/gethashcode/)() | Επιστρέφει μια τιμή κώδικα κατακερματισμού για την παρουσία της κλάσης `WeekDay`. |
| [GetWorkingTime](../../aspose.tasks/weekday/getworkingtime/)() | Επιστρέφει τον χρόνο εργασίας για μια ημέρα της εβδομάδας. |
| static [CastToDayType](../../aspose.tasks/weekday/casttodaytype/)(DayOfWeek) | Μετατρέπει το DayOfWeek του .Net σε [`DayType`](./daytype/). |
| static [SetDefaultWorkingTime](../../aspose.tasks/weekday/setdefaultworkingtime/)(WeekDay) | Ορίζει προεπιλεγμένες χρονικές περιόδους για την καθορισμένη ημέρα της εβδομάδας. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


