---
title: "RecurringTaskInfo"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt die Details einer wiederkehrenden Aufgabe in einem Projekt dar."
type: docs
weight: 244
url: /de/java/com.aspose.tasks/recurringtaskinfo/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskInfo
```

Stellt die Details einer wiederkehrenden Aufgabe in einem Projekt dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getDailyRepetitions()](#getDailyRepetitions--) | Gibt die Anzahl der Wiederholungen für das tägliche Wiederholungsmuster zurück. |
| [getDailyUseWorkdays()](#getDailyUseWorkdays--) | Gibt einen Wert zurück, der angibt, ob Arbeitstage für das tägliche Wiederholungsmuster verwendet werden sollen. |
| [getDuration()](#getDuration--) | Gibt die Dauer für ein Vorkommen der wiederkehrenden Aufgabe zurück. |
| [getEndDate()](#getEndDate--) | Gibt das Datum zurück, an dem die Vorkommen enden. |
| [getMonthlyDay()](#getMonthlyDay--) | Gibt die Anzahl der Tage des monatlichen Wiederholungsmusters zurück. |
| [getMonthlyOrdinalDay()](#getMonthlyOrdinalDay--) | Gibt einen Tag des monatlichen Wiederholungsmusters zurück, wenn ein Ordinaltag verwendet wird. |
| [getMonthlyOrdinalNumber()](#getMonthlyOrdinalNumber--) | Gibt eine Ordinalzahl des monatlichen Wiederholungsmusters zurück. |
| [getMonthlyOrdinalRepetitions()](#getMonthlyOrdinalRepetitions--) | Ermittelt die Anzahl der Wiederholungen für das monatliche Wiederholungsmuster, wenn ein Ordinaltag verwendet wird. |
| [getMonthlyRepetitions()](#getMonthlyRepetitions--) | Ermittelt die Anzahl der Wiederholungen für das monatliche Wiederholungsmuster. |
| [getMonthlyUseOrdinalDay()](#getMonthlyUseOrdinalDay--) | Ermittelt einen Wert, der angibt, ob ein Ordinaltag für das monatliche Wiederholungsmuster verwendet werden soll. |
| [getOccurrences()](#getOccurrences--) | Ermittelt die Anzahl der Vorkommen der wiederkehrenden Aufgabe. |
| [getRecurrencePattern()](#getRecurrencePattern--) | Ermittelt das Wiederholungsmuster der wiederkehrenden Aufgabe. |
| [getStartDate()](#getStartDate--) | Ermittelt das Datum, an dem die Vorkommen beginnen. |
| [getTask()](#getTask--) | Ermittelt die übergeordnete Aufgabe dieser Instanz der Klasse [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo). |
| [getUseEndDate()](#getUseEndDate--) | Ermittelt einen Wert, der angibt, ob das Enddatum oder eine Anzahl von Vorkommen für die wiederkehrende Aufgabe verwendet werden soll. |
| [getWeeklyDays()](#getWeeklyDays--) | Ermittelt eine Sammlung von Tagen, die im wöchentlichen Wiederholungsmuster verwendet werden. |
| [getWeeklyRepetitions()](#getWeeklyRepetitions--) | Ermittelt die Anzahl der Wiederholungen für das wöchentliche Wiederholungsmuster. |
| [getYearlyDate()](#getYearlyDate--) | Ermittelt ein Datum für das jährliche Wiederholungsmuster. |
| [getYearlyOrdinalDay()](#getYearlyOrdinalDay--) | Ermittelt einen Wochentag des jährlichen Wiederholungsmusters, wenn ein Ordinaltag verwendet wird. |
| [getYearlyOrdinalMonth()](#getYearlyOrdinalMonth--) | Ermittelt einen Monat des jährlichen Wiederholungsmusters, wenn ein Ordinaltag verwendet wird. |
| [getYearlyOrdinalNumber()](#getYearlyOrdinalNumber--) | Ermittelt eine Ordinalzahl des jährlichen Wiederholungsmusters. |
| [getYearlyUseOrdinalDay()](#getYearlyUseOrdinalDay--) | Ermittelt einen Wert, der angibt, ob ein Ordinaltag für das jährliche Wiederholungsmuster verwendet werden soll. |
| [setDailyRepetitions(int value)](#setDailyRepetitions-int-) | Legt die Anzahl der Wiederholungen für das tägliche Wiederholungsmuster fest. |
| [setDailyUseWorkdays(boolean value)](#setDailyUseWorkdays-boolean-) | Legt einen Wert fest, der angibt, ob Arbeitstage für das tägliche Wiederholungsmuster verwendet werden sollen. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Legt die Dauer für ein Vorkommen der wiederkehrenden Aufgabe fest. |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Legt das Datum fest, an dem die Vorkommen enden. |
| [setMonthlyDay(int value)](#setMonthlyDay-int-) | Legt die Anzahl der Tage des monatlichen Wiederholungsmusters fest. |
| [setMonthlyOrdinalDay(int value)](#setMonthlyOrdinalDay-int-) | Legt einen Tag des monatlichen Wiederholungsmusters fest, wenn ein Ordinaltag verwendet wird. |
| [setMonthlyOrdinalNumber(int value)](#setMonthlyOrdinalNumber-int-) | Legt eine Ordinalzahl des monatlichen Wiederholungsmusters fest. |
| [setMonthlyOrdinalRepetitions(int value)](#setMonthlyOrdinalRepetitions-int-) | Legt die Anzahl der Wiederholungen für das monatliche Wiederholungsmuster fest, wenn ein Ordinaltag verwendet wird. |
| [setMonthlyRepetitions(int value)](#setMonthlyRepetitions-int-) | Legt die Anzahl der Wiederholungen für das monatliche Wiederholungsmuster fest. |
| [setMonthlyUseOrdinalDay(boolean value)](#setMonthlyUseOrdinalDay-boolean-) | Legt einen Wert fest, der angibt, ob ein Ordinaltag für das monatliche Wiederholungsmuster verwendet werden soll. |
| [setOccurrences(int value)](#setOccurrences-int-) | Legt eine Anzahl von Vorkommen der wiederkehrenden Aufgabe fest. |
| [setRecurrencePattern(int value)](#setRecurrencePattern-int-) | Legt ein Wiederholungsmuster der wiederkehrenden Aufgabe fest. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Legt das Datum fest, an dem die Vorkommen beginnen. |
| [setUseEndDate(boolean value)](#setUseEndDate-boolean-) | Legt einen Wert fest, der angibt, ob das Enddatum oder eine Anzahl von Vorkommen für die wiederkehrende Aufgabe verwendet werden soll. |
| [setWeeklyDays(int value)](#setWeeklyDays-int-) | Legt eine Sammlung von Tagen fest, die im wöchentlichen Wiederholungsmuster verwendet werden. |
| [setWeeklyRepetitions(int value)](#setWeeklyRepetitions-int-) | Legt eine Anzahl von Wiederholungen für das wöchentliche Wiederholungsmuster fest. |
| [setYearlyDate(Date value)](#setYearlyDate-java.util.Date-) | Legt ein Datum für das jährliche Wiederholungsmuster fest. |
| [setYearlyOrdinalDay(int value)](#setYearlyOrdinalDay-int-) | Legt einen Wochentag des jährlichen Wiederholungsmusters fest, wenn ein Ordinaltag verwendet wird. |
| [setYearlyOrdinalMonth(int value)](#setYearlyOrdinalMonth-int-) | Legt einen Monat des jährlichen Wiederholungsmusters fest, wenn ein Ordinaltag verwendet wird. |
| [setYearlyOrdinalNumber(int value)](#setYearlyOrdinalNumber-int-) | Legt eine Ordnungszahl des jährlichen Wiederholungsmusters fest. |
| [setYearlyUseOrdinalDay(boolean value)](#setYearlyUseOrdinalDay-boolean-) | Legt einen Wert fest, der angibt, ob ein Ordinaltag für das jährliche Wiederholungsmuster verwendet werden soll. |
### getDailyRepetitions() {#getDailyRepetitions--}
```
public final int getDailyRepetitions()
```


Gibt die Anzahl der Wiederholungen für das tägliche Wiederholungsmuster zurück.

**Returns:**
int - eine Anzahl von Wiederholungen für das tägliche Wiederholungsmuster.
### getDailyUseWorkdays() {#getDailyUseWorkdays--}
```
public final boolean getDailyUseWorkdays()
```


Gibt einen Wert zurück, der angibt, ob Arbeitstage für das tägliche Wiederholungsmuster verwendet werden sollen.

**Returns:**
boolean - ein Wert, der angibt, ob Arbeitstage für das tägliche Wiederholungsmuster verwendet werden sollen.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Gibt die Dauer für ein Vorkommen der wiederkehrenden Aufgabe zurück.

--------------------

die Instanz der `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)) Klasse.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration for one occurrence of the recurring task.
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Gibt das Datum zurück, an dem die Vorkommen enden.

