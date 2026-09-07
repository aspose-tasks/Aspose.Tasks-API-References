---
title: "CalendarException.CheckException"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "CalendarException μέθοδος. Επιστρέφει true εάν η καθορισμένη παρουσία της δομής DateTime είναι η ημέρα της εξαίρεσης."
type: docs
weight: 170
url: /el/net/aspose.tasks/calendarexception/checkexception/
---
## CalendarException.CheckException method

Επιστρέφει true εάν η καθορισμένη παρουσία της δομής DateTime είναι η ημέρα εξαίρεσης.

```csharp
public bool CheckException(DateTime dt)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dt | DateTime | η καθορισμένη παρουσία της δομής DateTime. |

### Τιμή Επιστροφής

Επιστρέφει true εάν η τιμή DateTime είναι η ημέρα της εξαίρεσης· διαφορετικά, false.

## Παραδείγματα

Δείχνει πώς να προσθέσετε/αφαιρέσετε εξαιρέσεις ημερολογίου.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// δημιουργήστε ένα ημερολόγιο
var calendar = project.Calendars.Add("Calendar1");

// Δημιουργήστε εξαίρεση ημερών της εβδομάδας για μια αργία.
var exception = new CalendarException();
exception.Name = "New Calendar Exception";
exception.EnteredByOccurrences = false;
exception.FromDate = new DateTime(2009, 12, 24, 0, 0, 0);
exception.ToDate = new DateTime(2009, 12, 31, 23, 59, 0);
exception.Type = CalendarExceptionType.Daily;
exception.Month = Month.December;

exception.DayWorking = false;

// Ελέγξτε αν η ημερομηνία είναι εξαιρετική.
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2009, 12, 26, 8, 0, 0)));

calendar.Exceptions.Add(exception);

// Αφαιρέστε μια εξαίρεση.
var cal = project.Calendars.ToList()[0];
if (cal.Exceptions.Count > 1)
{
    var excToRemove = cal.Exceptions[0];
    cal.Exceptions.Remove(excToRemove);
}

// Προσθέστε μια εξαίρεση.
var exception2 = new CalendarException();
exception2.FromDate = new System.DateTime(2009, 1, 1);
exception2.ToDate = new System.DateTime(2009, 1, 3);
cal.Exceptions.Add(exception2);

// Εκτυπώστε τις εξαιρέσεις.
foreach (var exc in cal.Exceptions)
{
    Console.WriteLine("Name: " + exc.Name);
    Console.WriteLine("From: " + exc.FromDate.ToShortDateString());
    Console.WriteLine("To: " + exc.ToDate.ToShortDateString());
}
```

### Δείτε επίσης

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


