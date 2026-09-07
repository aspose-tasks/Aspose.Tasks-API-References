---
title: "CalendarException.MonthDay"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "CalendarException proprietà. Ottiene o imposta il giorno del mese in cui è programmata una ricorrenza di eccezione"
type: docs
weight: 70
url: /it/net/aspose.tasks/calendarexception/monthday/
---
## CalendarException.MonthDay property

Ottiene o imposta il giorno del mese in cui è programmata una ricorrenza di eccezione.

```csharp
public int MonthDay { get; set; }
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

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


