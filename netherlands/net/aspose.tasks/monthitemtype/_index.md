---
title: "Enum MonthItemType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.MonthItemType‑enum. Specificeert het maanditem waarvoor een uitzonderingsherhaling is gepland"
type: docs
weight: 1050
url: /nl/net/aspose.tasks/monthitemtype/
---
## MonthItemType enumeration

Specificeert het maanditem waarvoor een uitzondering‑herhaling is gepland.

```csharp
public enum MonthItemType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Undefined | `-1` | Geeft een ongedefinieerd maanditemtype aan. |
| Day | `0` | Geeft een dag‑maanditemtype aan. |
| Weekday | `1` | Geeft een weekdag‑maanditemtype aan. |
| WeekendDay | `2` | Geeft een weekenddag‑maanditemtype aan. |
| Sunday | `3` | Geeft een zondag‑maanditemtype aan. |
| Monday | `4` | Geeft een maandag‑maanditemtype aan. |
| Tuesday | `5` | Geeft een dinsdag‑maanditemtype aan. |
| Wednesday | `6` | Geeft een woensdag‑maanditemtype aan. |
| Thursday | `7` | Geeft een donderdag‑maanditemtype aan. |
| Friday | `8` | Geeft een vrijdag‑maanditemtype aan. |
| Saturday | `9` | Geeft een zaterdag‑maanditemtype aan. |

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


