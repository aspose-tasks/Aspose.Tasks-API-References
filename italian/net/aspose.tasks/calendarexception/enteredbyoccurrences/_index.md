---
title: "CalendarException.EnteredByOccurrences"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà CalendarException. Ottiene o imposta un valore che indica se l'intervallo di ricorrenza è definito inserendo un numero di occorrenze. False specifica che l'intervallo di ricorrenza è definito inserendo una data di fine."
type: docs
weight: 40
url: /it/net/aspose.tasks/calendarexception/enteredbyoccurrences/
---
## CalendarException.EnteredByOccurrences property

Ottiene o imposta un valore che indica se l'intervallo di ricorrenza è definito inserendo un numero di occorrenze. False specifica che l'intervallo di ricorrenza è definito inserendo una data di fine.

```csharp
public bool EnteredByOccurrences { get; set; }
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


