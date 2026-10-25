---
title: "RecurringTaskInfo"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar detaljerna för en återkommande uppgift i ett projekt."
type: docs
weight: 244
url: /sv/java/com.aspose.tasks/recurringtaskinfo/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskInfo
```

Representerar detaljerna för en återkommande uppgift i ett projekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getDailyRepetitions()](#getDailyRepetitions--) | Hämtar antalet upprepningar för det dagliga återkomstande mönstret. |
| [getDailyUseWorkdays()](#getDailyUseWorkdays--) | Hämtar ett värde som indikerar om arbetsdagar ska användas för det dagliga återkomstande mönstret. |
| [getDuration()](#getDuration--) | Hämtar varaktigheten för en förekomst av den återkommande uppgiften. |
| [getEndDate()](#getEndDate--) | Hämtar datumet då förekomsterna ska avslutas. |
| [getMonthlyDay()](#getMonthlyDay--) | Hämtar antalet dagar för det månatliga återkomstande mönstret. |
| [getMonthlyOrdinalDay()](#getMonthlyOrdinalDay--) | Hämtar en dag i det månatliga återkomstande mönstret när ordinal dag används. |
| [getMonthlyOrdinalNumber()](#getMonthlyOrdinalNumber--) | Hämtar ett ordinalt tal för det månatliga återkomstande mönstret. |
| [getMonthlyOrdinalRepetitions()](#getMonthlyOrdinalRepetitions--) | Hämtar antalet upprepningar för det månatliga återkomstande mönstret när ordinal dag används. |
| [getMonthlyRepetitions()](#getMonthlyRepetitions--) | Hämtar antalet upprepningar för det månatliga återkomstande mönstret. |
| [getMonthlyUseOrdinalDay()](#getMonthlyUseOrdinalDay--) | Hämtar ett värde som indikerar om ordinal dag ska användas för det månatliga återkomstande mönstret. |
| [getOccurrences()](#getOccurrences--) | Hämtar ett antal förekomster av den återkommande uppgiften. |
| [getRecurrencePattern()](#getRecurrencePattern--) | Hämtar ett återkomstande mönster för den återkommande uppgiften. |
| [getStartDate()](#getStartDate--) | Hämtar datumet då förekomsterna ska börja. |
| [getTask()](#getTask--) | Hämtar föräldrauppgiften för detta exempel av klassen [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo). |
| [getUseEndDate()](#getUseEndDate--) | Hämtar ett värde som anger om slutdatumet eller ett antal förekomster ska användas för den återkommande uppgiften. |
| [getWeeklyDays()](#getWeeklyDays--) | Hämtar en samling dagar som används i det veckovisa återkomstande mönstret. |
| [getWeeklyRepetitions()](#getWeeklyRepetitions--) | Hämtar ett antal upprepningar för det veckovisa återkomstande mönstret. |
| [getYearlyDate()](#getYearlyDate--) | Hämtar ett datum för det årliga återkomstande mönstret. |
| [getYearlyOrdinalDay()](#getYearlyOrdinalDay--) | Hämtar en veckodag för det årliga återkomstande mönstret när ordinal dag används. |
| [getYearlyOrdinalMonth()](#getYearlyOrdinalMonth--) | Hämtar en månad för det årliga återkomstande mönstret när ordinal dag används. |
| [getYearlyOrdinalNumber()](#getYearlyOrdinalNumber--) | Hämtar ett ordinaltal för det årliga återkomstande mönstret. |
| [getYearlyUseOrdinalDay()](#getYearlyUseOrdinalDay--) | Hämtar ett värde som anger om ordinal dag ska användas för det årliga återkomstande mönstret. |
| [setDailyRepetitions(int value)](#setDailyRepetitions-int-) | Ställer in ett antal upprepningar för det dagliga återkomstande mönstret. |
| [setDailyUseWorkdays(boolean value)](#setDailyUseWorkdays-boolean-) | Ställer in ett värde som anger om arbetsdagar ska användas för det dagliga återkomstande mönstret. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Ställer in varaktigheten för en förekomst av den återkommande uppgiften. |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Ställer in datumet då förekomsterna ska avslutas. |
| [setMonthlyDay(int value)](#setMonthlyDay-int-) | Ställer in ett antal dagar för det månatliga återkomstande mönstret. |
| [setMonthlyOrdinalDay(int value)](#setMonthlyOrdinalDay-int-) | Ställer in en dag för det månatliga återkomstande mönstret när ordinal dag används. |
| [setMonthlyOrdinalNumber(int value)](#setMonthlyOrdinalNumber-int-) | Ställer in ett ordinaltal för det månatliga återkomstande mönstret. |
| [setMonthlyOrdinalRepetitions(int value)](#setMonthlyOrdinalRepetitions-int-) | Ställer in ett antal upprepningar för det månatliga återkomstande mönstret när ordinal dag används. |
| [setMonthlyRepetitions(int value)](#setMonthlyRepetitions-int-) | Ställer in ett antal upprepningar för det månatliga återkomstande mönstret. |
| [setMonthlyUseOrdinalDay(boolean value)](#setMonthlyUseOrdinalDay-boolean-) | Ställer in ett värde som anger om ordinal dag ska användas för det månatliga återkomstande mönstret. |
| [setOccurrences(int value)](#setOccurrences-int-) | Ställer in ett antal förekomster av den återkommande uppgiften. |
| [setRecurrencePattern(int value)](#setRecurrencePattern-int-) | Ställer in ett återkomstande mönster för den återkommande uppgiften. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Ställer in datumet då förekomsterna ska börja. |
| [setUseEndDate(boolean value)](#setUseEndDate-boolean-) | Ställer in ett värde som anger om slutdatum eller ett antal förekomster ska användas för den återkommande uppgiften. |
| [setWeeklyDays(int value)](#setWeeklyDays-int-) | Ställer in en samling av dagar som används i det veckovisa återkommande mönstret. |
| [setWeeklyRepetitions(int value)](#setWeeklyRepetitions-int-) | Ställer in ett antal upprepningar för det veckovisa återkommande mönstret. |
| [setYearlyDate(Date value)](#setYearlyDate-java.util.Date-) | Ställer in ett datum för det årliga återkommande mönstret. |
| [setYearlyOrdinalDay(int value)](#setYearlyOrdinalDay-int-) | Ställer in en veckodag för det årliga återkommande mönstret när ordinal dag används. |
| [setYearlyOrdinalMonth(int value)](#setYearlyOrdinalMonth-int-) | Ställer in en månad för det årliga återkommande mönstret när ordinal dag används. |
| [setYearlyOrdinalNumber(int value)](#setYearlyOrdinalNumber-int-) | Ställer in ett ordinalt tal för det årliga återkommande mönstret. |
| [setYearlyUseOrdinalDay(boolean value)](#setYearlyUseOrdinalDay-boolean-) | Ställer in ett värde som anger om ordinal dag ska användas för det årliga återkommande mönstret. |
### getDailyRepetitions() {#getDailyRepetitions--}
```
public final int getDailyRepetitions()
```


Hämtar antalet upprepningar för det dagliga återkomstande mönstret.

**Returns:**
int - ett antal upprepningar för det dagliga återkommande mönstret.
### getDailyUseWorkdays() {#getDailyUseWorkdays--}
```
public final boolean getDailyUseWorkdays()
```


Hämtar ett värde som indikerar om arbetsdagar ska användas för det dagliga återkomstande mönstret.

**Returns:**
boolean - ett värde som anger om arbetsdagar ska användas för det dagliga återkommande mönstret.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Hämtar varaktigheten för en förekomst av den återkommande uppgiften.

--------------------

instansen av `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)) klass.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration for one occurrence of the recurring task.
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Hämtar datumet då förekomsterna ska avslutas.

