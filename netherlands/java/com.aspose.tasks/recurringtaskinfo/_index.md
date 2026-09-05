---
title: "RecurringTaskInfo"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt de details van een terugkerende taak in een project voor."
type: docs
weight: 244
url: /nl/java/com.aspose.tasks/recurringtaskinfo/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskInfo
```

Stelt de details van een terugkerende taak in een project voor.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getDailyRepetitions()](#getDailyRepetitions--) | Haalt een aantal herhalingen op voor het dagelijkse terugkeerpatroon. |
| [getDailyUseWorkdays()](#getDailyUseWorkdays--) | Haalt een waarde op die aangeeft of werkdagen moeten worden gebruikt voor het dagelijkse terugkeerpatroon. |
| [getDuration()](#getDuration--) | Haalt de duur op voor één optreden van de terugkerende taak. |
| [getEndDate()](#getEndDate--) | Haalt de datum op waarop de optredens eindigen. |
| [getMonthlyDay()](#getMonthlyDay--) | Haalt een aantal dagen op van het maandelijkse terugkeerpatroon. |
| [getMonthlyOrdinalDay()](#getMonthlyOrdinalDay--) | Haalt een dag op van het maandelijkse terugkeerpatroon bij gebruik van een rangorde-dag. |
| [getMonthlyOrdinalNumber()](#getMonthlyOrdinalNumber--) | Haalt een rangordegetal op van het maandelijkse terugkeerpatroon. |
| [getMonthlyOrdinalRepetitions()](#getMonthlyOrdinalRepetitions--) | Haalt een aantal herhalingen op voor het maandelijkse terugkeerpatroon bij gebruik van een rangorde-dag. |
| [getMonthlyRepetitions()](#getMonthlyRepetitions--) | Haalt een aantal herhalingen op voor het maandelijkse terugkeerpatroon. |
| [getMonthlyUseOrdinalDay()](#getMonthlyUseOrdinalDay--) | Haalt een waarde op die aangeeft of een rangorde-dag moet worden gebruikt voor het maandelijkse terugkeerpatroon. |
| [getOccurrences()](#getOccurrences--) | Haalt een aantal optredens op van de terugkerende taak. |
| [getRecurrencePattern()](#getRecurrencePattern--) | Haalt een terugkeerpatroon op van de terugkerende taak. |
| [getStartDate()](#getStartDate--) | Haalt de datum op waarop de optredens beginnen. |
| [getTask()](#getTask--) | Haalt de bovenliggende taak op van deze instantie van de klasse [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo). |
| [getUseEndDate()](#getUseEndDate--) | Haalt een waarde op die aangeeft of de einddatum of een aantal optredens moet worden gebruikt voor de terugkerende taak. |
| [getWeeklyDays()](#getWeeklyDays--) | Haalt een verzameling dagen op die worden gebruikt in het wekelijkse terugkeerpatroon. |
| [getWeeklyRepetitions()](#getWeeklyRepetitions--) | Haalt een aantal herhalingen op voor het wekelijkse terugkeerpatroon. |
| [getYearlyDate()](#getYearlyDate--) | Haalt een datum op voor het jaarlijkse terugkeerpatroon. |
| [getYearlyOrdinalDay()](#getYearlyOrdinalDay--) | Haalt een weekdag op van het jaarlijkse terugkeerpatroon bij gebruik van een ordinale dag. |
| [getYearlyOrdinalMonth()](#getYearlyOrdinalMonth--) | Haalt een maand op van het jaarlijkse terugkeerpatroon bij gebruik van een ordinale dag. |
| [getYearlyOrdinalNumber()](#getYearlyOrdinalNumber--) | Haalt een ordinaal getal op van het jaarlijkse terugkeerpatroon. |
| [getYearlyUseOrdinalDay()](#getYearlyUseOrdinalDay--) | Haalt een waarde op die aangeeft of een ordinale dag moet worden gebruikt voor het jaarlijkse terugkeerpatroon. |
| [setDailyRepetitions(int value)](#setDailyRepetitions-int-) | Stelt een aantal herhalingen in voor het dagelijkse terugkeerpatroon. |
| [setDailyUseWorkdays(boolean value)](#setDailyUseWorkdays-boolean-) | Stelt een waarde in die aangeeft of werkdagen moeten worden gebruikt voor het dagelijkse terugkeerpatroon. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Stelt de duur in voor één gebeurtenis van de terugkerende taak. |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Stelt de datum in waarop de gebeurtenissen eindigen. |
| [setMonthlyDay(int value)](#setMonthlyDay-int-) | Stelt een dagnummer in van het maandelijkse terugkeerpatroon. |
| [setMonthlyOrdinalDay(int value)](#setMonthlyOrdinalDay-int-) | Stelt een dag in van het maandelijkse terugkeerpatroon bij gebruik van een ordinale dag. |
| [setMonthlyOrdinalNumber(int value)](#setMonthlyOrdinalNumber-int-) | Stelt een ordinaal getal in van het maandelijkse terugkeerpatroon. |
| [setMonthlyOrdinalRepetitions(int value)](#setMonthlyOrdinalRepetitions-int-) | Stelt een aantal herhalingen in voor het maandelijkse terugkeerpatroon bij gebruik van een ordinale dag. |
| [setMonthlyRepetitions(int value)](#setMonthlyRepetitions-int-) | Stelt een aantal herhalingen in voor het maandelijkse terugkeerpatroon. |
| [setMonthlyUseOrdinalDay(boolean value)](#setMonthlyUseOrdinalDay-boolean-) | Stelt een waarde in die aangeeft of een ordinale dag moet worden gebruikt voor het maandelijkse terugkeerpatroon. |
| [setOccurrences(int value)](#setOccurrences-int-) | Stelt een aantal gebeurtenissen in van de terugkerende taak. |
| [setRecurrencePattern(int value)](#setRecurrencePattern-int-) | Stelt een terugkeerpatroon in van de terugkerende taak. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Stelt de datum in waarop de gebeurtenissen beginnen. |
| [setUseEndDate(boolean value)](#setUseEndDate-boolean-) | Stelt een waarde in die aangeeft of de einddatum of een aantal gebeurtenissen moet worden gebruikt voor de terugkerende taak. |
| [setWeeklyDays(int value)](#setWeeklyDays-int-) | Stelt een verzameling dagen in die worden gebruikt in het wekelijkse terugkeerpatroon. |
| [setWeeklyRepetitions(int value)](#setWeeklyRepetitions-int-) | Stelt een aantal herhalingen in voor het wekelijkse terugkeerpatroon. |
| [setYearlyDate(Date value)](#setYearlyDate-java.util.Date-) | Stelt een datum in voor het jaarlijkse terugkeerpatroon. |
| [setYearlyOrdinalDay(int value)](#setYearlyOrdinalDay-int-) | Stelt een weekdag in van het jaarlijkse terugkeerpatroon bij gebruik van een ordinale dag. |
| [setYearlyOrdinalMonth(int value)](#setYearlyOrdinalMonth-int-) | Stelt een maand in van het jaarlijkse terugkeerpatroon bij gebruik van een ordinale dag. |
| [setYearlyOrdinalNumber(int value)](#setYearlyOrdinalNumber-int-) | Stelt een ordinaal getal in van het jaarlijkse terugkeerpatroon. |
| [setYearlyUseOrdinalDay(boolean value)](#setYearlyUseOrdinalDay-boolean-) | Stelt een waarde in die aangeeft of een ordinale dag moet worden gebruikt voor het jaarlijkse terugkeerpatroon. |
### getDailyRepetitions() {#getDailyRepetitions--}
```
public final int getDailyRepetitions()
```


Haalt een aantal herhalingen op voor het dagelijkse terugkeerpatroon.

**Returns:**
int - een aantal herhalingen voor het dagelijkse terugkeerpatroon.
### getDailyUseWorkdays() {#getDailyUseWorkdays--}
```
public final boolean getDailyUseWorkdays()
```


Haalt een waarde op die aangeeft of werkdagen moeten worden gebruikt voor het dagelijkse terugkeerpatroon.

**Returns:**
boolean - een waarde die aangeeft of werkdagen gebruikt moeten worden voor het dagelijkse terugkeerpatroon.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Haalt de duur op voor één optreden van de terugkerende taak.

--------------------

de instantie van `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)) klasse.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration for one occurrence of the recurring task.
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Haalt de datum op waarop de optredens eindigen.

