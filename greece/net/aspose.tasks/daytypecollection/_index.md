---
title: "Κλάση DayTypeCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η κλάση Aspose.Tasks.DayTypeCollection. Αντιπροσωπεύει μια συλλογή αντικειμένων DayType"
type: docs
weight: 460
url: /el/net/aspose.tasks/daytypecollection/
---
## DayTypeCollection class

Αντιπροσωπεύει μια συλλογή αντικειμένων [`DayType`](../daytype/).

```csharp
public class DayTypeCollection : IList<DayType>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/daytypecollection/count/) { get; } | Λαμβάνει τον αριθμό των στοιχείων που περιέχονται σε αυτή τη συλλογή. |
| [IsReadOnly](../../aspose.tasks/daytypecollection/isreadonly/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση· διαφορετικά, ψευδής. |
| [Item](../../aspose.tasks/daytypecollection/item/) { get; set; } | Επιστρέφει ή ορίζει το στοιχείο στη συγκεκριμένη θέση. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/daytypecollection/add/)(DayType) | Προσθέτει το καθορισμένο στοιχείο σε αυτή τη συλλογή. |
| [Clear](../../aspose.tasks/daytypecollection/clear/)() | Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή. |
| [Contains](../../aspose.tasks/daytypecollection/contains/)(DayType) | Επιστρέφει true εάν το καθορισμένο στοιχείο βρεθεί σε αυτή τη συλλογή· διαφορετικά, false. |
| [CopyTo](../../aspose.tasks/daytypecollection/copyto/)(DayType[], int) | Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα, ξεκινώντας από τη συγκεκριμένη θέση του πίνακα. |
| [GetEnumerator](../../aspose.tasks/daytypecollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [IndexOf](../../aspose.tasks/daytypecollection/indexof/)(DayType) | Καθορίζει το δείκτη του καθορισμένου στοιχείου σε αυτή τη συλλογή. |
| [Insert](../../aspose.tasks/daytypecollection/insert/)(int, DayType) | Εισάγει το καθορισμένο στοιχείο στον καθορισμένο δείκτη. |
| [Remove](../../aspose.tasks/daytypecollection/remove/)(DayType) | Αφαιρεί την πρώτη εμφάνιση ενός συγκεκριμένου αντικειμένου από αυτή τη συλλογή. |
| [RemoveAt](../../aspose.tasks/daytypecollection/removeat/)(int) | Αφαιρεί ένα στοιχείο στον καθορισμένο δείκτη. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε μια συλλογή ημερών της εβδομάδας για να ορίσετε εξαίρεση εβδομαδιαίου ημερολογίου.

```csharp
var project = new Project(DataDir + "WeeklyDayTypeException.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Exception Name: " + calendarException.Name);
    Console.WriteLine("Days of week count: " + calendarException.DaysOfWeek.Count);
    foreach (var dayType in calendarException.DaysOfWeek)
    {
        Console.WriteLine("Day type: " + dayType);
    }

    Console.WriteLine();
}

var exc1 = calendar.Exceptions.ToList()[0];
if (!exc1.DaysOfWeek.IsReadOnly && exc1.DaysOfWeek.IndexOf(DayType.Monday) < 0)
{
    exc1.DaysOfWeek.Insert(0, DayType.Wednesday);
}

var exc2 = calendar.Exceptions.ToList()[1];
if (exc2.DaysOfWeek.Contains(DayType.Sunday))
{
    // Διαγράψτε έναν τύπο ημέρας από το "Exception 2" με τύπο ημέρας
    exc2.DaysOfWeek.Remove(DayType.Sunday);
}

// Διαγράψτε έναν τύπο ημέρας από το "Exception 2" με δείκτη
Console.WriteLine("Remove " + exc2.DaysOfWeek[0] + " day type from exception by index...");
exc2.DaysOfWeek.RemoveAt(0);

// Αλλάξτε τις εξαιρέσεις (δεν υπάρχουν εξαιρέσεις στα αρχικά δεδομένα του έργου)
var exc4 = new CalendarException
               {
                   Name = "Weekly Exception 2",
                   FromDate = new DateTime(2020, 4, 13),
                   ToDate = new DateTime(2020, 4, 18),
                   Occurrences = 3,
                   Type = CalendarExceptionType.Weekly
               };
exc4.DaysOfWeek.Add(DayType.Monday);
exc4.DaysOfWeek.Add(DayType.Thursday);

calendar.Exceptions.Add(exc4);

var exc3 = calendar.Exceptions.ToList()[2];

// Αφαιρέστε όλες τις ημέρες της εβδομάδας για το "Exception 3"
exc3.DaysOfWeek.Clear();

var dayTypes = new DayType[exc4.DaysOfWeek.Count];
exc4.DaysOfWeek.CopyTo(dayTypes, 0);

foreach (var dayType in dayTypes)
{
    exc3.DaysOfWeek.Add(dayType);
}

Console.WriteLine("Days of week for exception: " + exc3.Name);
foreach (var dayType in exc3.DaysOfWeek)
{
    Console.WriteLine("Day type: " + dayType);
}
```

### Δείτε επίσης

* enum [DayType](../daytype/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