**Returns:**
java.util.Date - das Datum, an dem die Vorkommen enden.
### getMonthlyDay() {#getMonthlyDay--}
```
public final int getMonthlyDay()
```


Gibt die Anzahl der Tage des monatlichen Wiederholungsmusters zurück.

**Returns:**
int - eine Anzahl von Tagen des monatlichen Wiederholungsmusters.
### getMonthlyOrdinalDay() {#getMonthlyOrdinalDay--}
```
public final int getMonthlyOrdinalDay()
```


Gibt einen Tag des monatlichen Wiederholungsmusters zurück, wenn ein Ordinaltag verwendet wird.

--------------------

Kann einer der Werte der [DayOfWeek](../../com.aspose.tasks/dayofweek) Aufzählung sein.

**Returns:**
int - ein Tag des monatlichen Wiederholungsmusters, wenn ein Ordinaltag verwendet wird.
### getMonthlyOrdinalNumber() {#getMonthlyOrdinalNumber--}
```
public final int getMonthlyOrdinalNumber()
```


Gibt eine Ordinalzahl des monatlichen Wiederholungsmusters zurück.

--------------------

Kann einer der Werte der [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) Aufzählung sein.

**Returns:**
int - eine Ordnungszahl des monatlichen Wiederholungsmusters.
### getMonthlyOrdinalRepetitions() {#getMonthlyOrdinalRepetitions--}
```
public final int getMonthlyOrdinalRepetitions()
```


