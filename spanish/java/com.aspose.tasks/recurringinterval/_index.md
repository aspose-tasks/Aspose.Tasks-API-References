---
title: "RecurringInterval"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa intervalos recurrentes utilizados en las líneas de progreso de una vista de diagrama de Gantt."
type: docs
weight: 243
url: /es/java/com.aspose.tasks/recurringinterval/
---

**Inheritance:**
java.lang.Object
```
public class RecurringInterval
```

Representa intervalos recurrentes utilizados en las líneas de progreso de una vista de diagrama de Gantt.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [RecurringInterval()](#RecurringInterval--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [getDailyDayNumber()](#getDailyDayNumber--) | Obtiene el número del día diario. |
| [getDailyWorkday()](#getDailyWorkday--) | Obtiene un valor que indica si un día es laborable para las líneas de progreso diario. |
| [getInterval()](#getInterval--) | Obtiene el intervalo recurrente. |
| [getMonthlyDay()](#getMonthlyDay--) | Obtiene un valor que indica si se deben mostrar las líneas de progreso mensual por día. |
| [getMonthlyDayDayNumber()](#getMonthlyDayDayNumber--) | Obtiene el número del día de las líneas de progreso mensuales. |
| [getMonthlyDayMonthNumber()](#getMonthlyDayMonthNumber--) | Obtiene el número del mes de las líneas de progreso mensuales. |
| [getMonthlyFirstLast()](#getMonthlyFirstLast--) | Obtiene un valor que indica si se deben mostrar las líneas de progreso por el primer o último día predefinido. |
| [getMonthlyFirstLastDay()](#getMonthlyFirstLastDay--) | Obtiene el tipo de primer o último día de las líneas de progreso mensuales. |
| [getMonthlyFirstLastMonthNumber()](#getMonthlyFirstLastMonthNumber--) | Obtiene el número del mes de las líneas de progreso, que se muestran por el primer o último día predefinido. |
| [getWeeklyDays()](#getWeeklyDays--) | Obtiene una lista de días para las líneas de progreso semanales. |
| [getWeeklyWeekNumber()](#getWeeklyWeekNumber--) | Obtiene el número de la semana para las líneas de progreso semanales. |
| [setDailyDayNumber(int value)](#setDailyDayNumber-int-) | Establece el número del día diario. |
| [setDailyWorkday(boolean value)](#setDailyWorkday-boolean-) | Establece un valor que indica si un día es laborable para las líneas de progreso diarias. |
| [setInterval(int value)](#setInterval-int-) | Establece el intervalo recurrente. |
| [setMonthlyDay(boolean value)](#setMonthlyDay-boolean-) | Establece un valor que indica si se deben mostrar las líneas de progreso mensuales por día. |
| [setMonthlyDayDayNumber(int value)](#setMonthlyDayDayNumber-int-) | Establece el número del día de las líneas de progreso mensuales. |
| [setMonthlyDayMonthNumber(int value)](#setMonthlyDayMonthNumber-int-) | Establece el número del mes de las líneas de progreso mensuales. |
| [setMonthlyFirstLast(boolean value)](#setMonthlyFirstLast-boolean-) | Establece un valor que indica si se deben mostrar las líneas de progreso por el primer o último día predefinido. |
| [setMonthlyFirstLastDay(int value)](#setMonthlyFirstLastDay-int-) | Establece el tipo de primer o último día de las líneas de progreso mensuales. |
| [setMonthlyFirstLastMonthNumber(int value)](#setMonthlyFirstLastMonthNumber-int-) | Establece el número del mes de las líneas de progreso, que se muestran por el primer o último día predefinido. |
| [setWeeklyWeekNumber(int value)](#setWeeklyWeekNumber-int-) | Establece el número de la semana para las líneas de progreso semanales. |
### RecurringInterval() {#RecurringInterval--}
```
public RecurringInterval()
```


### getDailyDayNumber() {#getDailyDayNumber--}
```
public final int getDailyDayNumber()
```


Obtiene el número del día diario.

**Returns:**
int - el número del día diario.
### getDailyWorkday() {#getDailyWorkday--}
```
public final boolean getDailyWorkday()
```


Obtiene un valor que indica si un día es laborable para las líneas de progreso diario.

**Returns:**
boolean - un valor que indica si un día es laborable para las líneas de progreso diarias.
### getInterval() {#getInterval--}
```
public final int getInterval()
```


Obtiene el intervalo recurrente. Puede ser cualquier valor del tipo `Interval`([getInterval()](../../com.aspose/tasks/recurringinterval\#getInterval--)/[setInterval(int)](../../com.aspose/tasks/recurringinterval\#setInterval-int-)).

**Returns:**
int - el intervalo recurrente.
### getMonthlyDay() {#getMonthlyDay--}
```
public final boolean getMonthlyDay()
```


Obtiene un valor que indica si se deben mostrar las líneas de progreso mensual por día.

**Returns:**
boolean - un valor que indica si se deben mostrar las líneas de progreso mensuales por día.
### getMonthlyDayDayNumber() {#getMonthlyDayDayNumber--}
```
public final int getMonthlyDayDayNumber()
```


Obtiene el número del día de las líneas de progreso mensuales.

**Returns:**
int - el número del día de las líneas de progreso mensuales.
### getMonthlyDayMonthNumber() {#getMonthlyDayMonthNumber--}
```
public final int getMonthlyDayMonthNumber()
```


Obtiene el número del mes de las líneas de progreso mensuales.

**Returns:**
int - el número del mes de las líneas de progreso mensuales.
### getMonthlyFirstLast() {#getMonthlyFirstLast--}
```
public final boolean getMonthlyFirstLast()
```


Obtiene un valor que indica si se deben mostrar las líneas de progreso por el primer o último día predefinido.

**Returns:**
boolean - un valor que indica si se deben mostrar las líneas de progreso por el primer o último día predefinido.
### getMonthlyFirstLastDay() {#getMonthlyFirstLastDay--}
```
public final int getMonthlyFirstLastDay()
```


Obtiene el tipo de primer o último día de las líneas de progreso mensuales.

**Returns:**
int - el tipo de primer o último día de las líneas de progreso mensuales.
### getMonthlyFirstLastMonthNumber() {#getMonthlyFirstLastMonthNumber--}
```
public final int getMonthlyFirstLastMonthNumber()
```


Obtiene el número del mes de las líneas de progreso, que se muestran por el primer o último día predefinido.

**Returns:**
int - el número de mes de las líneas de progreso, que se muestran por el primer o último día predefinido.
### getWeeklyDays() {#getWeeklyDays--}
```
public final List<Integer> getWeeklyDays()
```


Obtiene una lista de días para las líneas de progreso semanales.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - una lista de días para líneas de progreso semanales.
### getWeeklyWeekNumber() {#getWeeklyWeekNumber--}
```
public final int getWeeklyWeekNumber()
```


Obtiene el número de la semana para las líneas de progreso semanales.

**Returns:**
int - el número de semana para líneas de progreso semanales.
### setDailyDayNumber(int value) {#setDailyDayNumber-int-}
```
public final void setDailyDayNumber(int value)
```


Establece el número del día diario.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el número de día diario. |

### setDailyWorkday(boolean value) {#setDailyWorkday-boolean-}
```
public final void setDailyWorkday(boolean value)
```


Establece un valor que indica si un día es laborable para las líneas de progreso diarias.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si un día es laborable para líneas de progreso diarias. |

### setInterval(int value) {#setInterval-int-}
```
public final void setInterval(int value)
```


Establece el intervalo recurrente. Puede ser cualquier valor del tipo `Interval`([getInterval()](../../com.aspose/tasks/recurringinterval\#getInterval--)/[setInterval(int)](../../com.aspose.tasks/recurringinterval\#setInterval-int-))

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el intervalo recurrente. |

### setMonthlyDay(boolean value) {#setMonthlyDay-boolean-}
```
public final void setMonthlyDay(boolean value)
```


Establece un valor que indica si se deben mostrar las líneas de progreso mensuales por día.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si mostrar líneas de progreso mensuales por día. |

### setMonthlyDayDayNumber(int value) {#setMonthlyDayDayNumber-int-}
```
public final void setMonthlyDayDayNumber(int value)
```


Establece el número del día de las líneas de progreso mensuales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el número de día de las líneas de progreso mensuales. |

### setMonthlyDayMonthNumber(int value) {#setMonthlyDayMonthNumber-int-}
```
public final void setMonthlyDayMonthNumber(int value)
```


Establece el número del mes de las líneas de progreso mensuales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el número de mes de las líneas de progreso mensuales. |

### setMonthlyFirstLast(boolean value) {#setMonthlyFirstLast-boolean-}
```
public final void setMonthlyFirstLast(boolean value)
```


Establece un valor que indica si se deben mostrar las líneas de progreso por el primer o último día predefinido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si mostrar líneas de progreso por el primer o último día predefinido. |

### setMonthlyFirstLastDay(int value) {#setMonthlyFirstLastDay-int-}
```
public final void setMonthlyFirstLastDay(int value)
```


Establece el tipo de primer o último día de las líneas de progreso mensuales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el tipo de primer o último día de las líneas de progreso mensuales. |

### setMonthlyFirstLastMonthNumber(int value) {#setMonthlyFirstLastMonthNumber-int-}
```
public final void setMonthlyFirstLastMonthNumber(int value)
```


Establece el número del mes de las líneas de progreso, que se muestran por el primer o último día predefinido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el número de mes de las líneas de progreso, que se muestran por el primer o último día predefinido. |

### setWeeklyWeekNumber(int value) {#setWeeklyWeekNumber-int-}
```
public final void setWeeklyWeekNumber(int value)
```


Establece el número de la semana para las líneas de progreso semanales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el número de semana para líneas de progreso semanales. |