**Returns:**
java.util.Date - de datum waarop de gebeurtenissen eindigen.
### getMonthlyDay() {#getMonthlyDay--}
```
public final int getMonthlyDay()
```


Haalt een aantal dagen op van het maandelijkse terugkeerpatroon.

**Returns:**
int - een aantal dagen van het maandelijkse terugkeerpatroon.
### getMonthlyOrdinalDay() {#getMonthlyOrdinalDay--}
```
public final int getMonthlyOrdinalDay()
```


Haalt een dag op van het maandelijkse terugkeerpatroon bij gebruik van een rangorde-dag.

--------------------

Kan een van de waarden van de [DayOfWeek](../../com.aspose.tasks/dayofweek) enumeratie zijn.

**Returns:**
int - een dag van het maandelijkse terugkeerpatroon bij gebruik van een ordinale dag.
### getMonthlyOrdinalNumber() {#getMonthlyOrdinalNumber--}
```
public final int getMonthlyOrdinalNumber()
```


Haalt een rangordegetal op van het maandelijkse terugkeerpatroon.

--------------------

Kan een van de waarden van de [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumeratie zijn.

**Returns:**
int - een ordinaal getal van het maandelijkse terugkeerpatroon.
### getMonthlyOrdinalRepetitions() {#getMonthlyOrdinalRepetitions--}
```
public final int getMonthlyOrdinalRepetitions()
```


Haalt een aantal herhalingen op voor het maandelijkse terugkeerpatroon bij gebruik van een rangorde-dag.

**Returns:**
int - een aantal herhalingen voor het maandelijkse terugkeerpatroon bij gebruik van een ordinale dag.
### getMonthlyRepetitions() {#getMonthlyRepetitions--}
```
public final int getMonthlyRepetitions()
```


Haalt een aantal herhalingen op voor het maandelijkse terugkeerpatroon.

**Returns:**
int - een aantal herhalingen voor het maandelijkse terugkeerpatroon.
### getMonthlyUseOrdinalDay() {#getMonthlyUseOrdinalDay--}
```
public final boolean getMonthlyUseOrdinalDay()
```


Haalt een waarde op die aangeeft of een rangorde-dag moet worden gebruikt voor het maandelijkse terugkeerpatroon.

**Returns:**
boolean - een waarde die aangeeft of een ordinale dag gebruikt moet worden voor het maandelijkse terugkeerpatroon.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Haalt een aantal optredens op van de terugkerende taak.

**Returns:**
int - een aantal gebeurtenissen van de terugkerende taak.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final int getRecurrencePattern()
```


Haalt een terugkeerpatroon op van de terugkerende taak.

--------------------

Kan een van de waarden van de `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)) enumeratie zijn.

