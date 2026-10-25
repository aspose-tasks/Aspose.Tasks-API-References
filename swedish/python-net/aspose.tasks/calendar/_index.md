---
title: "Calendar"
second_title: "Aspose.Tasks för Python via .NET API-referens"
description: 
type: docs
weight: 140
url: /sv/python-net/aspose.tasks/calendar/
---

## Calendar class

Representerar en kalender som används i ett projekt.

Typen Calendar visar följande medlemmar:
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| name | Hämtar eller anger kalenderns namn. |
| uid | Hämtar eller anger kalenderns unika identifierare. |
| week_days | Hämtar WeekDaysCollection för denna kalender.<br/>            Samlingen av veckodagar som definierar kalendern. |
| exceptions | Hämtar CalendarExceptionCollection-objekt.<br/>            Samlingen av undantag som är associerade med kalendern. |
| work_weeks | Hämtar WorkWeekCollections-objekt.<br/>            Samlingen av arbetsveckor som är associerade med kalendern. |
| is_base_calendar | Hämtar ett värde som indikerar om kalendern är en grundkalender. |
| base_calendar | Hämtar eller anger grundkalendern som denna kalender är beroende av.<br/>            Endast tillämpligt om kalendern inte är en grundkalender. |
| is_baseline_calendar | Hämtar eller anger ett värde som indikerar om kalendern är en baslinjekalender. |
| guid | Hämtar kalenderns Guid. |
| primavera_properties | Hämtar ett objekt som innehåller Primavera-specifika egenskaper för en kalender läst från Primavera-format. |
## Methods
| Namn | Beskrivning |
| :- | :- |
| get_start_date_from_finish_and_duration(finish, duration) | Returnerar startdatum baserat på det specificerade slutdatumet och varaktigheten. |
| get_start_date_from_finish_and_duration(finish, duration) | Returnerar startdatum baserat på specificerat slutdatum och varaktighet. |
| get_working_hours(start, finish) | Returnera WorkUnit - Start, Slut och Varaktighet för arbetstimmar för det angivna datum-tidsintervallet. |
| get_working_hours(dt) | Returnera WorkUnit - Start, Slut och Varaktighet för arbetstimmar för det angivna datum-tidsintervallet. |
| get_finish_date_by_start_and_work(start, work) | Beräknar datumet då den angivna mängden arbetstid har passerat enligt kalendern. |
| get_finish_date_by_start_and_work(start, work) | Beräknar datumet då den angivna mängden arbetstid har passerat enligt kalendern. |
| get_intersection_calendar(calendar1, calendar2) | Hämtar [ICalendar](/tasks/python-net/aspose.tasks/icalendar/)-instans som kan användas för att utföra beräkningar på skärningspunkten av arbetsscheman för 2 kalendrar. |
| make_standard_calendar(calendar) | Skapar standardkalender som standard. |
| make_24_hour_calendar(calendar) | Gör en given kalender till en 24‑timmarskalender.<br/>            24‑timmarskalender är en kalender där varje veckodag arbetar med dygnet‑runt arbetstid. |
| make_night_shift_calendar(calendar) | Gör en given kalender till en nattskiftkalender. |
| delete() | Tar bort kalender från projektet. |
| is_day_working(dt) | Bestämmer om den angivna dagen är en arbetsdag enligt kalendern. |
| get_working_hours_time_span(start, finish) | Returnerar mängden arbetstimmar mellan de angivna datumen. |
| get_task_finish_date_from_duration(task, duration) | Beräknar uppgiftens slutdatum och tid utifrån dess startdatum, delade delar och arbetstidslängden. |
| get_working_times(dt) | Returnerar [WorkingTimeCollection](/tasks/python-net/aspose.tasks/workingtimecollection/) med arbetstider för det angivna datumet. |
| get_previous_working_day_end(date) | Beräknar slutet på föregående arbetsdag utifrån det angivna datumet. |
| get_next_working_day_start(date) | Beräknar nästa arbetsdags start för det angivna datumet. |
| get_work_start(date) | Beräknar nästa arbetstids start med början från det angivna datumet och tiden. |
| is_empty() | Returnerar om kalendern inte har definierade arbetstimmar. |

### Se även

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

