---
title: "Classe Calendar"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Calendar. Rappresenta un calendario utilizzato in un progetto"
type: docs
weight: 230
url: /it/net/aspose.tasks/calendar/
---
## Calendar class

Rappresenta un calendario utilizzato in un progetto.

```csharp
public class Calendar : ICalendar
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | Ottiene o imposta il calendario base da cui dipende questo calendario. Applicabile solo se il calendario non è un calendario base. |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | Ottiene l'oggetto CalendarExceptionCollection. La raccolta di eccezioni associata al calendario. |
| [Guid](../../aspose.tasks/calendar/guid/) { get; } | Ottiene il Guid del calendario. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | Ottiene un valore che indica se il calendario è un calendario base. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | Ottiene o imposta un valore che indica se il calendario è un calendario di baseline. |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | Ottiene o imposta il nome del calendario. |
| [PrimaveraProperties](../../aspose.tasks/calendar/primaveraproperties/) { get; } | Ottiene un oggetto contenente proprietà specifiche di Primavera per un calendario letto da formati Primavera. |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | Ottiene o imposta l'identificatore univoco del calendario. |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | Ottiene la WeekDaysCollection per questo calendario. La raccolta dei giorni della settimana che definisce il calendario. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | Ottiene l'oggetto WorkWeekCollections. La raccolta delle settimane lavorative associate al calendario. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | Trasforma un calendario dato in un Calendario 24Ore. Il Calendario 24Ore è un calendario in cui ogni giorno della settimana è lavorativo con orari di lavoro 24 ore su 24. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | Crea un Calendario Notturno a partire da un calendario fornito. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | Crea un calendario standard predefinito. |
| [Delete](../../aspose.tasks/calendar/delete/)() | Rimuove il calendario dal progetto. |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Calcola la data in cui il tempo di lavoro specificato sarà trascorso secondo il calendario. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Calcola la data in cui il tempo di lavoro specificato sarà trascorso secondo il calendario. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | Restituisce un codice hash per l'istanza della classe. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | Calcola l'inizio del prossimo giorno lavorativo per la data specificata. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | Calcola la fine della data lavorativa precedente a partire dalla data specificata. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Restituisce la data di inizio basata sulla data di fine e sulla durata specificate. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Restituisce la data di inizio basata sulla data di fine e sulla durata specificate. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Calcola la data e l'ora di fine dell'attività a partire dalla sua data di inizio, dalle parti suddivise e dalla durata del lavoro. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | Restituisce la quantità di ore lavorative nella data specificata. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Restituisce WorkUnit - Inizio, Fine e Durata delle ore lavorative per l'intervallo di data/ora specificato. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/calendar/getworkinghourstimespan/)(DateTime, DateTime) | Restituisce la quantità di ore lavorative tra le date specificate. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | Restituisce [`WorkingTimeCollection`](../workingtimecollection/) di orari di lavoro per la data specificata. |
| [GetWorkStart](../../aspose.tasks/calendar/getworkstart/)(DateTime) | Calcola l'inizio del prossimo orario lavorativo a partire dalla data e ora specificate. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | Determina se il giorno specificato è un giorno lavorativo secondo il calendario. |
| virtual [IsEmpty](../../aspose.tasks/calendar/isempty/)() | Restituisce se il calendario non ha ore lavorative definite. |
| static [GetIntersectionCalendar](../../aspose.tasks/calendar/getintersectioncalendar/)(Calendar, Calendar) | Ottiene l'istanza [`ICalendar`](../icalendar/) che può essere usata per eseguire calcoli sull'intersezione degli orari di lavoro di 2 calendari. |

## Osservazioni

I calendari sono usati per definire i tempi di lavoro e non lavoro standard. I progetti devono avere un calendario base. Attività e risorse possono avere i propri calendari non base basati su un calendario base.

## Esempi

Come creare un calendario semplice da zero.

```csharp
[C#]
// crea un calendario vuoto
Calendar calendar = new Calendar("New calendar");
// aggiunge giorni lavorativi predefiniti (8 ore lavorative dalle 9:00 alle 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// crea un nuovo giorno lavorativo
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Imposta l'orario di lavoro. È importante solo la parte ora di DateTime
    WorkingTime wt1 = new WorkingTime();
    wt1.FromTime = new DateTime(1, 1, 1, 6, 0, 0, 0);
    wt1.ToTime = new DateTime(1, 1, 1, 12, 0, 0, 0);
    WorkingTime wt2 = new WorkingTime();
    wt2.FromTime = new DateTime(1, 1, 1, 14, 0, 0, 0);
    wt2.ToTime = new DateTime(1, 1, 1, 18, 0, 0, 0);
    myWeekDay.WorkingTimes.Add(wt1);
    myWeekDay.WorkingTimes.Add(wt2);
    myWeekDay.DayWorking = true;
calendar.Days.Add(myWeekDay);
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
// aggiunge il weekend
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
' create empty calendar
Dim calendar As Calendar =  New Calendar("New calendar")
' adds default working days (8 working hours from 9:00 to 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' create new new working day
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Sets working time. Only time part of DateTime is important
    Dim wt1 As WorkingTime =  New WorkingTime()
    wt1.FromTime = New DateTime(1, 1, 1, 6, 0, 0, 0)
    wt1.ToTime = New DateTime(1, 1, 1, 12, 0, 0, 0)
    Dim wt2 As WorkingTime =  New WorkingTime()
    wt2.FromTime = New DateTime(1, 1, 1, 14, 0, 0, 0)
    wt2.ToTime = New DateTime(1, 1, 1, 18, 0, 0, 0)
    myWeekDay.WorkingTimes.Add(wt1)
    myWeekDay.WorkingTimes.Add(wt2)
    myWeekDay.DayWorking = True
calendar.Days.Add(myWeekDay)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday))
' adds weekend
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

Mostra come definire un nuovo calendario, aggiungere i giorni della settimana e definire gli orari di lavoro per i giorni.

```csharp
var project = new Project();

// Definisci un calendario
var calendar = project.Calendars.Add("Calendar1");

// Aggiungi giorni lavorativi da lunedì a giovedì con gli orari predefiniti
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Imposta il venerdì come giorno lavorativo breve
var weekDay = new WeekDay(DayType.Friday);

// Imposta l'orario di lavoro. È importante solo la parte ora di DateTime
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// lavorare con il progetto...
```

### Vedi anche

* interface [ICalendar](../icalendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


