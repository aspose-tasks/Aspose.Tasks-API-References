---
title: "CalendarException.GetWorkingTime"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "CalendarException μέθοδος. Επιστρέφει τον χρόνο εργασίας για μια εξαίρεση ημερολογίου."
type: docs
weight: 200
url: /el/net/aspose.tasks/calendarexception/getworkingtime/
---
## CalendarException.GetWorkingTime method

Επιστρέφει τον χρόνο εργασίας για μια εξαίρεση ημερολογίου.

```csharp
public TimeSpan GetWorkingTime()
```

### Τιμή Επιστροφής

Επιστρέφει τον χρόνο εργασίας για αυτήν την εξαίρεση ημερολογίου.

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

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


