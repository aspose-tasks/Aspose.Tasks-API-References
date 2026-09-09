---
title: "CalendarException"
second_title: "Aspose.Tasks für Python via .NET API-Referenz"
description: 
type: docs
weight: 160
url: /de/python-net/aspose.tasks/calendarexception/
---

## CalendarException class

Stellt außergewöhnliche Zeiträume in einem Kalender dar.

Der Typ CalendarException stellt die folgenden Mitglieder bereit:
## Konstruktoren
| Name | Beschreibung |
| :- | :- |
| CalendarException() | Initialisiert eine neue Instanz der Klasse [CalendarException](/tasks/python-net/aspose.tasks/calendarexception/). |
## Eigenschaften
| Name | Beschreibung |
| :- | :- |
| entered_by_occurrences | Liest oder setzt einen Wert, der angibt, ob der Wiederholungsbereich durch Eingabe einer Anzahl von Vorkommnissen definiert ist.<br/>            False gibt an, dass der Wiederholungsbereich durch Eingabe eines Enddatums definiert ist. |
| from_date | Liest oder setzt den Beginn der Ausnahmezeit. |
| to_date | Liest oder setzt das Ende der Ausnahmezeit. |
| Vorkommen | Liest oder setzt die Anzahl der Vorkommnisse, für die die Kalenderausnahme gültig ist. |
| name | Liest oder setzt den Namen der Ausnahme. |
| Typ | Liest oder setzt den Ausnahmetyp. |
| period | Liest oder setzt den Wiederholungszeitraum für die Ausnahme. |
| days_of_week | Liest die DayTypeCollection für dieses Objekt.<br/>            Die Wochentage, an denen die Ausnahme gültig ist. |
| month_item | Liest oder setzt das Monatselement, für das eine Ausnahmewiederholung geplant ist. |
| month_position | Liest oder setzt die Position eines Monatselements innerhalb eines Monats. |
| Monat | Liest oder setzt den Monat, für den eine Ausnahmewiederholung geplant ist. |
| month_day | Liest oder setzt den Tag eines Monats, an dem eine Ausnahmewiederholung geplant ist. |
| day_working | Liest oder setzt einen Wert, der angibt, ob das angegebene Datum oder der Tagtyp ein Arbeitstag ist. |
| working_times | Liest oder setzt das WorkingTimeCollection-Objekt.<br/>            Die Sammlung von Arbeitszeiten, die die an einem Wochentag gearbeitete Zeit definiert. |
| parent_calendar | Liefert den übergeordneten Kalender für dieses Objekt. |
## Methoden
| Name | Beschreibung |
| :- | :- |
| delete() | Löscht die Exception-Instanz aus dem übergeordneten Kalenderobjekt CalendarExceptionCollection. |
| check_exception(dt) | Gibt true zurück, wenn die angegebene Instanz der datetime-Struktur der Ausnahmetag ist. |
| get_working_time() | Gibt die Arbeitszeit für eine Kalenderausnahme zurück. |
| get_exception_dates() | Gibt die Daten zurück, an denen die Kalenderausnahme gilt. |

### Siehe auch

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

