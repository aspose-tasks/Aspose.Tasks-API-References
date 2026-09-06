---
title: "RecurringTaskInfo"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa los detalles de una tarea recurrente en un proyecto."
type: docs
weight: 244
url: /es/java/com.aspose.tasks/recurringtaskinfo/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskInfo
```

Representa los detalles de una tarea recurrente en un proyecto.
## Métodos

| Método | Descripción |
| --- | --- |
| [getDailyRepetitions()](#getDailyRepetitions--) | Obtiene un número de repeticiones para el patrón de recurrencia diaria. |
| [getDailyUseWorkdays()](#getDailyUseWorkdays--) | Obtiene un valor que indica si se deben usar días laborables para el patrón de recurrencia diaria. |
| [getDuration()](#getDuration--) | Obtiene la duración de una ocurrencia de la tarea recurrente. |
| [getEndDate()](#getEndDate--) | Obtiene la fecha en que deben terminar las ocurrencias. |
| [getMonthlyDay()](#getMonthlyDay--) | Obtiene un número de día del patrón de recurrencia mensual. |
| [getMonthlyOrdinalDay()](#getMonthlyOrdinalDay--) | Obtiene un día del patrón de recurrencia mensual al usar día ordinal. |
| [getMonthlyOrdinalNumber()](#getMonthlyOrdinalNumber--) | Obtiene un número ordinal del patrón de recurrencia mensual. |
| [getMonthlyOrdinalRepetitions()](#getMonthlyOrdinalRepetitions--) | Obtiene un número de repeticiones para el patrón de recurrencia mensual al usar día ordinal. |
| [getMonthlyRepetitions()](#getMonthlyRepetitions--) | Obtiene un número de repeticiones para el patrón de recurrencia mensual. |
| [getMonthlyUseOrdinalDay()](#getMonthlyUseOrdinalDay--) | Obtiene un valor que indica si se debe usar día ordinal para el patrón de recurrencia mensual. |
| [getOccurrences()](#getOccurrences--) | Obtiene un número de ocurrencias de la tarea recurrente. |
| [getRecurrencePattern()](#getRecurrencePattern--) | Obtiene un patrón de recurrencia de la tarea recurrente. |
| [getStartDate()](#getStartDate--) | Obtiene la fecha en que deben comenzar las ocurrencias. |
| [getTask()](#getTask--) | Obtiene la tarea principal de esta instancia de la clase [RecurringTaskInfo](../../com.aspose/tasks/recurringtaskinfo). |
| [getUseEndDate()](#getUseEndDate--) | Obtiene un valor que indica si se debe usar la fecha de finalización o un número de ocurrencias para la tarea recurrente. |
| [getWeeklyDays()](#getWeeklyDays--) | Obtiene una colección de días utilizados en el patrón de recurrencia semanal. |
| [getWeeklyRepetitions()](#getWeeklyRepetitions--) | Obtiene un número de repeticiones para el patrón de recurrencia semanal. |
| [getYearlyDate()](#getYearlyDate--) | Obtiene una fecha para el patrón de recurrencia anual. |
| [getYearlyOrdinalDay()](#getYearlyOrdinalDay--) | Obtiene un día de la semana del patrón de recurrencia anual al usar día ordinal. |
| [getYearlyOrdinalMonth()](#getYearlyOrdinalMonth--) | Obtiene un mes del patrón de recurrencia anual al usar día ordinal. |
| [getYearlyOrdinalNumber()](#getYearlyOrdinalNumber--) | Obtiene un número ordinal del patrón de recurrencia anual. |
| [getYearlyUseOrdinalDay()](#getYearlyUseOrdinalDay--) | Obtiene un valor que indica si se debe usar día ordinal para el patrón de recurrencia anual. |
| [setDailyRepetitions(int value)](#setDailyRepetitions-int-) | Establece un número de repeticiones para el patrón de recurrencia diario. |
| [setDailyUseWorkdays(boolean value)](#setDailyUseWorkdays-boolean-) | Establece un valor que indica si se deben usar días laborables para el patrón de recurrencia diario. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Establece la duración de una ocurrencia de la tarea recurrente. |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Establece la fecha en que terminan las ocurrencias. |
| [setMonthlyDay(int value)](#setMonthlyDay-int-) | Establece un número de día del patrón de recurrencia mensual. |
| [setMonthlyOrdinalDay(int value)](#setMonthlyOrdinalDay-int-) | Establece un día del patrón de recurrencia mensual al usar día ordinal. |
| [setMonthlyOrdinalNumber(int value)](#setMonthlyOrdinalNumber-int-) | Establece un número ordinal del patrón de recurrencia mensual. |
| [setMonthlyOrdinalRepetitions(int value)](#setMonthlyOrdinalRepetitions-int-) | Establece un número de repeticiones para el patrón de recurrencia mensual al usar día ordinal. |
| [setMonthlyRepetitions(int value)](#setMonthlyRepetitions-int-) | Establece un número de repeticiones para el patrón de recurrencia mensual. |
| [setMonthlyUseOrdinalDay(boolean value)](#setMonthlyUseOrdinalDay-boolean-) | Establece un valor que indica si se debe usar día ordinal para el patrón de recurrencia mensual. |
| [setOccurrences(int value)](#setOccurrences-int-) | Establece un número de ocurrencias de la tarea recurrente. |
| [setRecurrencePattern(int value)](#setRecurrencePattern-int-) | Establece un patrón de recurrencia de la tarea recurrente. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Establece la fecha en que comienzan las ocurrencias. |
| [setUseEndDate(boolean value)](#setUseEndDate-boolean-) | Establece un valor que indica si se debe usar la fecha de finalización o un número de ocurrencias para la tarea recurrente. |
| [setWeeklyDays(int value)](#setWeeklyDays-int-) | Establece una colección de días usados en el patrón de recurrencia semanal. |
| [setWeeklyRepetitions(int value)](#setWeeklyRepetitions-int-) | Establece un número de repeticiones para el patrón de recurrencia semanal. |
| [setYearlyDate(Date value)](#setYearlyDate-java.util.Date-) | Establece una fecha para el patrón de recurrencia anual. |
| [setYearlyOrdinalDay(int value)](#setYearlyOrdinalDay-int-) | Establece un día de la semana del patrón de recurrencia anual al usar día ordinal. |
| [setYearlyOrdinalMonth(int value)](#setYearlyOrdinalMonth-int-) | Establece un mes del patrón de recurrencia anual al usar día ordinal. |
| [setYearlyOrdinalNumber(int value)](#setYearlyOrdinalNumber-int-) | Establece un número ordinal del patrón de recurrencia anual. |
| [setYearlyUseOrdinalDay(boolean value)](#setYearlyUseOrdinalDay-boolean-) | Establece un valor que indica si se debe usar día ordinal para el patrón de recurrencia anual. |
### getDailyRepetitions() {#getDailyRepetitions--}
```
public final int getDailyRepetitions()
```


Obtiene un número de repeticiones para el patrón de recurrencia diaria.

**Returns:**
int - un número de repeticiones para el patrón de recurrencia diario.
### getDailyUseWorkdays() {#getDailyUseWorkdays--}
```
public final boolean getDailyUseWorkdays()
```


Obtiene un valor que indica si se deben usar días laborables para el patrón de recurrencia diaria.

**Returns:**
boolean - un valor que indica si se deben usar días laborables para el patrón de recurrencia diario.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Obtiene la duración de una ocurrencia de la tarea recurrente.

--------------------

la instancia de la clase `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)).

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration for one occurrence of the recurring task.
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Obtiene la fecha en que deben terminar las ocurrencias.

