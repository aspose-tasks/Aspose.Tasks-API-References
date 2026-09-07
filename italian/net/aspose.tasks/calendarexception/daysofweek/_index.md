---
title: "CalendarException.DaysOfWeek"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "CalendarException proprietà. Ottiene la DayTypeCollection per questo oggetto. I giorni della settimana in cui l'eccezione è valida"
type: docs
weight: 20
url: /it/net/aspose.tasks/calendarexception/daysofweek/
---
## CalendarException.DaysOfWeek property

Ottiene la DayTypeCollection per questo oggetto. I giorni della settimana in cui l'eccezione è valida.

```csharp
public DayTypeCollection DaysOfWeek { get; }
```

## Esempi

Mostra come definire un'eccezione di calendario per giorno della settimana.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// crea un calendario
var calendar = project.Calendars.Add("Calendar1");

// crea un'eccezione di calendario per ogni venerdì
var exception = new CalendarException();
exception.Type = CalendarExceptionType.Weekly;
exception.FromDate = new DateTime(2020, 4, 6);
exception.ToDate = new DateTime(2020, 4, 12);
exception.DaysOfWeek.Add(DayType.Friday);

// verifica che venerdì sia eccezionale
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2020, 4, 10)));

// aggiungi l'eccezione al calendario
calendar.Exceptions.Add(exception);
```

### Vedi anche

* class [DayTypeCollection](../../daytypecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


