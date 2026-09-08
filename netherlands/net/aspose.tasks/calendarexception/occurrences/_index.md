---
title: "CalendarException.Occurrences"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CalendarException property. Haalt op of stelt het aantal keren in waarvoor de kalenderuitzondering geldig is"
type: docs
weight: 110
url: /nl/net/aspose.tasks/calendarexception/occurrences/
---
## CalendarException.Occurrences property

Haalt op of stelt het aantal herhalingen in waarvoor de kalenderuitzondering geldig is.

```csharp
public int Occurrences { get; set; }
```

## Voorbeelden

Toont hoe een kalenderuitzondering te definiëren op basis van gebeurtenissen.

```csharp
var project = new Project();

// Definieer een kalender
var calendar = project.Calendars.Add("Calendar1");

// Definieer uitzondering en specificeer gebeurtenissen
var exception = new CalendarException();
exception.EnteredByOccurrences = true;
exception.Occurrences = 5;
exception.Type = CalendarExceptionType.YearlyByDay;
exception.MonthDay = 22;
exception.Month = Month.April;

// Voeg uitzondering toe aan kalender
calendar.Exceptions.Add(exception);
```

### Zie ook

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