**Returns:**
java.util.Date - la fecha en que terminan las ocurrencias.
### getMonthlyDay() {#getMonthlyDay--}
```
public final int getMonthlyDay()
```


Obtiene un número de día del patrón de recurrencia mensual.

**Returns:**
int - un número de día del patrón de recurrencia mensual.
### getMonthlyOrdinalDay() {#getMonthlyOrdinalDay--}
```
public final int getMonthlyOrdinalDay()
```


Obtiene un día del patrón de recurrencia mensual al usar día ordinal.

--------------------

Puede ser uno de los valores de la enumeración [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Returns:**
int - un día del patrón de recurrencia mensual al usar día ordinal.
### getMonthlyOrdinalNumber() {#getMonthlyOrdinalNumber--}
```
public final int getMonthlyOrdinalNumber()
```


Obtiene un número ordinal del patrón de recurrencia mensual.

--------------------

Puede ser uno de los valores de la enumeración [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Returns:**
int - un número ordinal del patrón de recurrencia mensual.
### getMonthlyOrdinalRepetitions() {#getMonthlyOrdinalRepetitions--}
```
public final int getMonthlyOrdinalRepetitions()
```


Obtiene un número de repeticiones para el patrón de recurrencia mensual al usar día ordinal.

**Returns:**
int - un número de repeticiones para el patrón de recurrencia mensual al usar día ordinal.
### getMonthlyRepetitions() {#getMonthlyRepetitions--}
```
public final int getMonthlyRepetitions()
```


Obtiene un número de repeticiones para el patrón de recurrencia mensual.

**Returns:**
int - un número de repeticiones para el patrón de recurrencia mensual.
### getMonthlyUseOrdinalDay() {#getMonthlyUseOrdinalDay--}
```
public final boolean getMonthlyUseOrdinalDay()
```


Obtiene un valor que indica si se debe usar día ordinal para el patrón de recurrencia mensual.

**Returns:**
boolean - un valor que indica si se debe usar día ordinal para el patrón de recurrencia mensual.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Obtiene un número de ocurrencias de la tarea recurrente.

**Returns:**
int - un número de ocurrencias de la tarea recurrente.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final int getRecurrencePattern()
```


Obtiene un patrón de recurrencia de la tarea recurrente.

--------------------

Puede ser uno de los valores de la enumeración `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)).

