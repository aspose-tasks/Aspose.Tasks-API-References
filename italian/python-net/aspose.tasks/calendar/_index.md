---
title: "Calendar"
second_title: "Riferimento API di Aspose.Tasks per Python via .NET"
description: 
type: docs
weight: 140
url: /it/python-net/aspose.tasks/calendar/
---

## Calendar class

Rappresenta un calendario utilizzato in un progetto.

Il tipo Calendar espone i seguenti membri:
## Proprietà
| Nome | Descrizione |
| :- | :- |
| name | Ottiene o imposta il nome del calendario. |
| uid | Ottiene o imposta l'identificatore univoco del calendario. |
| week_days | Ottiene WeekDaysCollection per questo calendario.<br/>            La collezione dei giorni della settimana che definisce il calendario. |
| exceptions | Ottiene l'oggetto CalendarExceptionCollection.<br/>            La collezione delle eccezioni associate al calendario. |
| work_weeks | Ottiene l'oggetto WorkWeekCollections.<br/>            La collezione delle settimane lavorative associate al calendario. |
| is_base_calendar | Ottiene un valore che indica se il calendario è un calendario base. |
| base_calendar | Ottiene o imposta il calendario base da cui dipende questo calendario.<br/>            Applicabile solo se il calendario non è un calendario base. |
| is_baseline_calendar | Ottiene o imposta un valore che indica se il calendario è un calendario di baseline. |
| guid | Ottiene il Guid del calendario. |
| primavera_properties | Ottiene un oggetto contenente le proprietà specifiche di Primavera per un calendario letto dai formati Primavera. |
## Methods
| Nome | Descrizione |
| :- | :- |
| get_start_date_from_finish_and_duration(finish, duration) | Restituisce la data di inizio basata sulla data di fine e sulla durata specificate. |
| get_start_date_from_finish_and_duration(finish, duration) | Restituisce la data di inizio basata sulla data di fine e sulla durata specificate. |
| get_working_hours(start, finish) | Restituisce WorkUnit - Inizio, Fine e Durata delle ore lavorative per l'intervallo di data e ora specificato. |
| get_working_hours(dt) | Restituisce WorkUnit - Inizio, Fine e Durata delle ore lavorative per l'intervallo di data e ora specificato. |
| get_finish_date_by_start_and_work(start, work) | Calcola la data in cui il tempo di lavoro specificato trascorrerà secondo il calendario. |
| get_finish_date_by_start_and_work(start, work) | Calcola la data in cui il tempo di lavoro specificato trascorrerà secondo il calendario. |
| get_intersection_calendar(calendar1, calendar2) | Ottiene l'istanza [ICalendar](/tasks/python-net/aspose.tasks/icalendar/) che può essere usata per eseguire calcoli sull'intersezione degli orari di lavoro di 2 calendari. |
| make_standard_calendar(calendar) | Crea un calendario standard predefinito. |
| make_24_hour_calendar(calendar) | Trasforma un Calendario dato in un Calendario 24Ore.<br/>            Il Calendario 24Ore è un Calendario in cui ogni giorno della settimana è operativo con ore di lavoro 24 ore su 24. |
| make_night_shift_calendar(calendar) | Trasforma un Calendario dato in un Calendario Notturno. |
| delete() | Rimuove il calendario dal progetto. |
| is_day_working(dt) | Determina se il giorno specificato è un giorno lavorativo secondo il calendario. |
| get_working_hours_time_span(start, finish) | Restituisce la quantità di ore lavorative tra le date specificate. |
| get_task_finish_date_from_duration(task, duration) | Calcola la data e l'ora di fine attività a partire dalla sua data di inizio, dalle parti suddivise e dalla durata del lavoro. |
| get_working_times(dt) | Restituisce [WorkingTimeCollection](/tasks/python-net/aspose.tasks/workingtimecollection/) dei tempi di lavoro per la data specificata. |
| get_previous_working_day_end(date) | Calcola la fine della data lavorativa precedente a partire dalla data specificata. |
| get_next_working_day_start(date) | Calcola l'inizio del prossimo giorno lavorativo per la data specificata. |
| get_work_start(date) | Calcola l'inizio del prossimo periodo di lavoro a partire dalla data e ora specificate. |
| is_empty() | Restituisce se il calendario non ha ore lavorative definite. |

### Vedi anche

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

