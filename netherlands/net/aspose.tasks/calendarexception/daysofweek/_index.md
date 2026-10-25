---
title: "CalendarException.DaysOfWeek"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CalendarException property. Haalt de DayTypeCollection op voor dit object. De dagen van de week waarop de uitzondering geldig is"
type: docs
weight: 20
url: /nl/net/aspose.tasks/calendarexception/daysofweek/
---
## CalendarException.DaysOfWeek property

Haalt de DayTypeCollection op voor dit object. De dagen van de week waarop de uitzondering geldig is.

```csharp
public DayTypeCollection DaysOfWeek { get; }
```

## Voorbeelden

Toont hoe een kalenderuitzondering per weekdag te definiëren.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// maak een kalender
var calendar = project.Calendars.Add("Calendar1");

// maak een kalenderuitzondering voor elke vrijdag
var exception = new CalendarException();
exception.Type = CalendarExceptionType.Weekly;
exception.FromDate = new DateTime(2020, 4, 6);
exception.ToDate = new DateTime(2020, 4, 12);
exception.DaysOfWeek.Add(DayType.Friday);

// controleer dat vrijdag uitzonderlijk is
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2020, 4, 10)));

// voeg de uitzondering toe aan de agenda
calendar.Exceptions.Add(exception);
```

### Zie ook

* class [DayTypeCollection](../../daytypecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


