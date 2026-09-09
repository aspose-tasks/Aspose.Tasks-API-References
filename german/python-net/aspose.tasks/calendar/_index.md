---
title: "Calendar"
second_title: "Aspose.Tasks für Python via .NET API-Referenz"
description: 
type: docs
weight: 140
url: /de/python-net/aspose.tasks/calendar/
---

## Calendar class

Stellt einen Kalender dar, der in einem Projekt verwendet wird.

Der Typ Calendar stellt die folgenden Mitglieder bereit:
## Eigenschaften
| Name | Beschreibung |
| :- | :- |
| name | Liest oder setzt den Namen des Kalenders. |
| uid | Liest oder setzt die eindeutige Kennung des Kalenders. |
| week_days | Liest WeekDaysCollection für diesen Kalender.<br/>            Die Sammlung von Wochentagen, die den Kalender definiert. |
| exceptions | Liest CalendarExceptionCollection-Objekt.<br/>            Die Sammlung von Ausnahmen, die dem Kalender zugeordnet ist. |
| work_weeks | Liest WorkWeekCollections-Objekt.<br/>            Die Sammlung von Arbeitswochen, die dem Kalender zugeordnet ist. |
| is_base_calendar | Liest einen Wert, der angibt, ob der Kalender ein Basiskalender ist. |
| base_calendar | Liest oder setzt den Basiskalender, von dem dieser Kalender abhängt.<br/>            Nur anwendbar, wenn der Kalender kein Basiskalender ist. |
| is_baseline_calendar | Liest oder setzt einen Wert, der angibt, ob der Kalender ein Basiskalender ist. |
| guid | Liest die GUID des Kalenders. |
| primavera_properties | Liest ein Objekt, das Primavera-spezifische Eigenschaften für einen aus Primavera-Formaten gelesenen Kalender enthält. |
## Methoden
| Name | Beschreibung |
| :- | :- |
| get_start_date_from_finish_and_duration(finish, duration) | Gibt das Startdatum basierend auf dem angegebenen Enddatum und der Dauer zurück. |
| get_start_date_from_finish_and_duration(finish, duration) | Gibt das Startdatum basierend auf dem angegebenen Enddatum und der Dauer zurück. |
| get_working_hours(start, finish) | Rückgabe WorkUnit - Start, Ende und Dauer der Arbeitsstunden für das angegebene Datum‑Zeitintervall. |
| get_working_hours(dt) | Rückgabe WorkUnit - Start, Ende und Dauer der Arbeitsstunden für das angegebene Datum‑Zeitintervall. |
| get_finish_date_by_start_and_work(start, work) | Berechnet das Datum, an dem die angegebene Arbeitszeit gemäß dem Kalender verstrichen ist. |
| get_finish_date_by_start_and_work(start, work) | Berechnet das Datum, an dem die angegebene Arbeitszeit gemäß dem Kalender verstrichen ist. |
| get_intersection_calendar(calendar1, calendar2) | Ruft die [ICalendar](/tasks/python-net/aspose.tasks/icalendar/) Instanz ab, die verwendet werden kann, um Berechnungen an der Schnittmenge von Arbeitsplänen zweier Kalender durchzuführen. |
| make_standard_calendar(calendar) | Erstellt den standardmäßigen Standardkalender. |
| make_24_hour_calendar(calendar) | Wandelt einen angegebenen Kalender in einen 24‑Stunden‑Kalender um.<br/>            Der 24‑Stunden‑Kalender ist ein Kalender, in dem jeder Wochentag mit Rund-um-die‑Uhr-Arbeitszeiten arbeitet. |
| make_night_shift_calendar(calendar) | Wandelt einen angegebenen Kalender in einen Nachtschicht‑Kalender um. |
| delete() | Entfernt den Kalender aus dem Projekt. |
| is_day_working(dt) | Bestimmt, ob der angegebene Tag ein Arbeitstag gemäß dem Kalender ist. |
| get_working_hours_time_span(start, finish) | Gibt die Menge an Arbeitsstunden zwischen den angegebenen Daten zurück. |
| get_task_finish_date_from_duration(task, duration) | Berechnet das Enddatum und die Endzeit der Aufgabe aus ihrem Startdatum, aufgeteilten Teilen und der Arbeitsdauer. |
| get_working_times(dt) | Gibt [WorkingTimeCollection](/tasks/python-net/aspose.tasks/workingtimecollection/) von Arbeitszeiten für das angegebene Datum zurück. |
| get_previous_working_day_end(date) | Berechnet das Ende des vorherigen Arbeitstages aus dem angegebenen Datum. |
| get_next_working_day_start(date) | Berechnet den Beginn des nächsten Arbeitstages für das angegebene Datum. |
| get_work_start(date) | Berechnet den Beginn der nächsten Arbeitszeit ab dem angegebenen Datum und Uhrzeit. |
| is_empty() | Gibt zurück, ob im Kalender keine Arbeitszeiten definiert sind. |

### Siehe auch

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