**Returns:**
int - een terugkeerpatroon van de terugkerende taak.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Haalt de datum op waarop de optredens beginnen.

**Returns:**
java.util.Date - de datum waarop de gebeurtenissen beginnen.
### getTask() {#getTask--}
```
public final Task getTask()
```


Haalt de bovenliggende taak op van deze instantie van de klasse [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo).

**Returns:**
[Task](../../com.aspose.tasks/task) - the parent task of this instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class.
### getUseEndDate() {#getUseEndDate--}
```
public final boolean getUseEndDate()
```


Haalt een waarde op die aangeeft of de einddatum of een aantal optredens moet worden gebruikt voor de terugkerende taak.

**Returns:**
boolean - een waarde die aangeeft of de einddatum of een aantal gebeurtenissen gebruikt moet worden voor de terugkerende taak.
### getWeeklyDays() {#getWeeklyDays--}
```
public final int getWeeklyDays()
```


Haalt een verzameling dagen op die worden gebruikt in het wekelijkse terugkeerpatroon.

--------------------

**Returns:**
int - een verzameling dagen die gebruikt worden in het wekelijkse terugkeerpatroon.
### getWeeklyRepetitions() {#getWeeklyRepetitions--}
```
public final int getWeeklyRepetitions()
```


Haalt een aantal herhalingen op voor het wekelijkse terugkeerpatroon.

**Returns:**
int - een aantal herhalingen voor het wekelijkse terugkeerpatroon.
### getYearlyDate() {#getYearlyDate--}
```
public final Date getYearlyDate()
```


Haalt een datum op voor het jaarlijkse terugkeerpatroon.