**Returns:**
java.util.Date - datumet för när förekomsterna ska avslutas.
### getMonthlyDay() {#getMonthlyDay--}
```
public final int getMonthlyDay()
```


Hämtar antalet dagar för det månatliga återkomstande mönstret.

**Returns:**
int - ett antal dagar för det månatliga återkommande mönstret.
### getMonthlyOrdinalDay() {#getMonthlyOrdinalDay--}
```
public final int getMonthlyOrdinalDay()
```


Hämtar en dag i det månatliga återkomstande mönstret när ordinal dag används.

--------------------

Kan vara ett av värdena i [DayOfWeek](../../com.aspose.tasks/dayofweek) enumeration.

**Returns:**
int - en dag i det månatliga återkommande mönstret när ordinal dag används.
### getMonthlyOrdinalNumber() {#getMonthlyOrdinalNumber--}
```
public final int getMonthlyOrdinalNumber()
```


Hämtar ett ordinalt tal för det månatliga återkomstande mönstret.

--------------------

Kan vara ett av värdena i [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumeration.

**Returns:**
int - ett ordinalt tal för det månatliga återkommande mönstret.
### getMonthlyOrdinalRepetitions() {#getMonthlyOrdinalRepetitions--}
```
public final int getMonthlyOrdinalRepetitions()
```


Hämtar antalet upprepningar för det månatliga återkomstande mönstret när ordinal dag används.

**Returns:**
int - ett antal upprepningar för det månatliga återkommande mönstret när ordinal dag används.
### getMonthlyRepetitions() {#getMonthlyRepetitions--}
```
public final int getMonthlyRepetitions()
```


Hämtar antalet upprepningar för det månatliga återkomstande mönstret.

**Returns:**
int - ett antal upprepningar för det månatliga återkommande mönstret.
### getMonthlyUseOrdinalDay() {#getMonthlyUseOrdinalDay--}
```
public final boolean getMonthlyUseOrdinalDay()
```


Hämtar ett värde som indikerar om ordinal dag ska användas för det månatliga återkomstande mönstret.

**Returns:**
boolean - ett värde som anger om ordinal dag ska användas för det månatliga återkommande mönstret.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Hämtar ett antal förekomster av den återkommande uppgiften.

**Returns:**
int - ett antal förekomster av den återkommande uppgiften.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final int getRecurrencePattern()
```


Hämtar ett återkomstande mönster för den återkommande uppgiften.

--------------------

Kan vara ett av värdena i `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)) enumeration.