**Returns:**
int - un patrón de recurrencia de la tarea recurrente.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Obtiene la fecha en que deben comenzar las ocurrencias.

**Returns:**
java.util.Date - la fecha en que comienzan las ocurrencias.
### getTask() {#getTask--}
```
public final Task getTask()
```


Obtiene la tarea principal de esta instancia de la clase [RecurringTaskInfo](../../com.aspose/tasks/recurringtaskinfo).

**Returns:**
[Task](../../com.aspose.tasks/task) - the parent task of this instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class.
### getUseEndDate() {#getUseEndDate--}
```
public final boolean getUseEndDate()
```


Obtiene un valor que indica si se debe usar la fecha de finalización o un número de ocurrencias para la tarea recurrente.

**Returns:**
boolean - un valor que indica si se debe usar la fecha de finalización o un número de ocurrencias para la tarea recurrente.
### getWeeklyDays() {#getWeeklyDays--}
```
public final int getWeeklyDays()
```


Obtiene una colección de días utilizados en el patrón de recurrencia semanal.

--------------------

**Returns:**
int - una colección de días usados en el patrón de recurrencia semanal.
### getWeeklyRepetitions() {#getWeeklyRepetitions--}
```
public final int getWeeklyRepetitions()
```


Obtiene un número de repeticiones para el patrón de recurrencia semanal.

**Returns:**
int - un número de repeticiones para el patrón de recurrencia semanal.
### getYearlyDate() {#getYearlyDate--}
```
public final Date getYearlyDate()
```


Obtiene una fecha para el patrón de recurrencia anual.

**Returns:**
java.util.Date - una fecha para el patrón de recurrencia anual.
### getYearlyOrdinalDay() {#getYearlyOrdinalDay--}
```
public final int getYearlyOrdinalDay()
```


Obtiene un día de la semana del patrón de recurrencia anual al usar día ordinal.

--------------------

