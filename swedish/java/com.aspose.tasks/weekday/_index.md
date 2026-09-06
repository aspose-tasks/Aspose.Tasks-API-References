---
title: "WeekDay"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en veckodag som antingen definierar vanliga dagar i en vecka eller undantagsdagar i en kalender."
type: docs
weight: 352
url: /sv/java/com.aspose.tasks/weekday/
---

**Inheritance:**
java.lang.Object
```
public class WeekDay
```

Representerar en veckodag som antingen definierar vanliga dagar i en vecka eller undantagsdagar i en kalender.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [WeekDay(int dayType)](#WeekDay-int-) | Initierar en ny instans av klassen [WeekDay](../../com.aspose.tasks/weekday) med den angivna dagtypen. |
| [WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes)](#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--) | Initierar en ny instans av klassen [WeekDay](../../com.aspose.tasks/weekday) med den angivna dagtypen och en lista över arbetstidsperioder. |
| [WeekDay(int dayType, WorkingTime[] workingTimes)](#WeekDay-int-com.aspose.tasks.WorkingTime...-) | Initierar en ny instans av klassen [WeekDay](../../com.aspose.tasks/weekday) med den angivna dagtypen och arbetstidsperioder. |
| [WeekDay()](#WeekDay--) | Initierar en ny instans av klassen [WeekDay](../../com.aspose.tasks/weekday). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [castToDayType(int dw)](#castToDayType-int-) | Kastar .Net:s [DayOfWeek](../../com.aspose.tasks/dayofweek) till `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)). |
| [createDefaultWorkingDay(int dayType)](#createDefaultWorkingDay-int-) | Skapar standardarbetsdag. |
| [deepClone()](#deepClone--) | Returnerar en djup kopia av veckodagen. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt. |
| [getDayType()](#getDayType--) | Hämtar typen av en dag. |
| [getDayWorking()](#getDayWorking--) | Hämtar ett värde som indikerar om det angivna datumet eller dagtypen är arbetsdag. |
| [getFromDate()](#getFromDate--) | Hämtar början av en undantagstid. |
| [getToDate()](#getToDate--) | Hämtar slutet av en undantagstid. |
| [getWorkingTime()](#getWorkingTime--) | Returnerar arbetstiden för en veckodag. |
| [getWorkingTimes()](#getWorkingTimes--) | Hämtar WorkingTimeCollection för denna WeekDay-instans. |
| [hashCode()](#hashCode--) | Returnerar ett hashkodvärde för en instans av klassen [WeekDay](../../com.aspose.tasks/weekday). |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Ställer in ett värde som indikerar om det angivna datumet eller dagtypen är arbetsdag. |
| [setDefaultWorkingTime(WeekDay day)](#setDefaultWorkingTime-com.aspose.tasks.WeekDay-) | Ställer in standardtidsperioder för den angivna veckodagen. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | Ställer in början av en undantagstid. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | Ställer in slutet av en undantagstid. |
### WeekDay(int dayType) {#WeekDay-int-}
```
public WeekDay(int dayType)
```


Initierar en ny instans av klassen [WeekDay](../../com.aspose.tasks/weekday) med den angivna dagtypen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dayType | int | Den angivna dagtypen. |

### WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes) {#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--}
```
public WeekDay(int dayType, List<WorkingTime> workingTimes)
```


Initierar en ny instans av klassen [WeekDay](../../com.aspose.tasks/weekday) med den angivna dagtypen och en lista över arbetstidsperioder.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dayType | int | Den angivna dagtypen. |
| workingTimes | java.util.List&lt;com.aspose.tasks.WorkingTime&gt; | Lista över arbetsperioder. |

### WeekDay(int dayType, WorkingTime[] workingTimes) {#WeekDay-int-com.aspose.tasks.WorkingTime...-}
```
public WeekDay(int dayType, WorkingTime[] workingTimes)
```


Initierar en ny instans av klassen [WeekDay](../../com.aspose.tasks/weekday) med den angivna dagtypen och arbetstidsperioder.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dayType | int | Den angivna dagtypen. |
| workingTimes | [WorkingTime\[\]](../../com.aspose.tasks/workingtime) | Array av arbetsperioder. |

### WeekDay() {#WeekDay--}
```
public WeekDay()
```


Initierar en ny instans av klassen [WeekDay](../../com.aspose.tasks/weekday).

### castToDayType(int dw) {#castToDayType-int-}
```
public static int castToDayType(int dw)
```


Kastar .Net:s [DayOfWeek](../../com.aspose.tasks/dayofweek) till `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dw | int | Veckodagen att kasta från. |

**Returns:**
int - En kastad dagtyp.
### createDefaultWorkingDay(int dayType) {#createDefaultWorkingDay-int-}
```
public static WeekDay createDefaultWorkingDay(int dayType)
```


Skapar standardarbetsdag.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dayType | int | Dagtypen att skapa standardarbetsdag från. |

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - A default working day with working times 8-12 and 13-17.
### deepClone() {#deepClone--}
```
public final WeekDay deepClone()
```


Returnerar en djup kopia av veckodagen.

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - Returns the deep copy of the week day.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | Objektet att jämföra med denna instans. |

**Returns:**
boolean - **True** om det angivna objektet är en WeekDay som har samma FromDate-, ToDate-värden och WorkingTimes som detta objekt; annars, **false**.
### getDayType() {#getDayType--}
```
public final int getDayType()
```


Hämtar typen av en dag.

**Returns:**
int - typen av en dag.
### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Hämtar ett värde som indikerar om det angivna datumet eller dagtypen är arbetsdag.

**Returns:**
boolean - ett värde som indikerar om det angivna datumet eller dagtypen är arbetsdag.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


Hämtar början av en undantagstid.

**Returns:**
java.util.Date - början av en undantagstid.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


Hämtar slutet av en undantagstid.

**Returns:**
java.util.Date - slutet av en undantagstid.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Returnerar arbetstiden för en veckodag.

**Returns:**
double - Arbetstid.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


Hämtar WorkingTimeCollection för detta WeekDay-instans. Samlingen av arbetstider som definierar den tid som arbetas på veckodagen.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - WorkingTimeCollection for this WeekDay instance.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returnerar ett hashkodvärde för en instans av klassen [WeekDay](../../com.aspose.tasks/weekday).

**Returns:**
int - returnerar ett hash‑kodvärde för detta objekt.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Ställer in ett värde som indikerar om det angivna datumet eller dagtypen är arbetsdag.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om det angivna datumet eller dagtypen är arbetsdag. |

### setDefaultWorkingTime(WeekDay day) {#setDefaultWorkingTime-com.aspose.tasks.WeekDay-}
```
public static void setDefaultWorkingTime(WeekDay day)
```


Ställer in standardtidsperioder för den angivna veckodagen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| day | [WeekDay](../../com.aspose.tasks/weekday) | Veckodagen att ställa in standardarbetsdag på. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


Ställer in början av en undantagstid.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | början av en undantagstid. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


Ställer in slutet av en undantagstid.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | slutet av en undantagstid. |

