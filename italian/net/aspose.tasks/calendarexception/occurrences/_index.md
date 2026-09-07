---
title: "CalendarException.Occurrences"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "CalendarException proprietà. Ottiene o imposta il numero di occorrenze per le quali l'eccezione di calendario è valida"
type: docs
weight: 110
url: /it/net/aspose.tasks/calendarexception/occurrences/
---
## CalendarException.Occurrences property

Ottiene o imposta il numero di occorrenze per le quali l'eccezione del calendario è valida.

```csharp
public int Occurrences { get; set; }
```

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

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


