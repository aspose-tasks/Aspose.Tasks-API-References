---
title: "Enum CalendarExceptionType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.CalendarExceptionType‑enum. Specificeert het type kalenderuitzondering"
type: docs
weight: 270
url: /nl/net/aspose.tasks/calendarexceptiontype/
---
## CalendarExceptionType enumeration

Specificeert het type kalenderuitzondering.

```csharp
public enum CalendarExceptionType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Daily | `0` | Geeft het dagelijkse uitzonderingstype aan. |
| YearlyByDay | `1` | Geeft het jaarlijkse uitzonderingstype op basis van dag van de maand aan. |
| YearlyByPosition | `2` | Geeft het jaarlijkse uitzonderingstype op basis van positie aan. |
| MonthlyByDay | `3` | Geeft het maandelijkse uitzonderingstype op basis van dag van de maand aan. |
| MonthlyByPosition | `4` | Geeft het maandelijkse uitzonderingstype op basis van positie aan. |
| Weekly | `5` | Geeft wekelijks uitzonderingstype aan. |
| ByDayCount | `6` | Geeft uitzonderingstype per dagtelling aan. |
| ByWeekDayCount | `7` | Geeft uitzonderingstype per weekdagtelling aan. |
| NoExceptionType | `8` | Geeft geen uitzonderingstype aan. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