Puede ser uno de los valores de la enumeración [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Returns:**
int - un día laborable del patrón de recurrencia anual al usar día ordinal.
### getYearlyOrdinalMonth() {#getYearlyOrdinalMonth--}
```
public final int getYearlyOrdinalMonth()
```


Obtiene un mes del patrón de recurrencia anual al usar día ordinal.

--------------------

Puede ser uno de los valores de la enumeración [Month](../../com.aspose.tasks/month).

**Returns:**
int - un mes del patrón de recurrencia anual al usar día ordinal.
### getYearlyOrdinalNumber() {#getYearlyOrdinalNumber--}
```
public final int getYearlyOrdinalNumber()
```


Obtiene un número ordinal del patrón de recurrencia anual.

--------------------

Puede ser uno de los valores de la enumeración [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Returns:**
int - un número ordinal del patrón de recurrencia anual.
### getYearlyUseOrdinalDay() {#getYearlyUseOrdinalDay--}
```
public final boolean getYearlyUseOrdinalDay()
```


Obtiene un valor que indica si se debe usar día ordinal para el patrón de recurrencia anual.

**Returns:**
boolean - un valor que indica si se debe usar día ordinal para el patrón de recurrencia anual.
### setDailyRepetitions(int value) {#setDailyRepetitions-int-}
```
public final void setDailyRepetitions(int value)
```


Establece un número de repeticiones para el patrón de recurrencia diario.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un número de repeticiones para el patrón de recurrencia diario. |

### setDailyUseWorkdays(boolean value) {#setDailyUseWorkdays-boolean-}
```
public final void setDailyUseWorkdays(boolean value)
```


Establece un valor que indica si se deben usar días laborables para el patrón de recurrencia diario.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se deben usar días laborables para el patrón de recurrencia diario. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Establece la duración de una ocurrencia de la tarea recurrente.

--------------------

la instancia de la clase `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | la duración de una ocurrencia de la tarea recurrente. |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Establece la fecha en que terminan las ocurrencias.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | la fecha en que terminan las ocurrencias. |

### setMonthlyDay(int value) {#setMonthlyDay-int-}
```
public final void setMonthlyDay(int value)
```


Establece un número de día del patrón de recurrencia mensual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un número de día del patrón de recurrencia mensual. |

### setMonthlyOrdinalDay(int value) {#setMonthlyOrdinalDay-int-}
```
public final void setMonthlyOrdinalDay(int value)
```


Establece un día del patrón de recurrencia mensual al usar día ordinal.

--------------------

Puede ser uno de los valores de la enumeración [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un día del patrón de recurrencia mensual al usar día ordinal. |

### setMonthlyOrdinalNumber(int value) {#setMonthlyOrdinalNumber-int-}
```
public final void setMonthlyOrdinalNumber(int value)
```


Establece un número ordinal del patrón de recurrencia mensual.

--------------------

Puede ser uno de los valores de la enumeración [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un número ordinal del patrón de recurrencia mensual. |

### setMonthlyOrdinalRepetitions(int value) {#setMonthlyOrdinalRepetitions-int-}
```
public final void setMonthlyOrdinalRepetitions(int value)
```


Establece un número de repeticiones para el patrón de recurrencia mensual al usar día ordinal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un número de repeticiones para el patrón de recurrencia mensual al usar día ordinal. |

### setMonthlyRepetitions(int value) {#setMonthlyRepetitions-int-}
```
public final void setMonthlyRepetitions(int value)
```


Establece un número de repeticiones para el patrón de recurrencia mensual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un número de repeticiones para el patrón de recurrencia mensual. |

### setMonthlyUseOrdinalDay(boolean value) {#setMonthlyUseOrdinalDay-boolean-}
```
public final void setMonthlyUseOrdinalDay(boolean value)
```


Establece un valor que indica si se debe usar día ordinal para el patrón de recurrencia mensual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se debe usar día ordinal para el patrón de recurrencia mensual. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Establece un número de ocurrencias de la tarea recurrente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un número de ocurrencias de la tarea recurrente. |

### setRecurrencePattern(int value) {#setRecurrencePattern-int-}
```
public final void setRecurrencePattern(int value)
```


Establece un patrón de recurrencia de la tarea recurrente.

--------------------

Puede ser uno de los valores de la enumeración `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un patrón de recurrencia de la tarea recurrente. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Establece la fecha en que comienzan las ocurrencias.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | la fecha en que comienzan las ocurrencias. |

### setUseEndDate(boolean value) {#setUseEndDate-boolean-}
```
public final void setUseEndDate(boolean value)
```


Establece un valor que indica si se debe usar la fecha de finalización o un número de ocurrencias para la tarea recurrente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se debe usar la fecha de finalización o un número de ocurrencias para la tarea recurrente. |

### setWeeklyDays(int value) {#setWeeklyDays-int-}
```
public final void setWeeklyDays(int value)
```


Establece una colección de días usados en el patrón de recurrencia semanal.

--------------------

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | una colección de días usados en el patrón de recurrencia semanal. |

### setWeeklyRepetitions(int value) {#setWeeklyRepetitions-int-}
```
public final void setWeeklyRepetitions(int value)
```


Establece un número de repeticiones para el patrón de recurrencia semanal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un número de repeticiones para el patrón de recurrencia semanal. |

### setYearlyDate(Date value) {#setYearlyDate-java.util.Date-}
```
public final void setYearlyDate(Date value)
```


Establece una fecha para el patrón de recurrencia anual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | una fecha para el patrón de recurrencia anual. |

### setYearlyOrdinalDay(int value) {#setYearlyOrdinalDay-int-}
```
public final void setYearlyOrdinalDay(int value)
```


Establece un día de la semana del patrón de recurrencia anual al usar día ordinal.

--------------------

Puede ser uno de los valores de la enumeración [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un día de la semana del patrón de recurrencia anual al usar día ordinal. |

### setYearlyOrdinalMonth(int value) {#setYearlyOrdinalMonth-int-}
```
public final void setYearlyOrdinalMonth(int value)
```


Establece un mes del patrón de recurrencia anual al usar día ordinal.

--------------------

Puede ser uno de los valores de la enumeración [Month](../../com.aspose.tasks/month).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un mes del patrón de recurrencia anual al usar día ordinal. |

### setYearlyOrdinalNumber(int value) {#setYearlyOrdinalNumber-int-}
```
public final void setYearlyOrdinalNumber(int value)
```


Establece un número ordinal del patrón de recurrencia anual.

--------------------

Puede ser uno de los valores de la enumeración [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un número ordinal del patrón de recurrencia anual. |

### setYearlyUseOrdinalDay(boolean value) {#setYearlyUseOrdinalDay-boolean-}
```
public final void setYearlyUseOrdinalDay(boolean value)
```


Establece un valor que indica si se debe usar día ordinal para el patrón de recurrencia anual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se debe usar día ordinal para el patrón de recurrencia anual. |