Ermittelt die Anzahl der Wiederholungen für das monatliche Wiederholungsmuster, wenn ein Ordinaltag verwendet wird.

**Returns:**
int - eine Anzahl von Wiederholungen für das monatliche Wiederholungsmuster, wenn ein Ordinaltag verwendet wird.
### getMonthlyRepetitions() {#getMonthlyRepetitions--}
```
public final int getMonthlyRepetitions()
```


Ermittelt die Anzahl der Wiederholungen für das monatliche Wiederholungsmuster.

**Returns:**
int - eine Anzahl von Wiederholungen für das monatliche Wiederholungsmuster.
### getMonthlyUseOrdinalDay() {#getMonthlyUseOrdinalDay--}
```
public final boolean getMonthlyUseOrdinalDay()
```


Ermittelt einen Wert, der angibt, ob ein Ordinaltag für das monatliche Wiederholungsmuster verwendet werden soll.

**Returns:**
boolean - ein Wert, der angibt, ob ein Ordinaltag für das monatliche Wiederholungsmuster verwendet werden soll.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Ermittelt die Anzahl der Vorkommen der wiederkehrenden Aufgabe.

**Returns:**
int - eine Anzahl von Vorkommen der wiederkehrenden Aufgabe.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final int getRecurrencePattern()
```


Ermittelt das Wiederholungsmuster der wiederkehrenden Aufgabe.

--------------------

Kann einer der Werte der `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)) Aufzählung sein.

**Returns:**
int - ein Wiederholungsmuster der wiederkehrenden Aufgabe.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Ermittelt das Datum, an dem die Vorkommen beginnen.

**Returns:**
java.util.Date - das Datum, an dem die Vorkommen beginnen.
### getTask() {#getTask--}
```
public final Task getTask()
```


Ermittelt die übergeordnete Aufgabe dieser Instanz der Klasse [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo).

**Returns:**
[Task](../../com.aspose.tasks/task) - the parent task of this instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class.
### getUseEndDate() {#getUseEndDate--}
```
public final boolean getUseEndDate()
```


Ermittelt einen Wert, der angibt, ob das Enddatum oder eine Anzahl von Vorkommen für die wiederkehrende Aufgabe verwendet werden soll.

**Returns:**
boolean - ein Wert, der angibt, ob das Enddatum oder eine Anzahl von Vorkommen für die wiederkehrende Aufgabe verwendet werden soll.
### getWeeklyDays() {#getWeeklyDays--}
```
public final int getWeeklyDays()
```


Ermittelt eine Sammlung von Tagen, die im wöchentlichen Wiederholungsmuster verwendet werden.

--------------------

**Returns:**
int - eine Sammlung von Tagen, die im wöchentlichen Wiederholungsmuster verwendet werden.
### getWeeklyRepetitions() {#getWeeklyRepetitions--}
```
public final int getWeeklyRepetitions()
```


Ermittelt die Anzahl der Wiederholungen für das wöchentliche Wiederholungsmuster.

**Returns:**
int - eine Anzahl von Wiederholungen für das wöchentliche Wiederholungsmuster.
### getYearlyDate() {#getYearlyDate--}
```
public final Date getYearlyDate()
```