**Returns:**
int - ett återkomstmönster för den återkommande uppgiften.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Hämtar datumet då förekomsterna ska börja.

**Returns:**
java.util.Date - datumet för när förekomsterna ska börja.
### getTask() {#getTask--}
```
public final Task getTask()
```


Hämtar föräldrauppgiften för detta exempel av klassen [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo).

**Returns:**
[Task](../../com.aspose.tasks/task) - the parent task of this instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class.
### getUseEndDate() {#getUseEndDate--}
```
public final boolean getUseEndDate()
```


Hämtar ett värde som anger om slutdatumet eller ett antal förekomster ska användas för den återkommande uppgiften.

**Returns:**
boolean - ett värde som anger om slutdatum eller ett antal förekomster ska användas för den återkommande uppgiften.
### getWeeklyDays() {#getWeeklyDays--}
```
public final int getWeeklyDays()
```


Hämtar en samling dagar som används i det veckovisa återkomstande mönstret.

--------------------

**Returns:**
int - en samling dagar som används i det veckovisa återkommande mönstret.
### getWeeklyRepetitions() {#getWeeklyRepetitions--}
```
public final int getWeeklyRepetitions()
```


Hämtar ett antal upprepningar för det veckovisa återkomstande mönstret.

**Returns:**
int - ett antal upprepningar för det veckovisa återkommande mönstret.
### getYearlyDate() {#getYearlyDate--}
```
public final Date getYearlyDate()
```


Hämtar ett datum för det årliga återkomstande mönstret.

