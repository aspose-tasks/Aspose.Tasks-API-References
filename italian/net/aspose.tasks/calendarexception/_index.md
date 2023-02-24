---
title: Class CalendarException
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Aspose.Tasks.CalendarException classe. Rappresenta periodi di tempo eccezionali in un calendario.
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
| [CalendarException](calendarexception/)() | Inizializza una nuova istanza di`CalendarException` classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DaysOfWeek](../../aspose.tasks/calendarexception/daysofweek/) { get; } | Ottiene il DayTypeCollection per questo oggetto. I giorni della settimana in cui l'eccezione è valida. |
| [DayWorking](../../aspose.tasks/calendarexception/dayworking/) { get; set; } | Ottiene o imposta un valore che indica se la data o il tipo di giorno specificato funziona. |
| [EnteredByOccurrences](../../aspose.tasks/calendarexception/enteredbyoccurrences/) { get; set; } | Ottiene o imposta un valore che indica se l'intervallo di ricorrenza viene definito immettendo un numero di occorrenze. False specifica che l'intervallo di ricorrenza viene definito immettendo una data di fine. |
| [FromDate](../../aspose.tasks/calendarexception/fromdate/) { get; set; } | Ottiene o imposta l'inizio del tempo di eccezione. |
| [Month](../../aspose.tasks/calendarexception/month/) { get; set; } | Ottiene o imposta il mese per il quale è pianificata una ricorrenza di eccezione. |
| [MonthDay](../../aspose.tasks/calendarexception/monthday/) { get; set; } | Ottiene o imposta il giorno di un mese in cui è pianificata una ricorrenza di eccezione. |
| [MonthItem](../../aspose.tasks/calendarexception/monthitem/) { get; set; } | Ottiene o imposta l'elemento del mese per il quale è pianificata una ricorrenza di eccezione. |
| [MonthPosition](../../aspose.tasks/calendarexception/monthposition/) { get; set; } | Ottiene o imposta la posizione di un elemento del mese all'interno di un mese. |
| [Name](../../aspose.tasks/calendarexception/name/) { get; set; } | Ottiene o imposta il nome dell'eccezione. |
| [Occurrences](../../aspose.tasks/calendarexception/occurrences/) { get; set; } | Ottiene o imposta il numero di occorrenze per cui è valida l'eccezione del calendario. |
| [ParentCalendar](../../aspose.tasks/calendarexception/parentcalendar/) { get; } | Ottiene il calendario principale per questo oggetto. |
| [Period](../../aspose.tasks/calendarexception/period/) { get; set; } | Ottiene o imposta il periodo di ricorrenza per l'eccezione. |
| [ToDate](../../aspose.tasks/calendarexception/todate/) { get; set; } | Ottiene o imposta la fine del tempo di eccezione. |
| [Type](../../aspose.tasks/calendarexception/type/) { get; set; } | Ottiene o imposta il tipo di eccezione. |
| [WorkingTimes](../../aspose.tasks/calendarexception/workingtimes/) { get; set; } | Ottiene o imposta l'oggetto WorkingTimeCollection. La raccolta di orari di lavoro che definisce il tempo lavorato nel giorno della settimana.  Deve essere presente almeno un orario di lavoro e non possono essercene più di cinque. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CheckException](../../aspose.tasks/calendarexception/checkexception/)(DateTime) | Restituisce vero se l'istanza specificata diDateTime struct è il giorno dell'eccezione. |
| [Delete](../../aspose.tasks/calendarexception/delete/)() | Elimina l'istanza Exception dall'oggetto calendario principale CalendarExceptionCollection. |
| [GetExceptionDates](../../aspose.tasks/calendarexception/getexceptiondates/)() | Restituisce le date in cui è applicabile l'eccezione del calendario. |
| [GetWorkingTime](../../aspose.tasks/calendarexception/getworkingtime/)() | Restituisce l'orario di lavoro per un'eccezione del calendario. |

### Guarda anche

* spazio dei nomi [Aspose.Tasks](../../aspose.tasks/)
* assemblea [Aspose.Tasks](../../)


