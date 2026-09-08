---
title: "CalendarException.EnteredByOccurrences"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CalendarException property. Haalt een waarde op of stelt deze in die aangeeft of het bereik van de herhaling wordt gedefinieerd door een aantal herhalingen in te voeren. False geeft aan dat het bereik van de herhaling wordt gedefinieerd door een einddatum in te voeren."
type: docs
weight: 40
url: /nl/net/aspose.tasks/calendarexception/enteredbyoccurrences/
---
## CalendarException.EnteredByOccurrences property

Haalt op of stelt een waarde in die aangeeft of het bereik van herhaling wordt gedefinieerd door een aantal herhalingen in te voeren. False geeft aan dat het bereik van herhaling wordt gedefinieerd door een einddatum in te voeren.

```csharp
public bool EnteredByOccurrences { get; set; }
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


