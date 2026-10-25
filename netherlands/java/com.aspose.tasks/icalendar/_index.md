---
title: "ICalendar"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een kalenderabstractie voor die kan worden gebruikt voor verschillende berekeningen van datums en duur."
type: docs
weight: 376
url: /nl/java/com.aspose.tasks/icalendar/
---
```
public interface ICalendar
```

Stelt een kalenderabstractie voor die kan worden gebruikt voor verschillende berekeningen van datums en duur.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getFinishDateByStartAndWork(Date start, Duration work)](#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-) | Berekent de datum waarop de opgegeven hoeveelheid werktijd volgens de kalender is verstreken. |
| [getFinishDateByStartAndWork(Date start, double work)](#getFinishDateByStartAndWork-java.util.Date-double-) | Berekent de datum waarop de opgegeven hoeveelheid werktijd volgens de kalender is verstreken. |
| [getNextWorkingDayStart(Date date)](#getNextWorkingDayStart-java.util.Date-) | Berekent de start van de volgende werkdag voor de opgegeven datum. |
| [getPreviousWorkingDayEnd(Date date)](#getPreviousWorkingDayEnd-java.util.Date-) | Berekent het einde van de vorige werkdag vanaf de opgegeven datum. |
| [getStartDateFromFinishAndDuration(Date finish, Duration duration)](#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-) | Geeft de startdatum terug op basis van de opgegeven einddatum en duur. |
| [getStartDateFromFinishAndDuration(Date finish, double duration)](#getStartDateFromFinishAndDuration-java.util.Date-double-) | Geeft de startdatum terug op basis van de opgegeven einddatum en duur. |
| [getTaskFinishDateFromDuration(Task task, double duration)](#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-) | Berekent de einddatum en -tijd van de taak op basis van de startdatum, gesplitste delen en de werktijdduur. |
| [getWorkStart(Date date)](#getWorkStart-java.util.Date-) | Berekent de start van de volgende werktijd beginnend vanaf de opgegeven datum en tijd. |
| [getWorkingHours(Date dt)](#getWorkingHours-java.util.Date-) | Geeft het aantal werkuren op de opgegeven datum terug. |
| [getWorkingHours(Date start, Date finish)](#getWorkingHours-java.util.Date-java.util.Date-) | Retourneer WorkUnit - Start, Eind en Duur van werkuren voor het opgegeven datum‑tijdinterval. |
| [getWorkingHoursTimeSpan(Date start, Date finish)](#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-) | Geeft het aantal werkuren tussen de opgegeven data terug. |
| [getWorkingTimes(Date dt)](#getWorkingTimes-java.util.Date-) | Geeft [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) van werktijden voor de opgegeven datum terug. |
| [isDayWorking(Date dt)](#isDayWorking-java.util.Date-) | Bepaalt of de opgegeven dag een werkdag is volgens de kalender. |
| [isEmpty()](#isEmpty--) | Geeft terug of de kalender geen werkuren heeft gedefinieerd. |
### getFinishDateByStartAndWork(Date start, Duration work) {#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getFinishDateByStartAndWork(Date start, Duration work)
```


Berekent de datum waarop de opgegeven hoeveelheid werktijd volgens de kalender is verstreken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | java.util.Date | Startdatum. |
| work | [Duration](../../com.aspose.tasks/duration) | Werkduur. |

**Returns:**
java.util.Date - Einddatum.
### getFinishDateByStartAndWork(Date start, double work) {#getFinishDateByStartAndWork-java.util.Date-double-}
```
public abstract Date getFinishDateByStartAndWork(Date start, double work)
```


Berekent de datum waarop de opgegeven hoeveelheid werktijd volgens de kalender is verstreken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | java.util.Date | Startdatum. |
| werk | double | Werkduur. |

**Returns:**
java.util.Date - Einddatum.
### getNextWorkingDayStart(Date date) {#getNextWorkingDayStart-java.util.Date-}
```
public abstract Date getNextWorkingDayStart(Date date)
```


Berekent de start van de volgende werkdag voor de opgegeven datum.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| datum | java.util.Date | De datum om de start van de volgende werkdag te verkrijgen. |

**Returns:**
java.util.Date - Start van de volgende werkdag System.DateTime.
### getPreviousWorkingDayEnd(Date date) {#getPreviousWorkingDayEnd-java.util.Date-}
```
public abstract Date getPreviousWorkingDayEnd(Date date)
```


Berekent het einde van de vorige werkdag vanaf de opgegeven datum.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| datum | java.util.Date | de datum om het einde van de vorige werkdag te berekenen. |

**Returns:**
java.util.Date - Het einde van de vorige werkdag.
### getStartDateFromFinishAndDuration(Date finish, Duration duration) {#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, Duration duration)
```


Geeft de startdatum terug op basis van de opgegeven einddatum en duur.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| einde | java.util.Date | De opgegeven einddatum. |
| duration | [Duration](../../com.aspose.tasks/duration) | De opgegeven duur. |

**Returns:**
java.util.Date - Berekende startdatum.
### getStartDateFromFinishAndDuration(Date finish, double duration) {#getStartDateFromFinishAndDuration-java.util.Date-double-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, double duration)
```


Geeft de startdatum terug op basis van de opgegeven einddatum en duur.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| einde | java.util.Date | De opgegeven einddatum. |
| duur | double | De opgegeven duur. |

**Returns:**
java.util.Date - Berekende startdatum.
### getTaskFinishDateFromDuration(Task task, double duration) {#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-}
```
public abstract Date getTaskFinishDateFromDuration(Task task, double duration)
```


Berekent de einddatum en -tijd van de taak op basis van de startdatum, gesplitste delen en de werktijdduur.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | De taak waarvoor de einddatum moet worden berekend. |
|  | duur | double | De te berekenen duur. |

Retourneert DateTime.MinValue als de taak een samenvatting is, null of als de startdatum niet is ingesteld. |

**Returns:**
java.util.Date - Einddatum van de taak voor de gegeven startdatum en duur.
### getWorkStart(Date date) {#getWorkStart-java.util.Date-}
```
public abstract Date getWorkStart(Date date)
```


Berekent de start van de volgende werktijd beginnend vanaf de opgegeven datum en tijd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| datum | java.util.Date | De datum en tijd. |

**Returns:**
java.util.Date - De dichtstbijzijnde start van werktijd.
### getWorkingHours(Date dt) {#getWorkingHours-java.util.Date-}
```
public abstract double getWorkingHours(Date dt)
```


Geeft het aantal werkuren op de opgegeven datum terug.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dt | java.util.Date | De datum om de werkuren te verkrijgen. |

**Returns:**
double - Werkuren op de opgegeven datum.
### getWorkingHours(Date start, Date finish) {#getWorkingHours-java.util.Date-java.util.Date-}
```
public abstract WorkUnit getWorkingHours(Date start, Date finish)
```


Retourneer WorkUnit - Start, Eind en Duur van werkuren voor het opgegeven datum‑tijdinterval.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | java.util.Date | Startdatum van het interval. |
| einde | java.util.Date | Einddatum van het interval. |

**Returns:**
[WorkUnit](../../com.aspose.tasks/workunit) - Instance of [WorkUnit](../../com.aspose.tasks/workunit) class containing Start, Finish and Duration of working hours.
### getWorkingHoursTimeSpan(Date start, Date finish) {#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-}
```
public abstract double getWorkingHoursTimeSpan(Date start, Date finish)
```


Geeft het aantal werkuren tussen de opgegeven data terug.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | java.util.Date | Startdatum van het interval. |
| einde | java.util.Date | Einddatum van het interval. |

**Returns:**
double - Aantal werkuren volgens de kalenderinstantie.
### getWorkingTimes(Date dt) {#getWorkingTimes-java.util.Date-}
```
public abstract WorkingTimeCollection getWorkingTimes(Date dt)
```


Geeft [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) van werktijden voor de opgegeven datum terug.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dt | java.util.Date | De datum om de werktijden te verkrijgen. |

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - Collection of [WorkingTime](../../com.aspose.tasks/workingtime) instances.
### isDayWorking(Date dt) {#isDayWorking-java.util.Date-}
```
public abstract boolean isDayWorking(Date dt)
```


Bepaalt of de opgegeven dag een werkdag is volgens de kalender.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dt | java.util.Date | De datum om te controleren of de dag een werkdag is. |

**Returns:**
boolean - Waar als de dag een werkdag is.
### isEmpty() {#isEmpty--}
```
public abstract boolean isEmpty()
```


Geeft terug of de kalender geen werkuren heeft gedefinieerd.

**Returns:**
boolean - Waar als de agenda geen werkuren heeft gedefinieerd.
