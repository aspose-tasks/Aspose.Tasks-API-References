---
title: Calendar
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Rappresenta un calendario utilizzato in un progetto.
type: docs
weight: 220
url: /it/net/aspose.tasks/calendar/
---
## Calendar class

Rappresenta un calendario utilizzato in un progetto.

```csharp
public class Calendar
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar) { get; set; } | Ottiene o imposta il calendario di base da cui dipende questo calendario. Applicabile solo se il calendario non è un calendario di base. Lettura/scrittura[`Calendar`](../calendar) . |
| [Exceptions](../../aspose.tasks/calendar/exceptions) { get; } | Ottiene l'oggetto CalendarExceptionCollection. La raccolta di eccezioni associata al calendario. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar) { get; } | Ottiene un valore che indica se il calendario è un calendario di base. Sola letturaBoolean . |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar) { get; set; } | Ottiene o imposta un valore che indica se il calendario è un calendario di base. Lettura/scritturaBoolean . |
| [Name](../../aspose.tasks/calendar/name) { get; set; } | Ottiene o imposta il nome del calendario. Lettura/scritturaString . |
| [ParentProject](../../aspose.tasks/calendar/parentproject) { get; } | Ottiene il progetto principale per questo calendario. |
| [Uid](../../aspose.tasks/calendar/uid) { get; set; } | Ottiene o imposta l'identificatore univoco del calendario. Lettura/scritturaInt32 . |
| [WeekDays](../../aspose.tasks/calendar/weekdays) { get; } | Ottiene WeekDaysCollection per questo calendario. La raccolta di giorni della settimana che definisce il calendario. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks) { get; } | Ottiene l'oggetto WorkWeekCollections. La raccolta di settimane lavorative associata al calendario. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar)(Calendar) | Trasforma un determinato calendario in un calendario di 24 ore. Il calendario di 24 ore è un calendario in cui ogni giorno della settimana lavora con orari di lavoro 24 ore su 24. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar)(Calendar) | Crea un determinato calendario come calendario dei turni notturni. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar)(Calendar) | Crea un calendario standard predefinito. |
| [Delete](../../aspose.tasks/calendar/delete)() | Rimuove il calendario dal progetto. |
| override [Equals](../../aspose.tasks/calendar/equals)(object) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork#getfinishdatebystartandwork)(DateTime, Duration) | Calcola la data in cui trascorrerà il tempo di lavoro specificato in base al calendario. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Calcola la data in cui trascorrerà il tempo di lavoro specificato in base al calendario. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode)() | Restituisce un codice hash per l'istanza di[`Calendar`](../calendar) classe. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart)(DateTime) | Calcola il giorno lavorativo successivo a partire dalla data. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend)(DateTime) | Calcola la data di fine lavoro precedente dalla data specificata. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration#getstartdatefromfinishandduration)(DateTime, Duration) | Restituisce StartDate in base a FinishDate e Duration specificati. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Restituisce StartDate in base a FinishDate e Duration specificati. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration)(Task, TimeSpan) | Calcola la data e l'ora di fine dell'attività dalla data di inizio, le parti divise e la durata. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours#getworkinghours_1)(DateTime) | Restituisce la quantità di ore lavorative alla data. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours#getworkinghours)(DateTime, DateTime) | Restituisci l'orario di lavoro per le date specificate. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes)(DateTime) | Restituisce[`WorkingTimeCollection`](../workingtimecollection) dei tempi di lavoro. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking)(DateTime) | Determina se il giorno è lavorativo. |

### Osservazioni

I calendari vengono utilizzati per definire gli orari di lavoro e non lavorativi standard. I progetti devono avere un calendario di base. Le attività e le risorse possono avere i propri calendari non di base basati su un calendario di base.

### Esempi

Come creare un semplice calendario da zero.

```csharp
[C#]
// crea un calendario vuoto
Calendar calendar = new Calendar("New calendar");
// aggiunge giorni lavorativi predefiniti (8 ore lavorative dalle 9:00 alle 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// crea un nuovo nuovo giorno lavorativo
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Imposta l'orario di lavoro. Solo la parte temporale di DateTime è importante
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
// aggiunge il fine settimana
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
' crea un calendario vuoto
Dim calendar As Calendar =  New Calendar("New calendar")
' aggiunge giorni lavorativi predefiniti (8 ore lavorative dalle 9:00 alle 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' creare una nuova nuova giornata lavorativa
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Imposta l'orario di lavoro. Solo la parte temporale di DateTime è importante
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
' aggiunge il fine settimana
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

### Guarda anche

* spazio dei nomi [Aspose.Tasks](../../aspose.tasks)
* assemblea [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
