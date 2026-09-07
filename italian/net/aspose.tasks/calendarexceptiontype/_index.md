---
title: "Enum CalendarExceptionType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.CalendarExceptionType enum. Specifica il tipo di eccezione del calendario"
type: docs
weight: 270
url: /it/net/aspose.tasks/calendarexceptiontype/
---
## CalendarExceptionType enumeration

Specifica il tipo di eccezione del calendario.

```csharp
public enum CalendarExceptionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Daily | `0` | Indica il tipo di eccezione giornaliera. |
| YearlyByDay | `1` | Indica il tipo di eccezione annuale per giorno del mese. |
| YearlyByPosition | `2` | Indica il tipo di eccezione annuale per posizione. |
| MonthlyByDay | `3` | Indica il tipo di eccezione mensile per giorno del mese. |
| MonthlyByPosition | `4` | Indica il tipo di eccezione mensile per posizione. |
| Weekly | `5` | Indica il tipo di eccezione settimanale. |
| ByDayCount | `6` | Indica il tipo di eccezione per conteggio giornaliero. |
| ByWeekDayCount | `7` | Indica il tipo di eccezione per conteggio dei giorni della settimana. |
| NoExceptionType | `8` | Indica nessun tipo di eccezione. |

## Esempi

Mostra come definire un'eccezione del calendario per occorrenze.

```csharp
var project = new Project();

// Definisci un calendario
var calendar = project.Calendars.Add("Calendar1");

// Definisci l'eccezione e specifica le occorrenze
var exception = new CalendarException();
exception.EnteredByOccurrences = true;
exception.Occurrences = 5;
exception.Type = CalendarExceptionType.YearlyByDay;
exception.MonthDay = 22;
exception.Month = Month.April;

// Aggiungi un'eccezione al calendario
calendar.Exceptions.Add(exception);
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