Ermittelt ein Datum für das jährliche Wiederholungsmuster.

**Returns:**
java.util.Date - ein Datum für das jährliche Wiederholungsmuster.
### getYearlyOrdinalDay() {#getYearlyOrdinalDay--}
```
public final int getYearlyOrdinalDay()
```


Ermittelt einen Wochentag des jährlichen Wiederholungsmusters, wenn ein Ordinaltag verwendet wird.

--------------------

Kann einer der Werte der [DayOfWeek](../../com.aspose.tasks/dayofweek) Aufzählung sein.

**Returns:**
int - ein Wochentag des jährlichen Wiederholungsmusters bei Verwendung eines Ordinaltages.
### getYearlyOrdinalMonth() {#getYearlyOrdinalMonth--}
```
public final int getYearlyOrdinalMonth()
```


Ermittelt einen Monat des jährlichen Wiederholungsmusters, wenn ein Ordinaltag verwendet wird.

--------------------

Kann einer der Werte der [Month](../../com.aspose/tasks/month)-Aufzählung sein.

**Returns:**
int - ein Monat des jährlichen Wiederholungsmusters bei Verwendung eines Ordinaltages.
### getYearlyOrdinalNumber() {#getYearlyOrdinalNumber--}
```
public final int getYearlyOrdinalNumber()
```


Ermittelt eine Ordinalzahl des jährlichen Wiederholungsmusters.

--------------------

Kann einer der Werte der [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) Aufzählung sein.

**Returns:**
int - eine Ordinalzahl des jährlichen Wiederholungsmusters.
### getYearlyUseOrdinalDay() {#getYearlyUseOrdinalDay--}
```
public final boolean getYearlyUseOrdinalDay()
```


Ermittelt einen Wert, der angibt, ob ein Ordinaltag für das jährliche Wiederholungsmuster verwendet werden soll.

**Returns:**
boolean - ein Wert, der angibt, ob ein Ordinaltag für das jährliche Wiederholungsmuster verwendet werden soll.
### setDailyRepetitions(int value) {#setDailyRepetitions-int-}
```
public final void setDailyRepetitions(int value)
```


Legt die Anzahl der Wiederholungen für das tägliche Wiederholungsmuster fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | eine Anzahl von Wiederholungen für das tägliche Wiederholungsmuster. |

### setDailyUseWorkdays(boolean value) {#setDailyUseWorkdays-boolean-}
```
public final void setDailyUseWorkdays(boolean value)
```


Legt einen Wert fest, der angibt, ob Arbeitstage für das tägliche Wiederholungsmuster verwendet werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Arbeitstage für das tägliche Wiederholungsmuster verwendet werden sollen. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Legt die Dauer für ein Vorkommen der wiederkehrenden Aufgabe fest.

--------------------

die Instanz der `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)) Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | die Dauer für ein Vorkommen der wiederkehrenden Aufgabe. |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Legt das Datum fest, an dem die Vorkommen enden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | das Datum, an dem die Vorkommen enden. |

### setMonthlyDay(int value) {#setMonthlyDay-int-}
```
public final void setMonthlyDay(int value)
```


Legt die Anzahl der Tage des monatlichen Wiederholungsmusters fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | eine Anzahl von Tagen des monatlichen Wiederholungsmusters. |

### setMonthlyOrdinalDay(int value) {#setMonthlyOrdinalDay-int-}
```
public final void setMonthlyOrdinalDay(int value)
```


Legt einen Tag des monatlichen Wiederholungsmusters fest, wenn ein Ordinaltag verwendet wird.

--------------------

Kann einer der Werte der [DayOfWeek](../../com.aspose.tasks/dayofweek) Aufzählung sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Tag des monatlichen Wiederholungsmusters bei Verwendung eines Ordinaltages. |

### setMonthlyOrdinalNumber(int value) {#setMonthlyOrdinalNumber-int-}
```
public final void setMonthlyOrdinalNumber(int value)
```


Legt eine Ordinalzahl des monatlichen Wiederholungsmusters fest.

--------------------

Kann einer der Werte der [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) Aufzählung sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | eine Ordinalzahl des monatlichen Wiederholungsmusters. |

### setMonthlyOrdinalRepetitions(int value) {#setMonthlyOrdinalRepetitions-int-}
```
public final void setMonthlyOrdinalRepetitions(int value)
```


Legt die Anzahl der Wiederholungen für das monatliche Wiederholungsmuster fest, wenn ein Ordinaltag verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | eine Anzahl von Wiederholungen für das monatliche Wiederholungsmuster bei Verwendung eines Ordinaltages. |

### setMonthlyRepetitions(int value) {#setMonthlyRepetitions-int-}
```
public final void setMonthlyRepetitions(int value)
```


Legt die Anzahl der Wiederholungen für das monatliche Wiederholungsmuster fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | eine Anzahl von Wiederholungen für das monatliche Wiederholungsmuster. |

### setMonthlyUseOrdinalDay(boolean value) {#setMonthlyUseOrdinalDay-boolean-}
```
public final void setMonthlyUseOrdinalDay(boolean value)
```


Legt einen Wert fest, der angibt, ob ein Ordinaltag für das monatliche Wiederholungsmuster verwendet werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob ein Ordinaltag für das monatliche Wiederholungsmuster verwendet werden soll. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Legt eine Anzahl von Vorkommen der wiederkehrenden Aufgabe fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | eine Anzahl von Vorkommen der wiederkehrenden Aufgabe. |

### setRecurrencePattern(int value) {#setRecurrencePattern-int-}
```
public final void setRecurrencePattern(int value)
```


Legt ein Wiederholungsmuster der wiederkehrenden Aufgabe fest.

--------------------

Kann einer der Werte der `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)) Aufzählung sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Wiederholungsmuster der wiederkehrenden Aufgabe. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Legt das Datum fest, an dem die Vorkommen beginnen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | das Datum, an dem die Vorkommen beginnen. |

