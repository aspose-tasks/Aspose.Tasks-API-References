---
title: "ICalendar"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Kalenderabstraktion dar, die für verschiedene Berechnungen von Daten und Zeitspannen verwendet werden kann."
type: docs
weight: 376
url: /de/java/com.aspose.tasks/icalendar/
---
```
public interface ICalendar
```

Stellt eine Kalenderabstraktion dar, die für verschiedene Berechnungen von Daten und Zeitspannen verwendet werden kann.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getFinishDateByStartAndWork(Date start, Duration work)](#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-) | Berechnet das Datum, an dem die angegebene Arbeitszeit laut Kalender verstrichen ist. |
| [getFinishDateByStartAndWork(Date start, double work)](#getFinishDateByStartAndWork-java.util.Date-double-) | Berechnet das Datum, an dem die angegebene Arbeitszeit laut Kalender verstrichen ist. |
| [getNextWorkingDayStart(Date date)](#getNextWorkingDayStart-java.util.Date-) | Berechnet den Beginn des nächsten Arbeitstages für das angegebene Datum. |
| [getPreviousWorkingDayEnd(Date date)](#getPreviousWorkingDayEnd-java.util.Date-) | Berechnet das Ende des vorherigen Arbeitstages vom angegebenen Datum. |
| [getStartDateFromFinishAndDuration(Date finish, Duration duration)](#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-) | Gibt das Startdatum basierend auf dem angegebenen Enddatum und der Dauer zurück. |
| [getStartDateFromFinishAndDuration(Date finish, double duration)](#getStartDateFromFinishAndDuration-java.util.Date-double-) | Gibt das Startdatum basierend auf dem angegebenen Enddatum und der Dauer zurück. |
| [getTaskFinishDateFromDuration(Task task, double duration)](#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-) | Berechnet das Fertigstellungsdatum und die -zeit einer Aufgabe aus ihrem Startdatum, den Teilabschnitten und der Arbeitsdauer. |
| [getWorkStart(Date date)](#getWorkStart-java.util.Date-) | Berechnet den Beginn der nächsten Arbeitszeit ab dem angegebenen Datum und der Uhrzeit. |
| [getWorkingHours(Date dt)](#getWorkingHours-java.util.Date-) | Gibt die Menge an Arbeitsstunden am angegebenen Datum zurück. |
| [getWorkingHours(Date start, Date finish)](#getWorkingHours-java.util.Date-java.util.Date-) | Gibt WorkUnit – Start, Ende und Dauer der Arbeitsstunden für das angegebene Datum‑Zeit‑Intervall zurück. |
| [getWorkingHoursTimeSpan(Date start, Date finish)](#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-) | Gibt die Menge an Arbeitsstunden zwischen den angegebenen Daten zurück. |
| [getWorkingTimes(Date dt)](#getWorkingTimes-java.util.Date-) | Gibt [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) der Arbeitszeiten für das angegebene Datum zurück. |
| [isDayWorking(Date dt)](#isDayWorking-java.util.Date-) | Bestimmt, ob der angegebene Tag ein Arbeitstag laut Kalender ist. |
| [isEmpty()](#isEmpty--) | Gibt zurück, ob im Kalender keine Arbeitszeiten definiert sind. |
### getFinishDateByStartAndWork(Date start, Duration work) {#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getFinishDateByStartAndWork(Date start, Duration work)
```


Berechnet das Datum, an dem die angegebene Arbeitszeit laut Kalender verstrichen ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| start | java.util.Date | Startdatum. |
| work | [Duration](../../com.aspose.tasks/duration) | Arbeitsdauer. |

**Returns:**
java.util.Date - Enddatum.
### getFinishDateByStartAndWork(Date start, double work) {#getFinishDateByStartAndWork-java.util.Date-double-}
```
public abstract Date getFinishDateByStartAndWork(Date start, double work)
```


Berechnet das Datum, an dem die angegebene Arbeitszeit laut Kalender verstrichen ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| start | java.util.Date | Startdatum. |
| Arbeit | double | Arbeitsdauer. |

**Returns:**
java.util.Date - Enddatum.
### getNextWorkingDayStart(Date date) {#getNextWorkingDayStart-java.util.Date-}
```
public abstract Date getNextWorkingDayStart(Date date)
```


Berechnet den Beginn des nächsten Arbeitstages für das angegebene Datum.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datum | java.util.Date | Das Datum, für das der Beginn des nächsten Arbeitstages ermittelt werden soll. |

**Returns:**
java.util.Date - Start des nächsten Arbeitstages System.DateTime.
### getPreviousWorkingDayEnd(Date date) {#getPreviousWorkingDayEnd-java.util.Date-}
```
public abstract Date getPreviousWorkingDayEnd(Date date)
```


Berechnet das Ende des vorherigen Arbeitstages vom angegebenen Datum.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datum | java.util.Date | Das Datum, um das Ende des vorherigen Arbeitstages zu berechnen. |

**Returns:**
java.util.Date - Das Ende des vorherigen Arbeitstages
### getStartDateFromFinishAndDuration(Date finish, Duration duration) {#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, Duration duration)
```


Gibt das Startdatum basierend auf dem angegebenen Enddatum und der Dauer zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschluss | java.util.Date | Das angegebene Enddatum. |
| duration | [Duration](../../com.aspose.tasks/duration) | Die angegebene Dauer. |

**Returns:**
java.util.Date - Berechnetes Startdatum.
### getStartDateFromFinishAndDuration(Date finish, double duration) {#getStartDateFromFinishAndDuration-java.util.Date-double-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, double duration)
```


Gibt das Startdatum basierend auf dem angegebenen Enddatum und der Dauer zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschluss | java.util.Date | Das angegebene Enddatum. |
| Dauer | double | Die angegebene Dauer. |

**Returns:**
java.util.Date - Berechnetes Startdatum.
### getTaskFinishDateFromDuration(Task task, double duration) {#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-}
```
public abstract Date getTaskFinishDateFromDuration(Task task, double duration)
```


Berechnet das Fertigstellungsdatum und die -zeit einer Aufgabe aus ihrem Startdatum, den Teilabschnitten und der Arbeitsdauer.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Die Aufgabe, für die das Enddatum berechnet werden soll. |
|  | Dauer | double | Die zu berechnende Dauer. |

Gibt DateTime.MinValue zurück, wenn die Aufgabe eine Zusammenfassung ist, null ist oder ihr Startdatum nicht gesetzt ist. |

**Returns:**
java.util.Date - Enddatum der Aufgabe für das gegebene Startdatum und die Dauer.
### getWorkStart(Date date) {#getWorkStart-java.util.Date-}
```
public abstract Date getWorkStart(Date date)
```


Berechnet den Beginn der nächsten Arbeitszeit ab dem angegebenen Datum und der Uhrzeit.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datum | java.util.Date | Datum und Uhrzeit. |

**Returns:**
java.util.Date - Der nächstgelegene Arbeitszeitbeginn.
### getWorkingHours(Date dt) {#getWorkingHours-java.util.Date-}
```
public abstract double getWorkingHours(Date dt)
```


Gibt die Menge an Arbeitsstunden am angegebenen Datum zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dt | java.util.Date | Das Datum, für das die Arbeitsstunden ermittelt werden sollen. |

**Returns:**
double - Arbeitsstunden am angegebenen Datum.
### getWorkingHours(Date start, Date finish) {#getWorkingHours-java.util.Date-java.util.Date-}
```
public abstract WorkUnit getWorkingHours(Date start, Date finish)
```


Gibt WorkUnit – Start, Ende und Dauer der Arbeitsstunden für das angegebene Datum‑Zeit‑Intervall zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| start | java.util.Date | Startdatum des Intervalls. |
| Abschluss | java.util.Date | Enddatum des Intervalls. |

**Returns:**
[WorkUnit](../../com.aspose.tasks/workunit) - Instance of [WorkUnit](../../com.aspose.tasks/workunit) class containing Start, Finish and Duration of working hours.
### getWorkingHoursTimeSpan(Date start, Date finish) {#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-}
```
public abstract double getWorkingHoursTimeSpan(Date start, Date finish)
```


Gibt die Menge an Arbeitsstunden zwischen den angegebenen Daten zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| start | java.util.Date | Startdatum des Intervalls. |
| Abschluss | java.util.Date | Enddatum des Intervalls. |

**Returns:**
double - Menge an Arbeitsstunden gemäß der Kalenderinstanz.
### getWorkingTimes(Date dt) {#getWorkingTimes-java.util.Date-}
```
public abstract WorkingTimeCollection getWorkingTimes(Date dt)
```


Gibt [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) der Arbeitszeiten für das angegebene Datum zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dt | java.util.Date | Das Datum, für das die Arbeitszeiten ermittelt werden sollen. |

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - Collection of [WorkingTime](../../com.aspose.tasks/workingtime) instances.
### isDayWorking(Date dt) {#isDayWorking-java.util.Date-}
```
public abstract boolean isDayWorking(Date dt)
```


Bestimmt, ob der angegebene Tag ein Arbeitstag laut Kalender ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dt | java.util.Date | Das Datum, um zu prüfen, ob der Tag ein Arbeitstag ist. |

**Returns:**
boolean - Wahr, wenn der Tag ein Arbeitstag ist.
### isEmpty() {#isEmpty--}
```
public abstract boolean isEmpty()
```


Gibt zurück, ob im Kalender keine Arbeitszeiten definiert sind.

**Returns:**
boolean - Wahr, wenn der Kalender keine Arbeitszeiten definiert hat.
