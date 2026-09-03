---
title: "classe Aspose::Tasks::Calendar"
linktitle: "Calendario"
articleTitle: "Calendario"
second_title: "Aspose.Tasks per C++"
description: "Rappresenta un calendario utilizzato in un progetto."
type: docs
weight: 10
url: /it/cpp/aspose.tasks/calendar/
---

## Calendar class

**Inherits:** Aspose::Tasks::ICalendar

Rappresenta un calendario utilizzato in un progetto.

Come creare un calendario semplice da zero.

```cpp
[C#]
// crea calendario vuoto
Calendar calendar = new Calendar("New calendar");
// aggiunge giorni lavorativi predefiniti (8 ore lavorative dalle 9:00 alle 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// crea nuovo giorno lavorativo
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Imposta l'orario di lavoro. Solo la parte oraria di DateTime è importante
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

```cpp
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

I calendari sono usati per definire orari di lavoro e non lavoro standard. I progetti devono avere un calendario base. Le attività e le risorse possono avere i propri calendari non di base che sono basati su un calendario base.

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Delete](./delete/) | Rimuove il calendario dal progetto. |
| [Equals](./equals/) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [get_BaseCalendar](./get_basecalendar/) | Restituisce il calendario base da cui dipende questo calendario. Applicabile solo se il calendario non è un calendario base. |
| [get_Exceptions](./get_exceptions/) | Restituisce l'oggetto CalendarExceptionCollection. La raccolta di eccezioni associata al calendario. |
| [get_Guid](./get_guid/) | Restituisce il Guid del calendario. |
| [get_IsBaseCalendar](./get_isbasecalendar/) | Restituisce un valore che indica se il calendario è un calendario base. |
| [get_IsBaselineCalendar](./get_isbaselinecalendar/) | Restituisce un valore che indica se il calendario è un calendario di baseline. |
| [get_Name](./get_name/) | Restituisce il nome del calendario. |
| [get_Uid](./get_uid/) | Restituisce l'identificatore univoco del calendario. |
| [get_WeekDays](./get_weekdays/) | Restituisce WeekDaysCollection per questo calendario. La raccolta di giorni della settimana che definisce il calendario. |
| [get_WorkWeeks](./get_workweeks/) | Restituisce l'oggetto WorkWeekCollections. La raccolta di settimane lavorative associata al calendario. |
| [GetFinishDateByStartAndWork (2 overloads)](./getfinishdatebystartandwork/) | Calcola la data in cui la quantità specificata di tempo di lavoro trascorrerà secondo il calendario. |
| [GetHashCode](./gethashcode/) | Restituisce un codice hash per l'istanza della classe. |
| [GetIntersectionCalendar](./getintersectioncalendar/) | Restituisce l'istanza ICalendar che può essere usata per eseguire calcoli sull'intersezione degli orari di lavoro di 2 calendari. |
| [GetNextWorkingDayStart](./getnextworkingdaystart/) | Calcola l'inizio del prossimo giorno lavorativo per la data specificata. |
| [GetPreviousWorkingDayEnd](./getpreviousworkingdayend/) | Calcola la fine della data lavorativa precedente dalla data specificata. |
| [GetStartDateFromFinishAndDuration (2 overloads)](./getstartdatefromfinishandduration/) | Restituisce la data di inizio basata sulla data di fine e sulla durata specificate. |
| [GetTaskFinishDateFromDuration](./gettaskfinishdatefromduration/) | Calcola la data e l'ora di fine dell'attività a partire dalla sua data di inizio, dalle parti suddivise e dalla durata del lavoro. |
| [GetWorkingHours (2 overloads)](./getworkinghours/) | Restituisce la quantità di ore lavorative nella data specificata. |
| [GetWorkingHoursTimeSpan](./getworkinghourstimespan/) | Restituisce la quantità di ore lavorative tra le date specificate. |
| [GetWorkingTimes](./getworkingtimes/) | Restituisce WorkingTimeCollection di orari di lavoro per la data specificata. |
| [GetWorkStart](./getworkstart/) | Calcola l'inizio del prossimo orario di lavoro a partire dalla data e ora specificate. |
| [IsDayWorking](./isdayworking/) | Determina se il giorno specificato è un giorno lavorativo secondo il calendario. |
| [IsEmpty](./isempty/) | Restituisce se il calendario non ha ore lavorative definite. |
| [Make24HourCalendar](./make24hourcalendar/) | Trasforma un calendario dato in un Calendario 24Ore. Il Calendario 24Ore è un calendario in cui ogni giorno della settimana è operativo con orari di lavoro 24 ore su 24. |
| [MakeNightShiftCalendar](./makenightshiftcalendar/) | Trasforma un calendario dato in un Calendario Turno Notturno. |
| [MakeStandardCalendar](./makestandardcalendar/) | Crea un calendario standard predefinito. |
| [set_BaseCalendar](./set_basecalendar/) | Imposta il calendario base da cui dipende questo calendario. Applicabile solo se il calendario non è un calendario base. |
| [set_IsBaselineCalendar](./set_isbaselinecalendar/) | Imposta un valore che indica se il calendario è un calendario di baseline. |
| [set_Name](./set_name/) | Imposta il nome del calendario. |
| [set_Uid](./set_uid/) | Imposta l'identificatore univoco del calendario. |

