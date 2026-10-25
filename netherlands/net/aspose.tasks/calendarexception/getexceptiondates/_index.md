---
title: "CalendarException.GetExceptionDates"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CalendarException method. Retourneert datums waarop de kalenderuitzondering van toepassing is"
type: docs
weight: 190
url: /nl/net/aspose.tasks/calendarexception/getexceptiondates/
---
## CalendarException.GetExceptionDates method

Retourneert data waarop de kalenderuitzondering van toepassing is.

```csharp
public IEnumerable<DateTime> GetExceptionDates()
```

### Retourwaarde

Retourneert een collectie van uitzonderingsdatums waarvoor de kalenderuitzondering van toepassing is.

## Voorbeelden

Toont hoe datums op te halen waarvoor een specifieke kalenderuitzondering van kracht is.

```csharp
Project project = new Project(DataDir + "CalendarExceptions.mpp");
Calendar calendar = project.Calendars.GetByUid(1);
CalendarException calendarException = calendar.Exceptions[0];

foreach (var date in calendarException.GetExceptionDates())
{
    Console.WriteLine(date);
}
```

### Zie ook

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


