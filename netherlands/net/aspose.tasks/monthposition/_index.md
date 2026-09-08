---
title: "Enum MonthPosition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.MonthPosition enum. Specificeert de positie van een maanditem binnen een maand."
type: docs
weight: 1070
url: /nl/net/aspose.tasks/monthposition/
---
## MonthPosition enumeration

Specificeert de positie van een maanditem binnen een maand.

```csharp
public enum MonthPosition
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Undefined | `-1` | Geeft een ongedefinieerde maandpositie aan. |
| First | `0` | Geeft de eerste positie van de maand aan. |
| Second | `1` | Geeft de tweede positie van de maand aan. |
| Third | `2` | Geeft de derde positie van de maand aan. |
| Fourth | `3` | Geeft de vierde positie van de maand aan. |
| Last | `4` | Geeft de laatste positie van de maand aan. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


