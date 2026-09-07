---
title: "CalendarException.ToDate"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "CalendarException proprietà. Ottiene o imposta la fine del periodo dell'eccezione"
type: docs
weight: 140
url: /it/net/aspose.tasks/calendarexception/todate/
---
## CalendarException.ToDate property

Ottiene o imposta la fine del periodo di eccezione.

```csharp
public DateTime ToDate { get; set; }
```

## Esempi

Mostra come aggiungere/rimuovere le eccezioni del calendario.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// crea un calendario
var calendar = project.Calendars.Add("Calendar1");

// crea un'eccezione per i giorni della settimana per una festività
var exception = new CalendarException();
exception.Name = "New Calendar Exception";
exception.EnteredByOccurrences = false;
exception.FromDate = new DateTime(2009, 12, 24, 0, 0, 0);
exception.ToDate = new DateTime(2009, 12, 31, 23, 59, 0);
exception.Type = CalendarExceptionType.Daily;
exception.Month = Month.December;

exception.DayWorking = false;

// verifica che la data sia eccezionale
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2009, 12, 26, 8, 0, 0)));

calendar.Exceptions.Add(exception);

// rimuovi un'eccezione
var cal = project.Calendars.ToList()[0];
if (cal.Exceptions.Count > 1)
{
    var excToRemove = cal.Exceptions[0];
    cal.Exceptions.Remove(excToRemove);
}

// aggiungi un'eccezione
var exception2 = new CalendarException();
exception2.FromDate = new System.DateTime(2009, 1, 1);
exception2.ToDate = new System.DateTime(2009, 1, 3);
cal.Exceptions.Add(exception2);

// stampa le eccezioni
foreach (var exc in cal.Exceptions)
{
    Console.WriteLine("Name: " + exc.Name);
    Console.WriteLine("From: " + exc.FromDate.ToShortDateString());
    Console.WriteLine("To: " + exc.ToDate.ToShortDateString());
}
```

### Vedi anche

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


