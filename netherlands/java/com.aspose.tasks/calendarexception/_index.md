---
title: "CalendarException"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt uitzonderlijke tijdsperioden in een kalender voor."
type: docs
weight: 43
url: /nl/java/com.aspose.tasks/calendarexception/
---

**Inheritance:**
java.lang.Object
```
public final class CalendarException
```

Stelt uitzonderlijke tijdsperioden in een kalender voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [CalendarException()](#CalendarException--) | Initialiseert een nieuw exemplaar van de [CalendarException](../../com.aspose.tasks/calendarexception) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [checkException(Date dt)](#checkException-java.util.Date-) | Retourneert true als de opgegeven instantie van de java.util.Date struct de exceptiedag is. |
| [delete()](#delete--) | Verwijdert de exceptie‑instantie uit het bovenliggende kalenderobject CalendarExceptionCollection. |
| [getDayWorking()](#getDayWorking--) | Haalt een waarde op die aangeeft of de opgegeven datum of dagtype werkend is. |
| [getDaysOfWeek()](#getDaysOfWeek--) | Haalt de DayTypeCollection op voor dit object. |
| [getEnteredByOccurrences()](#getEnteredByOccurrences--) | Haalt een waarde op die aangeeft of het bereik van herhaling wordt gedefinieerd door een aantal herhalingen in te voeren. |
| [getExceptionDates()](#getExceptionDates--) | Retourneert data waarop de kalenderuitzondering van toepassing is. |
| [getFromDate()](#getFromDate--) | Haalt het begin van de exceptietijd op. |
| [getMonth()](#getMonth--) | Haalt de maand op waarvoor een exceptie‑herhaling is gepland. |
| [getMonthDay()](#getMonthDay--) | Haalt de dag van de maand op waarop een exceptie‑herhaling is gepland. |
| [getMonthItem()](#getMonthItem--) | Haalt het maanditem op waarvoor een exceptie‑herhaling is gepland. |
| [getMonthPosition()](#getMonthPosition--) | Haalt de positie van een maanditem binnen een maand op. |
| [getName()](#getName--) | Haalt de naam van de exceptie op. |
| [getOccurrences()](#getOccurrences--) | Haalt het aantal herhalingen op waarvoor de kalenderuitzondering geldig is. |
| [getParentCalendar()](#getParentCalendar--) | Haalt de bovenliggende agenda op voor dit object. |
| [getPeriod()](#getPeriod--) | Haalt de periode van herhaling voor de exceptie op. |
| [getToDate()](#getToDate--) | Haalt het einde van de exceptietijd op. |
| [getType()](#getType--) | Haalt het type van de exceptie op. |
| [getWorkingTime()](#getWorkingTime--) | Retourneert de werktijd voor een kalenderuitzondering. |
| [getWorkingTimes()](#getWorkingTimes--) | Haalt het WorkingTimeCollection‑object op. |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Stelt een waarde in die aangeeft of de opgegeven datum of dagtype werkend is. |
| [setEnteredByOccurrences(boolean value)](#setEnteredByOccurrences-boolean-) | Stelt een waarde in die aangeeft of het bereik van herhaling wordt gedefinieerd door een aantal herhalingen in te voeren. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | Stelt het begin van de uitzonderingstijd in. |
| [setMonth(int value)](#setMonth-int-) | Stelt de maand in waarvoor een uitzonderingherhaling is gepland. |
| [setMonthDay(int value)](#setMonthDay-int-) | Stelt de dag van de maand in waarop een uitzonderingherhaling is gepland. |
| [setMonthItem(int value)](#setMonthItem-int-) | Stelt het maanditem in waarvoor een uitzonderingherhaling is gepland. |
| [setMonthPosition(int value)](#setMonthPosition-int-) | Stelt de positie van een maanditem binnen een maand in. |
| [setName(String value)](#setName-java.lang.String-) | Stelt de naam van de uitzondering in. |
| [setOccurrences(int value)](#setOccurrences-int-) | Stelt het aantal voorkomens in waarvoor de kalenderuitzondering geldig is. |
| [setPeriod(int value)](#setPeriod-int-) | Stelt de herhalingsperiode voor de uitzondering in. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | Stelt het einde van de uitzonderingstijd in. |
| [setType(int value)](#setType-int-) | Stelt het type van de uitzondering in. |
| [setWorkingTimes(WorkingTimeCollection value)](#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-) | Stelt het WorkingTimeCollection-object in. |
### CalendarException() {#CalendarException--}
```
public CalendarException()
```


Initialiseert een nieuw exemplaar van de [CalendarException](../../com.aspose.tasks/calendarexception) klasse.

### checkException(Date dt) {#checkException-java.util.Date-}
```
public final boolean checkException(Date dt)
```


Retourneert true als de opgegeven instantie van de java.util.Date struct de exceptiedag is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dt | java.util.Date | de opgegeven instantie van de java.util.Date-structuur. |

**Returns:**
boolean - Retourneert true als de java.util.Date-waarde de uitzonderingdag is; anders false.
### delete() {#delete--}
```
public final void delete()
```


Verwijdert de exceptie‑instantie uit het bovenliggende kalenderobject CalendarExceptionCollection.

### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Haalt een waarde op die aangeeft of de opgegeven datum of dagtype werkend is.

**Returns:**
boolean - een waarde die aangeeft of de opgegeven datum of dagtype werkend is.
### getDaysOfWeek() {#getDaysOfWeek--}
```
public final DayTypeCollection getDaysOfWeek()
```


Haalt de DayTypeCollection op voor dit object. De dagen van de week waarop de uitzondering geldig is.

**Returns:**
[DayTypeCollection](../../com.aspose.tasks/daytypecollection) - the DayTypeCollection for this object.
### getEnteredByOccurrences() {#getEnteredByOccurrences--}
```
public final boolean getEnteredByOccurrences()
```


Haalt een waarde op die aangeeft of het herhalingsbereik wordt gedefinieerd door een aantal voorkomens in te voeren. False geeft aan dat het herhalingsbereik wordt gedefinieerd door een einddatum in te voeren.

**Returns:**
boolean - een waarde die aangeeft of het herhalingsbereik wordt gedefinieerd door een aantal voorkomens in te voeren.
### getExceptionDates() {#getExceptionDates--}
```
public final Iterable<Date> getExceptionDates()
```


Retourneert data waarop de kalenderuitzondering van toepassing is.

**Returns:**
java.lang.Iterable&lt;java.util.Date&gt; - data waarop de kalenderuitzondering van toepassing is.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


Haalt het begin van de exceptietijd op.

**Returns:**
java.util.Date - het begin van de uitzonderingstijd.
### getMonth() {#getMonth--}
```
public final int getMonth()
```


Haalt de maand op waarvoor een exceptie‑herhaling is gepland.

**Returns:**
int - de maand waarvoor een uitzonderingherhaling is gepland.
### getMonthDay() {#getMonthDay--}
```
public final int getMonthDay()
```


Haalt de dag van de maand op waarop een exceptie‑herhaling is gepland.

**Returns:**
int - de dag van de maand waarop een uitzonderingherhaling is gepland.
### getMonthItem() {#getMonthItem--}
```
public final int getMonthItem()
```


Haalt het maanditem op waarvoor een exceptie‑herhaling is gepland.

**Returns:**
int - het maanditem waarvoor een uitzonderingherhaling is gepland.
### getMonthPosition() {#getMonthPosition--}
```
public final int getMonthPosition()
```


Haalt de positie van een maanditem binnen een maand op.

**Returns:**
int - de positie van een maanditem binnen een maand.
### getName() {#getName--}
```
public final String getName()
```


Haalt de naam van de exceptie op.

**Returns:**
java.lang.String - de naam van de uitzondering.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Haalt het aantal herhalingen op waarvoor de kalenderuitzondering geldig is.

**Returns:**
int - het aantal voorkomens waarvoor de kalenderuitzondering geldig is.
### getParentCalendar() {#getParentCalendar--}
```
public final Calendar getParentCalendar()
```


Haalt de bovenliggende agenda op voor dit object.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - the parent calendar for this object.
### getPeriod() {#getPeriod--}
```
public final int getPeriod()
```


Haalt de periode van herhaling voor de exceptie op.

**Returns:**
int - de herhalingsperiode voor de uitzondering.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


Haalt het einde van de exceptietijd op.

**Returns:**
java.util.Date - het einde van de uitzonderingstijd.
### getType() {#getType--}
```
public final int getType()
```


Haalt het type van de exceptie op.

**Returns:**
int - het type van de uitzondering.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Retourneert de werktijd voor een kalenderuitzondering.

**Returns:**
double - Retourneert de werktijd voor deze agenda-uitzondering.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


Haalt het WorkingTimeCollection-object op. De collectie werktijden die de op een weekdag gewerkte tijd definieert.

--------------------

Er moet ten minste één werktijd aanwezig zijn, en er mogen niet meer dan vijf zijn.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - the WorkingTimeCollection object.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Stelt een waarde in die aangeeft of de opgegeven datum of dagtype werkend is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de opgegeven datum of dagtype werkend is. |

### setEnteredByOccurrences(boolean value) {#setEnteredByOccurrences-boolean-}
```
public final void setEnteredByOccurrences(boolean value)
```


Stelt een waarde in die aangeeft of het herhalingsbereik wordt gedefinieerd door een aantal herhalingen in te voeren. False geeft aan dat het herhalingsbereik wordt gedefinieerd door een einddatum in te voeren.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of het herhalingsbereik wordt gedefinieerd door een aantal herhalingen in te voeren. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


Stelt het begin van de uitzonderingstijd in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | het begin van de uitzonderingstijd. |

### setMonth(int value) {#setMonth-int-}
```
public final void setMonth(int value)
```


Stelt de maand in waarvoor een uitzonderingherhaling is gepland.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de maand waarvoor een uitzonderingherhaling is gepland. |

### setMonthDay(int value) {#setMonthDay-int-}
```
public final void setMonthDay(int value)
```


Stelt de dag van de maand in waarop een uitzonderingherhaling is gepland.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de dag van de maand waarop een uitzonderingherhaling is gepland. |

### setMonthItem(int value) {#setMonthItem-int-}
```
public final void setMonthItem(int value)
```


Stelt het maanditem in waarvoor een uitzonderingherhaling is gepland.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het maandelement waarvoor een uitzonderingherhaling is gepland. |

### setMonthPosition(int value) {#setMonthPosition-int-}
```
public final void setMonthPosition(int value)
```


Stelt de positie van een maanditem binnen een maand in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de positie van een maandelement binnen een maand. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Stelt de naam van de uitzondering in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de naam van de uitzondering. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Stelt het aantal voorkomens in waarvoor de kalenderuitzondering geldig is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het aantal herhalingen waarvoor de agenda-uitzondering geldig is. |

### setPeriod(int value) {#setPeriod-int-}
```
public final void setPeriod(int value)
```


Stelt de herhalingsperiode voor de uitzondering in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de periode van herhaling voor de uitzondering. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


Stelt het einde van de uitzonderingstijd in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | het einde van de uitzonderingstijd. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Stelt het type van de uitzondering in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het type van de uitzondering. |

### setWorkingTimes(WorkingTimeCollection value) {#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-}
```
public final void setWorkingTimes(WorkingTimeCollection value)
```


Stelt het WorkingTimeCollection-object in. De collectie werktijden die de op een weekdag gewerkte tijd definieert.

--------------------

Er moet ten minste één werktijd aanwezig zijn, en er mogen niet meer dan vijf zijn.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) | het WorkingTimeCollection-object. |

