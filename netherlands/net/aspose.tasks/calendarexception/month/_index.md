---
title: "CalendarException.Month"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CalendarException property. Haalt op of stelt de maand in waarvoor een uitzondering herhaling is gepland"
type: docs
weight: 60
url: /nl/net/aspose.tasks/calendarexception/month/
---
## CalendarException.Month property

Haalt op of stelt de maand in waarvoor een uitzonderingherhaling is gepland.

```csharp
public Month Month { get; set; }
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

* enum [Month](../../month/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