### setUseEndDate(boolean value) {#setUseEndDate-boolean-}
```
public final void setUseEndDate(boolean value)
```


Legt einen Wert fest, der angibt, ob das Enddatum oder eine Anzahl von Vorkommen für die wiederkehrende Aufgabe verwendet werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob das Enddatum oder eine Anzahl von Vorkommen für die wiederkehrende Aufgabe verwendet werden soll. |

### setWeeklyDays(int value) {#setWeeklyDays-int-}
```
public final void setWeeklyDays(int value)
```


Legt eine Sammlung von Tagen fest, die im wöchentlichen Wiederholungsmuster verwendet werden.

--------------------

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | eine Sammlung von Tagen, die im wöchentlichen Wiederholungsmuster verwendet werden. |

### setWeeklyRepetitions(int value) {#setWeeklyRepetitions-int-}
```
public final void setWeeklyRepetitions(int value)
```


Legt eine Anzahl von Wiederholungen für das wöchentliche Wiederholungsmuster fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | eine Anzahl von Wiederholungen für das wöchentliche Wiederholungsmuster. |

### setYearlyDate(Date value) {#setYearlyDate-java.util.Date-}
```
public final void setYearlyDate(Date value)
```


Legt ein Datum für das jährliche Wiederholungsmuster fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | ein Datum für das jährliche Wiederholungsmuster. |

### setYearlyOrdinalDay(int value) {#setYearlyOrdinalDay-int-}
```
public final void setYearlyOrdinalDay(int value)
```


Legt einen Wochentag des jährlichen Wiederholungsmusters fest, wenn ein Ordinaltag verwendet wird.

--------------------

Kann einer der Werte der [DayOfWeek](../../com.aspose.tasks/dayofweek) Aufzählung sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Wochentag des jährlichen Wiederholungsmusters bei Verwendung eines Ordinaltages. |

### setYearlyOrdinalMonth(int value) {#setYearlyOrdinalMonth-int-}
```
public final void setYearlyOrdinalMonth(int value)
```


Legt einen Monat des jährlichen Wiederholungsmusters fest, wenn ein Ordinaltag verwendet wird.

--------------------

Kann einer der Werte der [Month](../../com.aspose/tasks/month)-Aufzählung sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Monat des jährlichen Wiederholungsmusters bei Verwendung eines Ordinaltages. |

### setYearlyOrdinalNumber(int value) {#setYearlyOrdinalNumber-int-}
```
public final void setYearlyOrdinalNumber(int value)
```


Legt eine Ordnungszahl des jährlichen Wiederholungsmusters fest.

--------------------

Kann einer der Werte der [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) Aufzählung sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | eine Ordinalzahl des jährlichen Wiederholungsmusters. |

### setYearlyUseOrdinalDay(boolean value) {#setYearlyUseOrdinalDay-boolean-}
```
public final void setYearlyUseOrdinalDay(boolean value)
```


Legt einen Wert fest, der angibt, ob ein Ordinaltag für das jährliche Wiederholungsmuster verwendet werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob ein Ordinaltag für das jährliche Wiederholungsmuster verwendet werden soll. |

