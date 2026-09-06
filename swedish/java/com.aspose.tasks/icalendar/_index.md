---
title: "ICalendar"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en kalenderabstraktion som kan användas för olika beräkningar av datum och varaktigheter."
type: docs
weight: 376
url: /sv/java/com.aspose.tasks/icalendar/
---
```
public interface ICalendar
```

Representerar en kalenderabstraktion som kan användas för olika beräkningar av datum och varaktigheter.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getFinishDateByStartAndWork(Date start, Duration work)](#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-) | Beräknar datumet då den angivna mängden arbetstid har passerat enligt kalendern. |
| [getFinishDateByStartAndWork(Date start, double work)](#getFinishDateByStartAndWork-java.util.Date-double-) | Beräknar datumet då den angivna mängden arbetstid har passerat enligt kalendern. |
| [getNextWorkingDayStart(Date date)](#getNextWorkingDayStart-java.util.Date-) | Beräknar nästa arbetsdags start för det angivna datumet. |
| [getPreviousWorkingDayEnd(Date date)](#getPreviousWorkingDayEnd-java.util.Date-) | Beräknar slutet på föregående arbetsdag utifrån det angivna datumet. |
| [getStartDateFromFinishAndDuration(Date finish, Duration duration)](#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-) | Returnerar startdatum baserat på angivet slutdatum och varaktighet. |
| [getStartDateFromFinishAndDuration(Date finish, double duration)](#getStartDateFromFinishAndDuration-java.util.Date-double-) | Returnerar startdatum baserat på angivet slutdatum och varaktighet. |
| [getTaskFinishDateFromDuration(Task task, double duration)](#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-) | Beräknar uppgiftens slutdatum och -tid från dess startdatum, delade delar och arbetstiden. |
| [getWorkStart(Date date)](#getWorkStart-java.util.Date-) | Beräknar nästa arbetstids start med början från det angivna datumet och tiden. |
| [getWorkingHours(Date dt)](#getWorkingHours-java.util.Date-) | Returnerar antalet arbetstimmar på det angivna datumet. |
| [getWorkingHours(Date start, Date finish)](#getWorkingHours-java.util.Date-java.util.Date-) | Returnera WorkUnit - Start, Slut och Varaktighet för arbetstimmar för det angivna datum-tidsintervallet. |
| [getWorkingHoursTimeSpan(Date start, Date finish)](#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-) | Returnerar antalet arbetstimmar mellan de angivna datumen. |
| [getWorkingTimes(Date dt)](#getWorkingTimes-java.util.Date-) | Returnerar [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) med arbetstider för det angivna datumet. |
| [isDayWorking(Date dt)](#isDayWorking-java.util.Date-) | Avgör om den angivna dagen är en arbetsdag enligt kalendern. |
| [isEmpty()](#isEmpty--) | Returnerar om kalendern inte har definierade arbetstimmar. |
### getFinishDateByStartAndWork(Date start, Duration work) {#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getFinishDateByStartAndWork(Date start, Duration work)
```


Beräknar datumet då den angivna mängden arbetstid har passerat enligt kalendern.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| start | java.util.Date | Startdatum. |
| work | [Duration](../../com.aspose.tasks/duration) | Arbetstid. |

**Returns:**
java.util.Date - Slutdatum.
### getFinishDateByStartAndWork(Date start, double work) {#getFinishDateByStartAndWork-java.util.Date-double-}
```
public abstract Date getFinishDateByStartAndWork(Date start, double work)
```


Beräknar datumet då den angivna mängden arbetstid har passerat enligt kalendern.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| start | java.util.Date | Startdatum. |
| arbete | double | Arbetstid. |

**Returns:**
java.util.Date - Slutdatum.
### getNextWorkingDayStart(Date date) {#getNextWorkingDayStart-java.util.Date-}
```
public abstract Date getNextWorkingDayStart(Date date)
```


Beräknar nästa arbetsdags start för det angivna datumet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| datum | java.util.Date | Datumet för att hämta nästa arbetsdagens start. |

**Returns:**
java.util.Date - Nästa arbetsdagens start System.DateTime.
### getPreviousWorkingDayEnd(Date date) {#getPreviousWorkingDayEnd-java.util.Date-}
```
public abstract Date getPreviousWorkingDayEnd(Date date)
```


Beräknar slutet på föregående arbetsdag utifrån det angivna datumet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| datum | java.util.Date | Datumet för att beräkna föregående arbetsdagens slut. |

**Returns:**
java.util.Date - Slutet på föregående arbetsdag
### getStartDateFromFinishAndDuration(Date finish, Duration duration) {#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, Duration duration)
```


Returnerar startdatum baserat på angivet slutdatum och varaktighet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| slut | java.util.Date | Det angivna slutdatumet. |
| duration | [Duration](../../com.aspose.tasks/duration) | Den angivna varaktigheten. |

**Returns:**
java.util.Date - Beräknat startdatum.
### getStartDateFromFinishAndDuration(Date finish, double duration) {#getStartDateFromFinishAndDuration-java.util.Date-double-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, double duration)
```


Returnerar startdatum baserat på angivet slutdatum och varaktighet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| slut | java.util.Date | Det angivna slutdatumet. |
| varaktighet | double | Den angivna varaktigheten. |

**Returns:**
java.util.Date - Beräknat startdatum.
### getTaskFinishDateFromDuration(Task task, double duration) {#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-}
```
public abstract Date getTaskFinishDateFromDuration(Task task, double duration)
```


Beräknar uppgiftens slutdatum och -tid från dess startdatum, delade delar och arbetstiden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Uppgiften för att beräkna slutdatum. |
|  | varaktighet | double | Varaktigheten att beräkna. |

Returnerar DateTime.MinValue om uppgiften är en sammanfattning, null eller om dess startdatum inte är angivet. |

**Returns:**
java.util.Date - Uppgiftens slutdatum för det givna startdatumet och varaktigheten.
### getWorkStart(Date date) {#getWorkStart-java.util.Date-}
```
public abstract Date getWorkStart(Date date)
```


Beräknar nästa arbetstids start med början från det angivna datumet och tiden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| datum | java.util.Date | Datumet och tiden. |

**Returns:**
java.util.Date - Närmaste arbetstidens start.
### getWorkingHours(Date dt) {#getWorkingHours-java.util.Date-}
```
public abstract double getWorkingHours(Date dt)
```


Returnerar antalet arbetstimmar på det angivna datumet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dt | java.util.Date | Datumet för att hämta arbetstimmar för. |

**Returns:**
double - Arbetstimmar på det angivna datumet.
### getWorkingHours(Date start, Date finish) {#getWorkingHours-java.util.Date-java.util.Date-}
```
public abstract WorkUnit getWorkingHours(Date start, Date finish)
```


Returnera WorkUnit - Start, Slut och Varaktighet för arbetstimmar för det angivna datum-tidsintervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| start | java.util.Date | Startdatum för intervallet. |
| slut | java.util.Date | Slutdatum för intervallet. |

**Returns:**
[WorkUnit](../../com.aspose.tasks/workunit) - Instance of [WorkUnit](../../com.aspose.tasks/workunit) class containing Start, Finish and Duration of working hours.
### getWorkingHoursTimeSpan(Date start, Date finish) {#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-}
```
public abstract double getWorkingHoursTimeSpan(Date start, Date finish)
```


Returnerar antalet arbetstimmar mellan de angivna datumen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| start | java.util.Date | Startdatum för intervallet. |
| slut | java.util.Date | Slutdatum för intervallet. |

**Returns:**
double - Antal arbetstimmar enligt kalenderinstansen.
### getWorkingTimes(Date dt) {#getWorkingTimes-java.util.Date-}
```
public abstract WorkingTimeCollection getWorkingTimes(Date dt)
```


Returnerar [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) med arbetstider för det angivna datumet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dt | java.util.Date | Datumet för att hämta arbetstider för. |

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - Collection of [WorkingTime](../../com.aspose.tasks/workingtime) instances.
### isDayWorking(Date dt) {#isDayWorking-java.util.Date-}
```
public abstract boolean isDayWorking(Date dt)
```


Avgör om den angivna dagen är en arbetsdag enligt kalendern.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dt | java.util.Date | Datumet för att kontrollera om dagen är en arbetsdag. |

**Returns:**
boolean - Sant om dagen är en arbetsdag.
### isEmpty() {#isEmpty--}
```
public abstract boolean isEmpty()
```


Returnerar om kalendern inte har definierade arbetstimmar.

**Returns:**
boolean - Sant om kalendern inte har definierade arbetstimmar.
