---
title: "CalendarException.MonthDay"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CalendarException property. Haalt op of stelt de dag van de maand in waarop een uitzondering herhaling is gepland"
type: docs
weight: 70
url: /nl/net/aspose.tasks/calendarexception/monthday/
---
## CalendarException.MonthDay property

Haalt op of stelt de dag van de maand in waarop een uitzonderingherhaling is gepland.

```csharp
public int MonthDay { get; set; }
```

## Voorbeelden

Toont hoe een kalenderuitzondering per maanddag te definiëren.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// maak een kalender
var calendar = project.Calendars.Add("Calendar1");

// maak een kalenderuitzondering voor elke vrijdag
var exception = new CalendarException();
exception.Type = CalendarExceptionType.MonthlyByDay;
exception.FromDate = new DateTime(2010, 1, 1);
exception.ToDate = new DateTime(2020, 12, 31);
exception.Month = Month.December;
exception.MonthDay = 1;
exception.MonthItem = MonthItemType.Undefined;
exception.MonthPosition = MonthPosition.Last;
exception.Period = 5;

// controleer dat een vrijdag uitzonderlijk is.
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2012, 12, 1)));

// voeg de uitzondering toe aan de agenda
calendar.Exceptions.Add(exception);
```

### Zie ook

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