**Returns:**
java.util.Date - ett datum för det årliga återkommande mönstret.
### getYearlyOrdinalDay() {#getYearlyOrdinalDay--}
```
public final int getYearlyOrdinalDay()
```


Hämtar en veckodag för det årliga återkomstande mönstret när ordinal dag används.

--------------------

Kan vara ett av värdena i [DayOfWeek](../../com.aspose.tasks/dayofweek) enumeration.

**Returns:**
int - en veckodag för det årliga återkommande mönstret när ordinal dag används.
### getYearlyOrdinalMonth() {#getYearlyOrdinalMonth--}
```
public final int getYearlyOrdinalMonth()
```


Hämtar en månad för det årliga återkomstande mönstret när ordinal dag används.

--------------------

Kan vara ett av värdena i [Month](../../com.aspose.tasks/month)-enumerationen.

**Returns:**
int - en månad för det årliga återkommande mönstret när ordinal dag används.
### getYearlyOrdinalNumber() {#getYearlyOrdinalNumber--}
```
public final int getYearlyOrdinalNumber()
```


Hämtar ett ordinaltal för det årliga återkomstande mönstret.

--------------------

Kan vara ett av värdena i [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumeration.

**Returns:**
int - ett ordinalt tal för det årliga återkommande mönstret.
### getYearlyUseOrdinalDay() {#getYearlyUseOrdinalDay--}
```
public final boolean getYearlyUseOrdinalDay()
```


Hämtar ett värde som anger om ordinal dag ska användas för det årliga återkomstande mönstret.

**Returns:**
boolean - ett värde som anger om ordinal dag ska användas för det årliga återkommande mönstret.
### setDailyRepetitions(int value) {#setDailyRepetitions-int-}
```
public final void setDailyRepetitions(int value)
```


Ställer in ett antal upprepningar för det dagliga återkomstande mönstret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett antal upprepningar för det dagliga återkommande mönstret. |

### setDailyUseWorkdays(boolean value) {#setDailyUseWorkdays-boolean-}
```
public final void setDailyUseWorkdays(boolean value)
```


Ställer in ett värde som anger om arbetsdagar ska användas för det dagliga återkomstande mönstret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som anger om arbetsdagar ska användas för det dagliga återkommande mönstret. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Ställer in varaktigheten för en förekomst av den återkommande uppgiften.

--------------------

instansen av `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)) klass.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | varaktigheten för en förekomst av den återkommande uppgiften. |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Ställer in datumet då förekomsterna ska avslutas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | datumet då förekomsterna ska avslutas. |

### setMonthlyDay(int value) {#setMonthlyDay-int-}
```
public final void setMonthlyDay(int value)
```


Ställer in ett antal dagar för det månatliga återkomstande mönstret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett antal dagar för det månatliga återkommande mönstret. |

### setMonthlyOrdinalDay(int value) {#setMonthlyOrdinalDay-int-}
```
public final void setMonthlyOrdinalDay(int value)
```


Ställer in en dag för det månatliga återkomstande mönstret när ordinal dag används.

--------------------

Kan vara ett av värdena i [DayOfWeek](../../com.aspose.tasks/dayofweek) enumeration.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | en dag i det månatliga återkommande mönstret när ordinal dag används. |

### setMonthlyOrdinalNumber(int value) {#setMonthlyOrdinalNumber-int-}
```
public final void setMonthlyOrdinalNumber(int value)
```


Ställer in ett ordinaltal för det månatliga återkomstande mönstret.

--------------------

Kan vara ett av värdena i [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumeration.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett ordinalt tal för det månatliga återkommande mönstret. |

### setMonthlyOrdinalRepetitions(int value) {#setMonthlyOrdinalRepetitions-int-}
```
public final void setMonthlyOrdinalRepetitions(int value)
```


Ställer in ett antal upprepningar för det månatliga återkomstande mönstret när ordinal dag används.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett antal upprepningar för det månatliga återkommande mönstret när ordinal dag används. |

### setMonthlyRepetitions(int value) {#setMonthlyRepetitions-int-}
```
public final void setMonthlyRepetitions(int value)
```


Ställer in ett antal upprepningar för det månatliga återkomstande mönstret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett antal upprepningar för det månatliga återkommande mönstret. |

### setMonthlyUseOrdinalDay(boolean value) {#setMonthlyUseOrdinalDay-boolean-}
```
public final void setMonthlyUseOrdinalDay(boolean value)
```


Ställer in ett värde som anger om ordinal dag ska användas för det månatliga återkomstande mönstret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som anger om ordinal dag ska användas för det månatliga återkommande mönstret. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Ställer in ett antal förekomster av den återkommande uppgiften.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett antal förekomster av den återkommande uppgiften. |

### setRecurrencePattern(int value) {#setRecurrencePattern-int-}
```
public final void setRecurrencePattern(int value)
```


Ställer in ett återkomstande mönster för den återkommande uppgiften.

--------------------

Kan vara ett av värdena i `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)) enumeration.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett återkommande mönster för den återkommande uppgiften. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Ställer in datumet då förekomsterna ska börja.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | datumet då förekomsterna ska börja. |