**Returns:**
java.util.Date - een datum voor het jaarlijkse terugkeerpatroon.
### getYearlyOrdinalDay() {#getYearlyOrdinalDay--}
```
public final int getYearlyOrdinalDay()
```


Haalt een weekdag op van het jaarlijkse terugkeerpatroon bij gebruik van een ordinale dag.

--------------------

Kan een van de waarden van de [DayOfWeek](../../com.aspose.tasks/dayofweek) enumeratie zijn.

**Returns:**
int - een weekdag van het jaarlijkse terugkeerpatroon bij gebruik van een ordinale dag.
### getYearlyOrdinalMonth() {#getYearlyOrdinalMonth--}
```
public final int getYearlyOrdinalMonth()
```


Haalt een maand op van het jaarlijkse terugkeerpatroon bij gebruik van een ordinale dag.

--------------------

Kan een van de waarden van de [Month](../../com.aspose.tasks/month) enumeratie zijn.

**Returns:**
int - een maand van het jaarlijkse terugkeerpatroon bij gebruik van een ordinale dag.
### getYearlyOrdinalNumber() {#getYearlyOrdinalNumber--}
```
public final int getYearlyOrdinalNumber()
```


Haalt een ordinaal getal op van het jaarlijkse terugkeerpatroon.

--------------------

Kan een van de waarden van de [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumeratie zijn.

**Returns:**
int - een ordinaal getal van het jaarlijkse terugkeerpatroon.
### getYearlyUseOrdinalDay() {#getYearlyUseOrdinalDay--}
```
public final boolean getYearlyUseOrdinalDay()
```


Haalt een waarde op die aangeeft of een ordinale dag moet worden gebruikt voor het jaarlijkse terugkeerpatroon.

**Returns:**
boolean - een waarde die aangeeft of een ordinale dag gebruikt moet worden voor het jaarlijkse terugkeerpatroon.
### setDailyRepetitions(int value) {#setDailyRepetitions-int-}
```
public final void setDailyRepetitions(int value)
```


Stelt een aantal herhalingen in voor het dagelijkse terugkeerpatroon.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een aantal herhalingen voor het dagelijkse recursiepatroon. |

### setDailyUseWorkdays(boolean value) {#setDailyUseWorkdays-boolean-}
```
public final void setDailyUseWorkdays(boolean value)
```


Stelt een waarde in die aangeeft of werkdagen moeten worden gebruikt voor het dagelijkse terugkeerpatroon.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of werkdagen moeten worden gebruikt voor het dagelijkse recursiepatroon. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Stelt de duur in voor één gebeurtenis van de terugkerende taak.

--------------------

de instantie van `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | de duur voor één gebeurtenis van de terugkerende taak. |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Stelt de datum in waarop de gebeurtenissen eindigen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | de datum waarop de gebeurtenissen eindigen. |

### setMonthlyDay(int value) {#setMonthlyDay-int-}
```
public final void setMonthlyDay(int value)
```


Stelt een dagnummer in van het maandelijkse terugkeerpatroon.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een dagnummer van het maandelijkse recursiepatroon. |

### setMonthlyOrdinalDay(int value) {#setMonthlyOrdinalDay-int-}
```
public final void setMonthlyOrdinalDay(int value)
```


Stelt een dag in van het maandelijkse terugkeerpatroon bij gebruik van een ordinale dag.

--------------------

Kan een van de waarden van de [DayOfWeek](../../com.aspose.tasks/dayofweek) enumeratie zijn.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een dag van het maandelijkse recursiepatroon bij gebruik van een ordinale dag. |

### setMonthlyOrdinalNumber(int value) {#setMonthlyOrdinalNumber-int-}
```
public final void setMonthlyOrdinalNumber(int value)
```


Stelt een ordinaal getal in van het maandelijkse terugkeerpatroon.

--------------------

Kan een van de waarden van de [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumeratie zijn.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een ordinaal getal van het maandelijkse recursiepatroon. |

### setMonthlyOrdinalRepetitions(int value) {#setMonthlyOrdinalRepetitions-int-}
```
public final void setMonthlyOrdinalRepetitions(int value)
```


Stelt een aantal herhalingen in voor het maandelijkse terugkeerpatroon bij gebruik van een ordinale dag.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een aantal herhalingen voor het maandelijkse recursiepatroon bij gebruik van een ordinale dag. |

### setMonthlyRepetitions(int value) {#setMonthlyRepetitions-int-}
```
public final void setMonthlyRepetitions(int value)
```


Stelt een aantal herhalingen in voor het maandelijkse terugkeerpatroon.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een aantal herhalingen voor het maandelijkse recursiepatroon. |

### setMonthlyUseOrdinalDay(boolean value) {#setMonthlyUseOrdinalDay-boolean-}
```
public final void setMonthlyUseOrdinalDay(boolean value)
```


Stelt een waarde in die aangeeft of een ordinale dag moet worden gebruikt voor het maandelijkse terugkeerpatroon.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of een ordinale dag moet worden gebruikt voor het maandelijkse recursiepatroon. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Stelt een aantal gebeurtenissen in van de terugkerende taak.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een aantal gebeurtenissen van de terugkerende taak. |

### setRecurrencePattern(int value) {#setRecurrencePattern-int-}
```
public final void setRecurrencePattern(int value)
```


Stelt een terugkeerpatroon in van de terugkerende taak.

--------------------

Kan een van de waarden van de `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)) enumeratie zijn.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een recursiepatroon van de terugkerende taak. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Stelt de datum in waarop de gebeurtenissen beginnen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | de datum waarop de gebeurtenissen beginnen. |

