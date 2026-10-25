---
title: "WeekDay"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt einen Wochentag dar, der entweder reguläre Tage einer Woche oder Ausnahme‑tage in einem Kalender definiert."
type: docs
weight: 352
url: /de/java/com.aspose.tasks/weekday/
---

**Inheritance:**
java.lang.Object
```
public class WeekDay
```

Stellt einen Wochentag dar, der entweder reguläre Tage einer Woche oder Ausnahme‑tage in einem Kalender definiert.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [WeekDay(int dayType)](#WeekDay-int-) | Initialisiert eine neue Instanz der [WeekDay](../../com.aspose.tasks/weekday) Klasse mit dem angegebenen Tagtyp. |
| [WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes)](#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--) | Initialisiert eine neue Instanz der [WeekDay](../../com.aspose.tasks/weekday) Klasse mit dem angegebenen Tagtyp und einer Liste von Arbeitszeiträumen. |
| [WeekDay(int dayType, WorkingTime[] workingTimes)](#WeekDay-int-com.aspose.tasks.WorkingTime...-) | Initialisiert eine neue Instanz der [WeekDay](../../com.aspose.tasks/weekday) Klasse mit dem angegebenen Tagtyp und Arbeitszeiträumen. |
| [WeekDay()](#WeekDay--) | Initialisiert eine neue Instanz der [WeekDay](../../com.aspose.tasks/weekday) Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [castToDayType(int dw)](#castToDayType-int-) | Wandelt .Net's [DayOfWeek](../../com.aspose.tasks/dayofweek) in `DayType`([getDayType()](../../com.aspose.tasks/weekday\\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\\#setDayType-int-)) um. |
| [createDefaultWorkingDay(int dayType)](#createDefaultWorkingDay-int-) | Erstellt einen Standard-Arbeitstag. |
| [deepClone()](#deepClone--) | Gibt eine tiefe Kopie des Wochentags zurück. |
| [equals(Object obj)](#equals-java.lang.Object-) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [getDayType()](#getDayType--) | Ermittelt den Typ eines Tages. |
| [getDayWorking()](#getDayWorking--) | Ermittelt einen Wert, der angibt, ob das angegebene Datum oder der Tagtyp ein Arbeitstag ist. |
| [getFromDate()](#getFromDate--) | Ermittelt den Beginn einer Ausnahmezeit. |
| [getToDate()](#getToDate--) | Ermittelt das Ende einer Ausnahmezeit. |
| [getWorkingTime()](#getWorkingTime--) | Gibt die Arbeitszeit für einen Wochentag zurück. |
| [getWorkingTimes()](#getWorkingTimes--) | Ermittelt WorkingTimeCollection für diese WeekDay-Instanz. |
| [hashCode()](#hashCode--) | Gibt einen Hashcode-Wert für die Instanz der [WeekDay](../../com.aspose.tasks/weekday) Klasse zurück. |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Legt einen Wert fest, der angibt, ob das angegebene Datum oder der Tagtyp ein Arbeitstag ist. |
| [setDefaultWorkingTime(WeekDay day)](#setDefaultWorkingTime-com.aspose.tasks.WeekDay-) | Legt Standardzeiträume für den angegebenen Wochentag fest. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | Legt den Beginn einer Ausnahmezeit fest. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | Legt das Ende einer Ausnahmezeit fest. |
### WeekDay(int dayType) {#WeekDay-int-}
```
public WeekDay(int dayType)
```


Initialisiert eine neue Instanz der [WeekDay](../../com.aspose.tasks/weekday) Klasse mit dem angegebenen Tagtyp.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dayType | int | Der angegebene Tagtyp. |

### WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes) {#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--}
```
public WeekDay(int dayType, List<WorkingTime> workingTimes)
```


Initialisiert eine neue Instanz der [WeekDay](../../com.aspose.tasks/weekday) Klasse mit dem angegebenen Tagtyp und einer Liste von Arbeitszeiträumen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dayType | int | Der angegebene Tagtyp. |
| workingTimes | java.util.List&lt;com.aspose.tasks.WorkingTime&gt; | Liste von Arbeitszeiträumen. |

### WeekDay(int dayType, WorkingTime[] workingTimes) {#WeekDay-int-com.aspose.tasks.WorkingTime...-}
```
public WeekDay(int dayType, WorkingTime[] workingTimes)
```


Initialisiert eine neue Instanz der [WeekDay](../../com.aspose.tasks/weekday) Klasse mit dem angegebenen Tagtyp und Arbeitszeiträumen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dayType | int | Der angegebene Tagtyp. |
| workingTimes | [WorkingTime\[\]](../../com.aspose.tasks/workingtime) | Array von Arbeitszeiträumen. |

### WeekDay() {#WeekDay--}
```
public WeekDay()
```


Initialisiert eine neue Instanz der [WeekDay](../../com.aspose.tasks/weekday) Klasse.

### castToDayType(int dw) {#castToDayType-int-}
```
public static int castToDayType(int dw)
```


Wandelt .Net's [DayOfWeek](../../com.aspose.tasks/dayofweek) in `DayType`([getDayType()](../../com.aspose.tasks/weekday\\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\\#setDayType-int-)) um.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dw | int | Der Wochentag, von dem konvertiert werden soll. |

**Returns:**
int - Ein konvertierter Tagtyp.
### createDefaultWorkingDay(int dayType) {#createDefaultWorkingDay-int-}
```
public static WeekDay createDefaultWorkingDay(int dayType)
```


Erstellt einen Standard-Arbeitstag.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dayType | int | Der Tagtyp, aus dem ein Standardarbeitstag erstellt wird. |

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - A default working day with working times 8-12 and 13-17.
### deepClone() {#deepClone--}
```
public final WeekDay deepClone()
```


Gibt eine tiefe Kopie des Wochentags zurück.

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - Returns the deep copy of the week day.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | Das Objekt, das mit dieser Instanz verglichen wird. |

**Returns:**
boolean - **True** wenn das angegebene Objekt ein WeekDay ist, das die gleichen FromDate-, ToDate-Werte und WorkingTimes wie diese Instanz hat; andernfalls **false**.
### getDayType() {#getDayType--}
```
public final int getDayType()
```


Ermittelt den Typ eines Tages.

**Returns:**
int - der Typ eines Tages.
### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Ermittelt einen Wert, der angibt, ob das angegebene Datum oder der Tagtyp ein Arbeitstag ist.

**Returns:**
boolean - ein Wert, der angibt, ob das angegebene Datum oder der Tagtyp ein Arbeitstag ist.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


Ermittelt den Beginn einer Ausnahmezeit.

**Returns:**
java.util.Date - der Beginn einer Ausnahmezeit.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


Ermittelt das Ende einer Ausnahmezeit.

**Returns:**
java.util.Date - das Ende einer Ausnahmezeit.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Gibt die Arbeitszeit für einen Wochentag zurück.

**Returns:**
double - Arbeitszeit.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


Ruft WorkingTimeCollection für diese WeekDay-Instanz ab. Die Sammlung von Arbeitszeiten, die die am Wochentag gearbeitete Zeit definieren.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - WorkingTimeCollection for this WeekDay instance.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Gibt einen Hashcode-Wert für die Instanz der [WeekDay](../../com.aspose.tasks/weekday) Klasse zurück.

**Returns:**
int - gibt einen Hashcode-Wert für dieses Objekt zurück.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Legt einen Wert fest, der angibt, ob das angegebene Datum oder der Tagtyp ein Arbeitstag ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob das angegebene Datum oder der Tagtyp ein Arbeitstag ist. |

### setDefaultWorkingTime(WeekDay day) {#setDefaultWorkingTime-com.aspose.tasks.WeekDay-}
```
public static void setDefaultWorkingTime(WeekDay day)
```


Legt Standardzeiträume für den angegebenen Wochentag fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| day | [WeekDay](../../com.aspose.tasks/weekday) | Der Wochentag, für den ein Standardarbeitstag festgelegt werden soll. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


Legt den Beginn einer Ausnahmezeit fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | der Beginn einer Ausnahmezeit. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


Legt das Ende einer Ausnahmezeit fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | das Ende einer Ausnahmezeit. |