### setUseEndDate(boolean value) {#setUseEndDate-boolean-}
```
public final void setUseEndDate(boolean value)
```


Ställer in ett värde som anger om slutdatum eller ett antal förekomster ska användas för den återkommande uppgiften.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som anger om slutdatum eller ett antal förekomster ska användas för den återkommande uppgiften. |

### setWeeklyDays(int value) {#setWeeklyDays-int-}
```
public final void setWeeklyDays(int value)
```


Ställer in en samling av dagar som används i det veckovisa återkommande mönstret.

--------------------

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | en samling dagar som används i det veckovisa återkommande mönstret. |

### setWeeklyRepetitions(int value) {#setWeeklyRepetitions-int-}
```
public final void setWeeklyRepetitions(int value)
```


Ställer in ett antal upprepningar för det veckovisa återkommande mönstret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett antal upprepningar för det veckovisa återkommande mönstret. |

### setYearlyDate(Date value) {#setYearlyDate-java.util.Date-}
```
public final void setYearlyDate(Date value)
```


Ställer in ett datum för det årliga återkommande mönstret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | ett datum för det årliga återkommande mönstret. |

### setYearlyOrdinalDay(int value) {#setYearlyOrdinalDay-int-}
```
public final void setYearlyOrdinalDay(int value)
```


Ställer in en veckodag för det årliga återkommande mönstret när ordinal dag används.

--------------------

Kan vara ett av värdena i [DayOfWeek](../../com.aspose.tasks/dayofweek) enumeration.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | en veckodag i det årliga återkomstmönstret när ordinal dag används. |

### setYearlyOrdinalMonth(int value) {#setYearlyOrdinalMonth-int-}
```
public final void setYearlyOrdinalMonth(int value)
```


Ställer in en månad för det årliga återkommande mönstret när ordinal dag används.

--------------------

Kan vara ett av värdena i [Month](../../com.aspose.tasks/month)-enumerationen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | en månad i det årliga återkomstmönstret när ordinal dag används. |

### setYearlyOrdinalNumber(int value) {#setYearlyOrdinalNumber-int-}
```
public final void setYearlyOrdinalNumber(int value)
```


Ställer in ett ordinalt tal för det årliga återkommande mönstret.

--------------------

Kan vara ett av värdena i [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumeration.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett ordinaltal i det årliga återkomstmönstret. |

### setYearlyUseOrdinalDay(boolean value) {#setYearlyUseOrdinalDay-boolean-}
```
public final void setYearlyUseOrdinalDay(boolean value)
```


Ställer in ett värde som anger om ordinal dag ska användas för det årliga återkommande mönstret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om ordinal dag ska användas för det årliga återkomstmönstret. |

