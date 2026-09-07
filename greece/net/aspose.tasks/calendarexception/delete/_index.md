---
title: "CalendarException.Delete"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "CalendarException μέθοδος. Διαγράφει το αντικείμενο Exception από το γονικό ημερολόγιο CalendarExceptionCollection"
type: docs
weight: 180
url: /el/net/aspose.tasks/calendarexception/delete/
---
## CalendarException.Delete method

Διαγράφει την παρουσία Exception από το αντικείμενο CalendarExceptionCollection του γονικού ημερολογίου.

```csharp
public void Delete()
```

## Παραδείγματα

Δείχνει πώς να διαγράψετε μια εξαίρεση ημερολογίου.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);

// αφαιρέστε την εξαίρεση
calendar.Exceptions[0].Delete();

Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
```

### Δείτε επίσης

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


