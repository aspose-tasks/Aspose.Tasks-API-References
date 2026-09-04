---
title: "CalendarException"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt außergewöhnliche Zeiträume in einem Kalender dar."
type: docs
weight: 43
url: /de/java/com.aspose.tasks/calendarexception/
---

**Inheritance:**
java.lang.Object
```
public final class CalendarException
```

Stellt außergewöhnliche Zeiträume in einem Kalender dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CalendarException()](#CalendarException--) | Initialisiert eine neue Instanz der Klasse [CalendarException](../../com.aspose.tasks/calendarexception). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [checkException(Date dt)](#checkException-java.util.Date-) | Gibt true zurück, wenn die angegebene Instanz der Struktur java.util.Date der Ausnahmetag ist. |
| [delete()](#delete--) | Löscht die Exception‑Instanz aus dem übergeordneten Kalenderobjekt CalendarExceptionCollection. |
| [getDayWorking()](#getDayWorking--) | Ermittelt einen Wert, der angibt, ob das angegebene Datum oder der Tagtyp ein Arbeitstag ist. |
| [getDaysOfWeek()](#getDaysOfWeek--) | Ruft die DayTypeCollection für dieses Objekt ab. |
| [getEnteredByOccurrences()](#getEnteredByOccurrences--) | Ruft einen Wert ab, der angibt, ob der Wiederholungsbereich durch Eingabe einer Anzahl von Vorkommen definiert ist. |
| [getExceptionDates()](#getExceptionDates--) | Gibt Daten zurück, an denen die Kalenderausnahme gilt. |
| [getFromDate()](#getFromDate--) | Ruft den Beginn der Ausnahmezeit ab. |
| [getMonth()](#getMonth--) | Ruft den Monat ab, für den eine Ausnahmewiederholung geplant ist. |
| [getMonthDay()](#getMonthDay--) | Ruft den Tag des Monats ab, an dem eine Ausnahmewiederholung geplant ist. |
| [getMonthItem()](#getMonthItem--) | Ruft das Monatselement ab, für das eine Ausnahmewiederholung geplant ist. |
| [getMonthPosition()](#getMonthPosition--) | Ruft die Position eines Monatselements innerhalb eines Monats ab. |
| [getName()](#getName--) | Ruft den Namen der Ausnahme ab. |
| [getOccurrences()](#getOccurrences--) | Ruft die Anzahl der Vorkommen ab, für die die Kalenderausnahme gültig ist. |
| [getParentCalendar()](#getParentCalendar--) | Ermittelt den übergeordneten Kalender für dieses Objekt. |
| [getPeriod()](#getPeriod--) | Ruft den Wiederholungszeitraum für die Ausnahme ab. |
| [getToDate()](#getToDate--) | Ruft das Ende der Ausnahmezeit ab. |
| [getType()](#getType--) | Ruft den Ausnahmetyp ab. |
| [getWorkingTime()](#getWorkingTime--) | Gibt die Arbeitszeit für eine Kalenderausnahme zurück. |
| [getWorkingTimes()](#getWorkingTimes--) | Ruft das WorkingTimeCollection-Objekt ab. |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Legt einen Wert fest, der angibt, ob das angegebene Datum oder der Tagtyp ein Arbeitstag ist. |
| [setEnteredByOccurrences(boolean value)](#setEnteredByOccurrences-boolean-) | Legt einen Wert fest, der angibt, ob der Wiederholungsbereich durch Eingabe einer Anzahl von Vorkommen definiert ist. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | Legt den Beginn der Ausnahmezeit fest. |
| [setMonth(int value)](#setMonth-int-) | Legt den Monat fest, für den eine Ausnahmewiederholung geplant ist. |
| [setMonthDay(int value)](#setMonthDay-int-) | Legt den Tag des Monats fest, an dem eine Ausnahmewiederholung geplant ist. |
| [setMonthItem(int value)](#setMonthItem-int-) | Legt das Monatselement fest, für das eine Ausnahmewiederholung geplant ist. |
| [setMonthPosition(int value)](#setMonthPosition-int-) | Legt die Position eines Monatselements innerhalb eines Monats fest. |
| [setName(String value)](#setName-java.lang.String-) | Legt den Namen der Ausnahme fest. |
| [setOccurrences(int value)](#setOccurrences-int-) | Legt die Anzahl der Vorkommen fest, für die die Kalenderausnahme gültig ist. |
| [setPeriod(int value)](#setPeriod-int-) | Legt den Wiederholungszeitraum für die Ausnahme fest. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | Legt das Ende der Ausnahmezeit fest. |
| [setType(int value)](#setType-int-) | Setzt den Ausnahmetyp. |
| [setWorkingTimes(WorkingTimeCollection value)](#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-) | Setzt das WorkingTimeCollection-Objekt. |
### CalendarException() {#CalendarException--}
```
public CalendarException()
```


Initialisiert eine neue Instanz der Klasse [CalendarException](../../com.aspose.tasks/calendarexception).

### checkException(Date dt) {#checkException-java.util.Date-}
```
public final boolean checkException(Date dt)
```


Gibt true zurück, wenn die angegebene Instanz der Struktur java.util.Date der Ausnahmetag ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dt | java.util.Date | die angegebene Instanz der java.util.Date-Struktur. |

**Returns:**
boolean - Gibt true zurück, wenn der java.util.Date-Wert der Ausnahmetag ist; andernfalls false.
### delete() {#delete--}
```
public final void delete()
```


Löscht die Exception‑Instanz aus dem übergeordneten Kalenderobjekt CalendarExceptionCollection.

### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Ermittelt einen Wert, der angibt, ob das angegebene Datum oder der Tagtyp ein Arbeitstag ist.

**Returns:**
boolean - ein Wert, der angibt, ob das angegebene Datum oder der Tagtyp ein Arbeitstag ist.
### getDaysOfWeek() {#getDaysOfWeek--}
```
public final DayTypeCollection getDaysOfWeek()
```


Ruft die DayTypeCollection für dieses Objekt ab. Die Wochentage, an denen die Ausnahme gültig ist.

**Returns:**
[DayTypeCollection](../../com.aspose.tasks/daytypecollection) - the DayTypeCollection for this object.
### getEnteredByOccurrences() {#getEnteredByOccurrences--}
```
public final boolean getEnteredByOccurrences()
```


Ruft einen Wert ab, der angibt, ob der Wiederholungsbereich durch Eingabe einer Anzahl von Vorkommen definiert ist. False gibt an, dass der Wiederholungsbereich durch Eingabe eines Enddatums definiert ist.

**Returns:**
boolean - ein Wert, der angibt, ob der Wiederholungsbereich durch Eingabe einer Anzahl von Vorkommen definiert ist.
### getExceptionDates() {#getExceptionDates--}
```
public final Iterable<Date> getExceptionDates()
```


Gibt Daten zurück, an denen die Kalenderausnahme gilt.

**Returns:**
java.lang.Iterable&lt;java.util.Date&gt; - Datumseinträge, für die die Kalenderausnahme gilt.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


Ruft den Beginn der Ausnahmezeit ab.

**Returns:**
java.util.Date - der Beginn der Ausnahmezeit.
### getMonth() {#getMonth--}
```
public final int getMonth()
```


Ruft den Monat ab, für den eine Ausnahmewiederholung geplant ist.

**Returns:**
int - der Monat, für den eine Ausnahmewiederholung geplant ist.
### getMonthDay() {#getMonthDay--}
```
public final int getMonthDay()
```


Ruft den Tag des Monats ab, an dem eine Ausnahmewiederholung geplant ist.

**Returns:**
int - der Tag des Monats, an dem eine Ausnahmewiederholung geplant ist.
### getMonthItem() {#getMonthItem--}
```
public final int getMonthItem()
```


Ruft das Monatselement ab, für das eine Ausnahmewiederholung geplant ist.

**Returns:**
int - das Monatselement, für das eine Ausnahmewiederholung geplant ist.
### getMonthPosition() {#getMonthPosition--}
```
public final int getMonthPosition()
```


Ruft die Position eines Monatselements innerhalb eines Monats ab.

**Returns:**
int - die Position eines Monatselements innerhalb eines Monats.
### getName() {#getName--}
```
public final String getName()
```


Ruft den Namen der Ausnahme ab.

**Returns:**
java.lang.String - der Name der Ausnahme.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Ruft die Anzahl der Vorkommen ab, für die die Kalenderausnahme gültig ist.

**Returns:**
int - die Anzahl der Vorkommen, für die die Kalenderausnahme gültig ist.
### getParentCalendar() {#getParentCalendar--}
```
public final Calendar getParentCalendar()
```


Ermittelt den übergeordneten Kalender für dieses Objekt.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - the parent calendar for this object.
### getPeriod() {#getPeriod--}
```
public final int getPeriod()
```


Ruft den Wiederholungszeitraum für die Ausnahme ab.

**Returns:**
int - der Wiederholungszeitraum für die Ausnahme.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


Ruft das Ende der Ausnahmezeit ab.

**Returns:**
java.util.Date - das Ende der Ausnahmezeit.
### getType() {#getType--}
```
public final int getType()
```


Ruft den Ausnahmetyp ab.

**Returns:**
int - der Ausnahmetyp.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Gibt die Arbeitszeit für eine Kalenderausnahme zurück.

**Returns:**
double - Gibt die Arbeitszeit für diese Kalenderausnahme zurück.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


Ruft das WorkingTimeCollection-Objekt ab. Die Sammlung von Arbeitszeiten, die die an einem Wochentag gearbeitete Zeit definiert.

--------------------

Mindestens eine Arbeitszeit muss vorhanden sein, und es dürfen nicht mehr als fünf sein.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - the WorkingTimeCollection object.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Legt einen Wert fest, der angibt, ob das angegebene Datum oder der Tagtyp ein Arbeitstag ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob das angegebene Datum oder der Tagtyp ein Arbeitstag ist. |

### setEnteredByOccurrences(boolean value) {#setEnteredByOccurrences-boolean-}
```
public final void setEnteredByOccurrences(boolean value)
```


Setzt einen Wert, der angibt, ob der Wiederholungsbereich durch Eingabe einer Anzahl von Vorkommen definiert ist. False gibt an, dass der Wiederholungsbereich durch Eingabe eines Enddatums definiert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob der Wiederholungsbereich durch Eingabe einer Anzahl von Vorkommen definiert ist. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


Legt den Beginn der Ausnahmezeit fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | der Beginn der Ausnahmezeit. |

### setMonth(int value) {#setMonth-int-}
```
public final void setMonth(int value)
```


Legt den Monat fest, für den eine Ausnahmewiederholung geplant ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | der Monat, für den eine Ausnahmewiederholung geplant ist. |

### setMonthDay(int value) {#setMonthDay-int-}
```
public final void setMonthDay(int value)
```


Legt den Tag des Monats fest, an dem eine Ausnahmewiederholung geplant ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | der Tag eines Monats, an dem eine Ausnahmewiederholung geplant ist. |

### setMonthItem(int value) {#setMonthItem-int-}
```
public final void setMonthItem(int value)
```


Legt das Monatselement fest, für das eine Ausnahmewiederholung geplant ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | das Monatselement, für das eine Ausnahmewiederholung geplant ist. |

### setMonthPosition(int value) {#setMonthPosition-int-}
```
public final void setMonthPosition(int value)
```


Legt die Position eines Monatselements innerhalb eines Monats fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | die Position eines Monatselements innerhalb eines Monats. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Legt den Namen der Ausnahme fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | der Name der Ausnahme. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Legt die Anzahl der Vorkommen fest, für die die Kalenderausnahme gültig ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | die Anzahl der Vorkommen, für die die Kalendarausnahme gültig ist. |

### setPeriod(int value) {#setPeriod-int-}
```
public final void setPeriod(int value)
```


Legt den Wiederholungszeitraum für die Ausnahme fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | der Wiederholungszeitraum für die Ausnahme. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


Legt das Ende der Ausnahmezeit fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | das Ende der Ausnahmezeit. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Setzt den Ausnahmetyp.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | der Ausnahmetyp. |

### setWorkingTimes(WorkingTimeCollection value) {#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-}
```
public final void setWorkingTimes(WorkingTimeCollection value)
```


Setzt das WorkingTimeCollection-Objekt. Die Sammlung von Arbeitszeiten, die die an einem Wochentag gearbeitete Zeit definiert.

--------------------

Mindestens eine Arbeitszeit muss vorhanden sein, und es dürfen nicht mehr als fünf sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) | das WorkingTimeCollection-Objekt. |

