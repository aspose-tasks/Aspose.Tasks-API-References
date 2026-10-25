---
title: "Classe CalendarException"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.CalendarException. Rappresenta periodi di tempo eccezionali in un calendario"
type: docs
weight: 250
url: /it/net/aspose.tasks/calendarexception/
---
## CalendarException class

Rappresenta periodi di tempo eccezionali in un calendario.

```csharp
public sealed class CalendarException
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [CalendarException](calendarexception/)() | Inizializza una nuova istanza della classe `CalendarException`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DaysOfWeek](../../aspose.tasks/calendarexception/daysofweek/) { get; } | Ottiene la DayTypeCollection per questo oggetto. I giorni della settimana in cui l'eccezione è valida. |
| [DayWorking](../../aspose.tasks/calendarexception/dayworking/) { get; set; } | Ottiene o imposta un valore che indica se la data o il tipo di giorno specificato è lavorativo. |
| [EnteredByOccurrences](../../aspose.tasks/calendarexception/enteredbyoccurrences/) { get; set; } | Ottiene o imposta un valore che indica se l'intervallo di ricorrenza è definito inserendo un numero di occorrenze. False specifica che l'intervallo di ricorrenza è definito inserendo una data di fine. |
| [FromDate](../../aspose.tasks/calendarexception/fromdate/) { get; set; } | Ottiene o imposta l'inizio del periodo di eccezione. |
| [Month](../../aspose.tasks/calendarexception/month/) { get; set; } | Ottiene o imposta il mese per il quale è programmata una ricorrenza di eccezione. |
| [MonthDay](../../aspose.tasks/calendarexception/monthday/) { get; set; } | Ottiene o imposta il giorno del mese in cui è programmata una ricorrenza di eccezione. |
| [MonthItem](../../aspose.tasks/calendarexception/monthitem/) { get; set; } | Ottiene o imposta l'elemento del mese per il quale è programmata una ricorrenza di eccezione. |
| [MonthPosition](../../aspose.tasks/calendarexception/monthposition/) { get; set; } | Ottiene o imposta la posizione di un elemento del mese all'interno di un mese. |
| [Name](../../aspose.tasks/calendarexception/name/) { get; set; } | Ottiene o imposta il nome dell'eccezione. |
| [Occurrences](../../aspose.tasks/calendarexception/occurrences/) { get; set; } | Ottiene o imposta il numero di occorrenze per le quali l'eccezione del calendario è valida. |
| [ParentCalendar](../../aspose.tasks/calendarexception/parentcalendar/) { get; } | Ottiene il calendario principale per questo oggetto. |
| [Period](../../aspose.tasks/calendarexception/period/) { get; set; } | Ottiene o imposta il periodo di ricorrenza per l'eccezione. |
| [ToDate](../../aspose.tasks/calendarexception/todate/) { get; set; } | Ottiene o imposta la fine del periodo di eccezione. |
| [Type](../../aspose.tasks/calendarexception/type/) { get; set; } | Ottiene o imposta il tipo di eccezione. |
| [WorkingTimes](../../aspose.tasks/calendarexception/workingtimes/) { get; set; } | Ottiene o imposta l'oggetto WorkingTimeCollection. La collezione di orari di lavoro che definisce il tempo lavorato nei giorni feriali. Deve essere presente almeno un orario di lavoro e non possono esserne più di cinque. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CheckException](../../aspose.tasks/calendarexception/checkexception/)(DateTime) | Restituisce true se l'istanza specificata della struct DateTime è il giorno di eccezione. |
| [Delete](../../aspose.tasks/calendarexception/delete/)() | Elimina l'istanza Exception dall'oggetto CalendarExceptionCollection del calendario padre. |
| [GetExceptionDates](../../aspose.tasks/calendarexception/getexceptiondates/)() | Restituisce le date in cui l'eccezione del calendario è applicabile. |
| [GetWorkingTime](../../aspose.tasks/calendarexception/getworkingtime/)() | Restituisce il tempo di lavoro per un'eccezione del calendario. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


