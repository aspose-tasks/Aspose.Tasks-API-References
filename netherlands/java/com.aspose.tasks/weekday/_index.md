---
title: "WeekDay"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een weekdag voor die ofwel reguliere dagen van een week definieert of uitzonderingsdagen in een kalender."
type: docs
weight: 352
url: /nl/java/com.aspose.tasks/weekday/
---

**Inheritance:**
java.lang.Object
```
public class WeekDay
```

Stelt een weekdag voor die ofwel reguliere dagen van een week definieert of uitzonderingsdagen in een kalender.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [WeekDay(int dayType)](#WeekDay-int-) | Initialiseert een nieuw exemplaar van de [WeekDay](../../com.aspose.tasks/weekday) klasse met het opgegeven dagtype. |
| [WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes)](#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--) | Initialiseert een nieuw exemplaar van de [WeekDay](../../com.aspose.tasks/weekday) klasse met het opgegeven dagtype en een lijst van werkperioden. |
| [WeekDay(int dayType, WorkingTime[] workingTimes)](#WeekDay-int-com.aspose.tasks.WorkingTime...-) | Initialiseert een nieuw exemplaar van de [WeekDay](../../com.aspose.tasks/weekday) klasse met het opgegeven dagtype en werkperioden. |
| [WeekDay()](#WeekDay--) | Initialiseert een nieuw exemplaar van de [WeekDay](../../com.aspose.tasks/weekday) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [castToDayType(int dw)](#castToDayType-int-) | Cast .Net's [DayOfWeek](../../com.aspose.tasks/dayofweek) naar `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)). |
| [createDefaultWorkingDay(int dayType)](#createDefaultWorkingDay-int-) | Maakt een standaard werkdag aan. |
| [deepClone()](#deepClone--) | Retourneert een diepe kopie van de weekdag. |
| [equals(Object obj)](#equals-java.lang.Object-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [getDayType()](#getDayType--) | Haalt het type van een dag op. |
| [getDayWorking()](#getDayWorking--) | Haalt een waarde op die aangeeft of de opgegeven datum of dagtype werkend is. |
| [getFromDate()](#getFromDate--) | Haalt het begin van een uitzonderingstijd op. |
| [getToDate()](#getToDate--) | Haalt het einde van een uitzonderingstijd op. |
| [getWorkingTime()](#getWorkingTime--) | Retourneert de werktijd voor een weekdag. |
| [getWorkingTimes()](#getWorkingTimes--) | Haalt WorkingTimeCollection op voor dit WeekDay-exemplaar. |
| [hashCode()](#hashCode--) | Retourneert een hashcode-waarde voor het exemplaar van de [WeekDay](../../com.aspose.tasks/weekday) klasse. |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Stelt een waarde in die aangeeft of de opgegeven datum of dagtype werkend is. |
| [setDefaultWorkingTime(WeekDay day)](#setDefaultWorkingTime-com.aspose.tasks.WeekDay-) | Stelt standaard tijdsperioden in voor de opgegeven weekdag. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | Stelt het begin van een uitzonderingstijd in. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | Stelt het einde van een uitzonderingstijd in. |
### WeekDay(int dayType) {#WeekDay-int-}
```
public WeekDay(int dayType)
```


Initialiseert een nieuw exemplaar van de [WeekDay](../../com.aspose.tasks/weekday) klasse met het opgegeven dagtype.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dayType | int | Het opgegeven dagtype. |

### WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes) {#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--}
```
public WeekDay(int dayType, List<WorkingTime> workingTimes)
```


Initialiseert een nieuw exemplaar van de [WeekDay](../../com.aspose.tasks/weekday) klasse met het opgegeven dagtype en een lijst van werkperioden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dayType | int | Het opgegeven dagtype. |
| workingTimes | java.util.List&lt;com.aspose.tasks.WorkingTime&gt; | Lijst van werktijdperioden. |

### WeekDay(int dayType, WorkingTime[] workingTimes) {#WeekDay-int-com.aspose.tasks.WorkingTime...-}
```
public WeekDay(int dayType, WorkingTime[] workingTimes)
```


Initialiseert een nieuw exemplaar van de [WeekDay](../../com.aspose.tasks/weekday) klasse met het opgegeven dagtype en werkperioden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dayType | int | Het opgegeven dagtype. |
| workingTimes | [WorkingTime\[\]](../../com.aspose.tasks/workingtime) | Array van werktijdperioden. |

### WeekDay() {#WeekDay--}
```
public WeekDay()
```


Initialiseert een nieuw exemplaar van de [WeekDay](../../com.aspose.tasks/weekday) klasse.

### castToDayType(int dw) {#castToDayType-int-}
```
public static int castToDayType(int dw)
```


Cast .Net's [DayOfWeek](../../com.aspose.tasks/dayofweek) naar `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dw | int | De dag van de week om van te casten. |

**Returns:**
int - Een gecast dagtype.
### createDefaultWorkingDay(int dayType) {#createDefaultWorkingDay-int-}
```
public static WeekDay createDefaultWorkingDay(int dayType)
```


Maakt een standaard werkdag aan.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dayType | int | Het dagtype om een standaard werkdag van te maken. |

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - A default working day with working times 8-12 and 13-17.
### deepClone() {#deepClone--}
```
public final WeekDay deepClone()
```


Retourneert een diepe kopie van de weekdag.

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - Returns the deep copy of the week day.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | java.lang.Object | Het object om te vergelijken met deze instantie. |

**Returns:**
boolean - **True** als het opgegeven object een WeekDay is die dezelfde FromDate-, ToDate-waarden en WorkingTimes heeft als deze instantie; anders **false**.
### getDayType() {#getDayType--}
```
public final int getDayType()
```


Haalt het type van een dag op.

**Returns:**
int - het type van een dag.
### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Haalt een waarde op die aangeeft of de opgegeven datum of dagtype werkend is.

**Returns:**
boolean - een waarde die aangeeft of de opgegeven datum of dagtype werkend is.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


Haalt het begin van een uitzonderingstijd op.

**Returns:**
java.util.Date - het begin van een uitzonderingstijd.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


Haalt het einde van een uitzonderingstijd op.

**Returns:**
java.util.Date - het einde van een uitzonderingstijd.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Retourneert de werktijd voor een weekdag.

**Returns:**
double - Werk tijd.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


Haalt WorkingTimeCollection op voor deze WeekDay-instantie. De collectie werkuren die de op de weekdag gewerkte tijd definiëren.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - WorkingTimeCollection for this WeekDay instance.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Retourneert een hashcode-waarde voor het exemplaar van de [WeekDay](../../com.aspose.tasks/weekday) klasse.

**Returns:**
int - retourneert een hashcode-waarde voor dit object.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Stelt een waarde in die aangeeft of de opgegeven datum of dagtype werkend is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de opgegeven datum of dagtype werkend is. |

### setDefaultWorkingTime(WeekDay day) {#setDefaultWorkingTime-com.aspose.tasks.WeekDay-}
```
public static void setDefaultWorkingTime(WeekDay day)
```


Stelt standaard tijdsperioden in voor de opgegeven weekdag.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| day | [WeekDay](../../com.aspose.tasks/weekday) | De weekdag waarop de standaard werkdag moet worden ingesteld. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


Stelt het begin van een uitzonderingstijd in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | het begin van een uitzonderingstijd. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


Stelt het einde van een uitzonderingstijd in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | het einde van een uitzonderingstijd. |

