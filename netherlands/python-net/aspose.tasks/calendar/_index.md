---
title: "Calendar"
second_title: "Aspose.Tasks for Python via .NET API-referentie"
description: 
type: docs
weight: 140
url: /nl/python-net/aspose.tasks/calendar/
---

## Calendar class

Stelt een kalender voor die in een project wordt gebruikt.

Het type Calendar bevat de volgende leden:
## Eigenschappen
| Naam | Beschrijving |
| :- | :- |
| name | Krijgt of stelt de naam van de agenda in. |
| uid | Haalt op of stelt de unieke identifier van de agenda in. |
| week_days | Haalt WeekDaysCollection op voor deze agenda.<br/>            De verzameling weekdagen die de agenda definieert. |
| exceptions | Haalt CalendarExceptionCollection-object op.<br/>            De verzameling uitzonderingen die aan de agenda zijn gekoppeld. |
| work_weeks | Haalt WorkWeekCollections-object op.<br/>            De verzameling werkweken die aan de agenda zijn gekoppeld. |
| is_base_calendar | Haalt een waarde op die aangeeft of de agenda een basisagenda is. |
| base_calendar | Haalt op of stelt de basisagenda in waarop deze agenda afhankelijk is.<br/>            Alleen van toepassing als de agenda geen basisagenda is. |
| is_baseline_calendar | Haalt op of stelt een waarde in die aangeeft of de agenda een baseline-agenda is. |
| guid | Haalt de Guid van de agenda op. |
| primavera_properties | Haalt een object op dat Primavera-specifieke eigenschappen bevat voor een agenda die uit Primavera-formaten is gelezen. |
## Methods
| Naam | Beschrijving |
| :- | :- |
| get_start_date_from_finish_and_duration(finish, duration) | Retourneert de startdatum op basis van de opgegeven einddatum en duur. |
| get_start_date_from_finish_and_duration(finish, duration) | Retourneert de startdatum op basis van de opgegeven einddatum en duur. |
| get_working_hours(start, finish) | Retourneer WorkUnit - Start, Eind en Duur van werktijd voor het opgegeven datum‑tijdinterval. |
| get_working_hours(dt) | Retourneer WorkUnit - Start, Eind en Duur van werktijd voor het opgegeven datum‑tijdinterval. |
| get_finish_date_by_start_and_work(start, work) | Berekent de datum waarop de opgegeven hoeveelheid werktijd volgens de kalender zal verstrijken. |
| get_finish_date_by_start_and_work(start, work) | Berekent de datum waarop de opgegeven hoeveelheid werktijd volgens de kalender zal verstrijken. |
| get_intersection_calendar(calendar1, calendar2) | Haalt een [ICalendar](/tasks/python-net/aspose.tasks/icalendar/)‑instantie op die kan worden gebruikt om berekeningen uit te voeren op de intersectie van werkschema's van 2 agenda's. |
| make_standard_calendar(calendar) | Maakt een standaard agenda aan. |
| make_24_hour_calendar(calendar) | Maakt een opgegeven Agenda tot een 24‑uur agenda.<br/>            Een 24‑uur agenda is een agenda waarin elke dag van de week werkt met doorlopende werktijden. |
| make_night_shift_calendar(calendar) | Maakt een opgegeven Agenda tot een nachtdienstagenda. |
| delete() | Verwijdert agenda uit het project. |
| is_day_working(dt) | Bepaalt of de opgegeven dag een werkdag is volgens de kalender. |
| get_working_hours_time_span(start, finish) | Retourneert de hoeveelheid werkuren tussen de opgegeven data. |
| get_task_finish_date_from_duration(task, duration) | Berekent de einddatum en -tijd van de taak op basis van de startdatum, gesplitste delen en de werktijd. |
| get_working_times(dt) | Retourneert een [WorkingTimeCollection](/tasks/python-net/aspose.tasks/workingtimecollection/) met werktijden voor de opgegeven datum. |
| get_previous_working_day_end(date) | Berekent het einde van de vorige werkdag op basis van de opgegeven datum. |
| get_next_working_day_start(date) | Berekent het begin van de volgende werkdag voor de opgegeven datum. |
| get_work_start(date) | Berekent het begin van de volgende werktijd vanaf de opgegeven datum en tijd. |
| is_empty() | Retourneert of de kalender geen gedefinieerde werkuren heeft. |

### Zie ook

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

