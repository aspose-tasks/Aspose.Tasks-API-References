---
title: "CalendarException.MonthPosition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "CalendarException proprietà. Ottiene o imposta la posizione di un elemento del mese all'interno di un mese"
type: docs
weight: 90
url: /it/net/aspose.tasks/calendarexception/monthposition/
---
## CalendarException.MonthPosition property

Ottiene o imposta la posizione di un elemento del mese all'interno di un mese.

```csharp
public MonthPosition MonthPosition { get; set; }
```

## Esempi

Mostra come definire un'eccezione di calendario per giorno del mese.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// crea un calendario
var calendar = project.Calendars.Add("Calendar1");

// crea un'eccezione di calendario per ogni venerdì
var exception = new CalendarException();
exception.Type = CalendarExceptionType.MonthlyByDay;
exception.FromDate = new DateTime(2010, 1, 1);
exception.ToDate = new DateTime(2020, 12, 31);
exception.Month = Month.December;
exception.MonthDay = 1;
exception.MonthItem = MonthItemType.Undefined;
exception.MonthPosition = MonthPosition.Last;
exception.Period = 5;

// verifica che un venerdì sia eccezionale
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2012, 12, 1)));

// aggiungi l'eccezione al calendario
calendar.Exceptions.Add(exception);
```

### Vedi anche

* enum [MonthPosition](../../monthposition/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


