---
title: "CalendarException"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar exceptionella tidsperioder i en kalender."
type: docs
weight: 43
url: /sv/java/com.aspose.tasks/calendarexception/
---

**Inheritance:**
java.lang.Object
```
public final class CalendarException
```

Representerar exceptionella tidsperioder i en kalender.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [CalendarException()](#CalendarException--) | Initierar en ny instans av klassen [CalendarException](../../com.aspose.tasks/calendarexception). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [checkException(Date dt)](#checkException-java.util.Date-) | Returnerar true om den angivna instansen av java.util.Date‑strukturen är undantagsdagen. |
| [delete()](#delete--) | Tar bort Exception‑instansen från föräldrakalenderns CalendarExceptionCollection‑objekt. |
| [getDayWorking()](#getDayWorking--) | Hämtar ett värde som indikerar om det angivna datumet eller dagtypen är arbetsdag. |
| [getDaysOfWeek()](#getDaysOfWeek--) | Hämtar DayTypeCollection för detta objekt. |
| [getEnteredByOccurrences()](#getEnteredByOccurrences--) | Hämtar ett värde som indikerar om återkommande intervallet definieras genom att ange ett antal förekomster. |
| [getExceptionDates()](#getExceptionDates--) | Returnerar datum då kalenderundantaget är tillämpligt. |
| [getFromDate()](#getFromDate--) | Hämtar början av undantagstiden. |
| [getMonth()](#getMonth--) | Hämtar månaden för vilken ett undantagsåterkommande är schemalagt. |
| [getMonthDay()](#getMonthDay--) | Hämtar dagen i månaden då ett undantagsåterkommande är schemalagt. |
| [getMonthItem()](#getMonthItem--) | Hämtar månadsposten för vilken ett undantagsåterkommande är schemalagt. |
| [getMonthPosition()](#getMonthPosition--) | Hämtar positionen för en månadspost inom en månad. |
| [getName()](#getName--) | Hämtar namnet på undantaget. |
| [getOccurrences()](#getOccurrences--) | Hämtar antalet förekomster som kalenderundantaget är giltigt för. |
| [getParentCalendar()](#getParentCalendar--) | Hämtar föräldrakalendern för detta objekt. |
| [getPeriod()](#getPeriod--) | Hämtar återkommande perioden för undantaget. |
| [getToDate()](#getToDate--) | Hämtar slutet på undantagstiden. |
| [getType()](#getType--) | Hämtar undantagstypen. |
| [getWorkingTime()](#getWorkingTime--) | Returnerar arbetstiden för ett kalenderundantag. |
| [getWorkingTimes()](#getWorkingTimes--) | Hämtar WorkingTimeCollection-objektet. |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Ställer in ett värde som indikerar om det angivna datumet eller dagtypen är arbetsdag. |
| [setEnteredByOccurrences(boolean value)](#setEnteredByOccurrences-boolean-) | Ställer in ett värde som indikerar om återkommande intervallet definieras genom att ange ett antal förekomster. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | Ställer in början av undantagstiden. |
| [setMonth(int value)](#setMonth-int-) | Ställer in månaden för vilken ett undantagsåterkommande är schemalagt. |
| [setMonthDay(int value)](#setMonthDay-int-) | Ställer in dagen i månaden då ett undantagsåterkommande är schemalagt. |
| [setMonthItem(int value)](#setMonthItem-int-) | Ställer in månadselementet för vilket ett undantagsåterkommande är schemalagt. |
| [setMonthPosition(int value)](#setMonthPosition-int-) | Ställer in positionen för ett månadselement inom en månad. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in namnet på undantaget. |
| [setOccurrences(int value)](#setOccurrences-int-) | Ställer in antalet förekomster som kalenderundantaget är giltigt för. |
| [setPeriod(int value)](#setPeriod-int-) | Ställer in återkommande perioden för undantaget. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | Ställer in slutet på undantagstiden. |
| [setType(int value)](#setType-int-) | Ställer in undantagstypen. |
| [setWorkingTimes(WorkingTimeCollection value)](#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-) | Ställer in WorkingTimeCollection-objektet. |
### CalendarException() {#CalendarException--}
```
public CalendarException()
```


Initierar en ny instans av klassen [CalendarException](../../com.aspose.tasks/calendarexception).

### checkException(Date dt) {#checkException-java.util.Date-}
```
public final boolean checkException(Date dt)
```


Returnerar true om den angivna instansen av java.util.Date‑strukturen är undantagsdagen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dt | java.util.Date | den angivna instansen av java.util.Date-strukturen. |

**Returns:**
boolean - Returnerar true om java.util.Date-värdet är undantagsdagen; annars false.
### delete() {#delete--}
```
public final void delete()
```


Tar bort Exception‑instansen från föräldrakalenderns CalendarExceptionCollection‑objekt.

### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Hämtar ett värde som indikerar om det angivna datumet eller dagtypen är arbetsdag.

**Returns:**
boolean - ett värde som indikerar om det angivna datumet eller dagtypen är arbetsdag.
### getDaysOfWeek() {#getDaysOfWeek--}
```
public final DayTypeCollection getDaysOfWeek()
```


Hämtar DayTypeCollection för detta objekt. Veckodagarna då undantaget är giltigt.

**Returns:**
[DayTypeCollection](../../com.aspose.tasks/daytypecollection) - the DayTypeCollection for this object.
### getEnteredByOccurrences() {#getEnteredByOccurrences--}
```
public final boolean getEnteredByOccurrences()
```


Hämtar ett värde som indikerar om återkommande intervallet definieras genom att ange ett antal förekomster. False anger att återkommande intervallet definieras genom att ange ett slutdatum.

**Returns:**
boolean - ett värde som indikerar om återkommande intervallet definieras genom att ange ett antal förekomster.
### getExceptionDates() {#getExceptionDates--}
```
public final Iterable<Date> getExceptionDates()
```


Returnerar datum då kalenderundantaget är tillämpligt.

**Returns:**
java.lang.Iterable&lt;java.util.Date&gt; - datum då kalenderundantaget är tillämpligt.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


Hämtar början av undantagstiden.

**Returns:**
java.util.Date - början av undantagstiden.
### getMonth() {#getMonth--}
```
public final int getMonth()
```


Hämtar månaden för vilken ett undantagsåterkommande är schemalagt.

**Returns:**
int - den månad för vilken en undantagsupprepning är schemalagd.
### getMonthDay() {#getMonthDay--}
```
public final int getMonthDay()
```


Hämtar dagen i månaden då ett undantagsåterkommande är schemalagt.

**Returns:**
int - den dag i en månad då en undantagsupprepning är schemalagd.
### getMonthItem() {#getMonthItem--}
```
public final int getMonthItem()
```


Hämtar månadsposten för vilken ett undantagsåterkommande är schemalagt.

**Returns:**
int - det månadselement som en undantagsupprepning är schemalagd för.
### getMonthPosition() {#getMonthPosition--}
```
public final int getMonthPosition()
```


Hämtar positionen för en månadspost inom en månad.

**Returns:**
int - positionen för ett månadselement inom en månad.
### getName() {#getName--}
```
public final String getName()
```


Hämtar namnet på undantaget.

**Returns:**
java.lang.String - namnet på undantaget.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Hämtar antalet förekomster som kalenderundantaget är giltigt för.

**Returns:**
int - antalet förekomster som kalenderundantaget är giltigt för.
### getParentCalendar() {#getParentCalendar--}
```
public final Calendar getParentCalendar()
```


Hämtar föräldrakalendern för detta objekt.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - the parent calendar for this object.
### getPeriod() {#getPeriod--}
```
public final int getPeriod()
```


Hämtar återkommande perioden för undantaget.

**Returns:**
int - återkommande period för undantaget.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


Hämtar slutet på undantagstiden.

**Returns:**
java.util.Date - slutet av undantagstiden.
### getType() {#getType--}
```
public final int getType()
```


Hämtar undantagstypen.

**Returns:**
int - undantagstypen.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Returnerar arbetstiden för ett kalenderundantag.

**Returns:**
double - Returnerar arbetstid för detta kalenderundantag.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


Hämtar WorkingTimeCollection-objektet. Samlingen av arbetstider som definierar den tid som arbetas på veckodagen.

--------------------

Minst en arbetstid måste finnas, och det kan inte vara fler än fem.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - the WorkingTimeCollection object.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Ställer in ett värde som indikerar om det angivna datumet eller dagtypen är arbetsdag.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om det angivna datumet eller dagtypen är arbetsdag. |

### setEnteredByOccurrences(boolean value) {#setEnteredByOccurrences-boolean-}
```
public final void setEnteredByOccurrences(boolean value)
```


Ställer in ett värde som indikerar om återkommande intervall definieras genom att ange ett antal förekomster. False betyder att återkommande intervall definieras genom att ange ett slutdatum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om återkommande intervall definieras genom att ange ett antal förekomster. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


Ställer in början av undantagstiden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | början av undantagstiden. |

### setMonth(int value) {#setMonth-int-}
```
public final void setMonth(int value)
```


Ställer in månaden för vilken ett undantagsåterkommande är schemalagt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | den månad för vilken en undantagsupprepning är schemalagd. |

### setMonthDay(int value) {#setMonthDay-int-}
```
public final void setMonthDay(int value)
```


Ställer in dagen i månaden då ett undantagsåterkommande är schemalagt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | den dag i en månad då en undantagsupprepning är schemalagd. |

### setMonthItem(int value) {#setMonthItem-int-}
```
public final void setMonthItem(int value)
```


Ställer in månadselementet för vilket ett undantagsåterkommande är schemalagt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | det månadselement som en undantagsupprepning är schemalagd för. |

### setMonthPosition(int value) {#setMonthPosition-int-}
```
public final void setMonthPosition(int value)
```


Ställer in positionen för ett månadselement inom en månad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | positionen för ett månadselement inom en månad. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Ställer in namnet på undantaget.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | namnet på undantaget. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Ställer in antalet förekomster som kalenderundantaget är giltigt för.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | antalet förekomster som kalenderundantaget är giltigt för. |

### setPeriod(int value) {#setPeriod-int-}
```
public final void setPeriod(int value)
```


Ställer in återkommande perioden för undantaget.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | återkommande period för undantaget. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


Ställer in slutet på undantagstiden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | slutet av undantagstiden. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Ställer in undantagstypen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | undantagstypen. |

### setWorkingTimes(WorkingTimeCollection value) {#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-}
```
public final void setWorkingTimes(WorkingTimeCollection value)
```


Ställer in WorkingTimeCollection-objektet. Samlingen av arbetstider som definierar den arbetade tiden på veckodagen.

--------------------

Minst en arbetstid måste finnas, och det kan inte vara fler än fem.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) | WorkingTimeCollection-objektet. |

