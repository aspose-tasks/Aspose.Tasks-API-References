---
title: "Calendar.Exceptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Calendar-eigenschap. Haalt een CalendarExceptionCollection-object op. De verzameling uitzonderingen die aan de kalender zijn gekoppeld"
type: docs
weight: 50
url: /nl/net/aspose.tasks/calendar/exceptions/
---
## Calendar.Exceptions property

Haalt CalendarExceptionCollection‑object op. De verzameling uitzonderingen die aan de kalender zijn gekoppeld.

```csharp
public CalendarExceptionCollection Exceptions { get; }
```

## Voorbeelden

Toont hoe informatie over kalenderuitzonderingen op te halen.

```csharp
var project = new Project(DataDir + "project_RetrieveExceptions_test.mpp");

// Itereer over kalenders
foreach (var calendar in project.Calendars)
{
    // Toegang tot kalenderuitzonderingen
    foreach (var exception in calendar.Exceptions)
    {
        Console.WriteLine("From: " + exception.FromDate.ToShortDateString());
        Console.WriteLine("To: " + exception.ToDate.ToShortDateString());
    }
}
```

### Zie ook

* class [CalendarExceptionCollection](../../calendarexceptioncollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