### setUseEndDate(boolean value) {#setUseEndDate-boolean-}
```
public final void setUseEndDate(boolean value)
```


Stelt een waarde in die aangeeft of de einddatum of een aantal gebeurtenissen moet worden gebruikt voor de terugkerende taak.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de einddatum of een aantal gebeurtenissen moet worden gebruikt voor de terugkerende taak. |

### setWeeklyDays(int value) {#setWeeklyDays-int-}
```
public final void setWeeklyDays(int value)
```


Stelt een verzameling dagen in die worden gebruikt in het wekelijkse terugkeerpatroon.

--------------------

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een verzameling dagen die worden gebruikt in het wekelijkse recursiepatroon. |

### setWeeklyRepetitions(int value) {#setWeeklyRepetitions-int-}
```
public final void setWeeklyRepetitions(int value)
```


Stelt een aantal herhalingen in voor het wekelijkse terugkeerpatroon.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een aantal herhalingen voor het wekelijkse recursiepatroon. |

### setYearlyDate(Date value) {#setYearlyDate-java.util.Date-}
```
public final void setYearlyDate(Date value)
```


Stelt een datum in voor het jaarlijkse terugkeerpatroon.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | een datum voor het jaarlijkse recursiepatroon. |

### setYearlyOrdinalDay(int value) {#setYearlyOrdinalDay-int-}
```
public final void setYearlyOrdinalDay(int value)
```


Stelt een weekdag in van het jaarlijkse terugkeerpatroon bij gebruik van een ordinale dag.

--------------------

Kan een van de waarden van de [DayOfWeek](../../com.aspose.tasks/dayofweek) enumeratie zijn.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een weekdag van het jaarlijkse recursiepatroon bij gebruik van een ordinale dag. |

### setYearlyOrdinalMonth(int value) {#setYearlyOrdinalMonth-int-}
```
public final void setYearlyOrdinalMonth(int value)
```


Stelt een maand in van het jaarlijkse terugkeerpatroon bij gebruik van een ordinale dag.

--------------------

Kan een van de waarden van de [Month](../../com.aspose.tasks/month) enumeratie zijn.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een maand van het jaarlijkse recursiepatroon bij gebruik van een ordinale dag. |

### setYearlyOrdinalNumber(int value) {#setYearlyOrdinalNumber-int-}
```
public final void setYearlyOrdinalNumber(int value)
```


Stelt een ordinaal getal in van het jaarlijkse terugkeerpatroon.

--------------------

Kan een van de waarden van de [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumeratie zijn.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een ordinaal getal van het jaarlijkse recursiepatroon. |

### setYearlyUseOrdinalDay(boolean value) {#setYearlyUseOrdinalDay-boolean-}
```
public final void setYearlyUseOrdinalDay(boolean value)
```


Stelt een waarde in die aangeeft of een ordinale dag moet worden gebruikt voor het jaarlijkse terugkeerpatroon.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of een ordinale dag moet worden gebruikt voor het jaarlijkse recursiepatroon. |

