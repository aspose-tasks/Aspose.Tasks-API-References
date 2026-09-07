---
title: "CalendarException.WorkingTimes"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "CalendarException ιδιότητα. Λαμβάνει ή ορίζει το αντικείμενο WorkingTimeCollection. Η συλλογή των χρόνων εργασίας που ορίζει τον χρόνο εργασίας κατά την ημέρα της εβδομάδας. Πρέπει να υπάρχει τουλάχιστον ένας χρόνος εργασίας και δεν μπορεί να υπάρχουν περισσότεροι από πέντε."
type: docs
weight: 160
url: /el/net/aspose.tasks/calendarexception/workingtimes/
---
## CalendarException.WorkingTimes property

Λαμβάνει ή ορίζει το αντικείμενο WorkingTimeCollection. Η συλλογή των ωρών εργασίας που ορίζει τον χρόνο εργασίας κατά τη διάρκεια της εβδομάδας. Πρέπει να υπάρχει τουλάχιστον μία ώρα εργασίας και δεν μπορούν να υπάρχουν περισσότερες από πέντε.

```csharp
public WorkingTimeCollection WorkingTimes { get; set; }
```

## Παραδείγματα

Δείχνει πώς να λάβετε τον χρόνο εργασίας μιας εξαίρεσης ημερολογίου.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];
var exception = calendar.Exceptions[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
Console.WriteLine("Calendar Exception Name: " + exception.Name);
Console.WriteLine();

var workingTime = exception.GetWorkingTime();
Console.WriteLine("Exception Working Time: " + workingTime);

foreach (var time in exception.WorkingTimes)
{
    Console.WriteLine("Working Time Start: " + time.From);
    Console.WriteLine("Working Time Finish: " + time.To);
}
```

### Δείτε επίσης

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


