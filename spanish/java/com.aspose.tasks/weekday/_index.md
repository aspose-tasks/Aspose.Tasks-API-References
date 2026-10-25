---
title: "WeekDay"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un día de la semana que define días regulares de la semana o días de excepción en un calendario."
type: docs
weight: 352
url: /es/java/com.aspose.tasks/weekday/
---

**Inheritance:**
java.lang.Object
```
public class WeekDay
```

Representa un día de la semana que define días regulares de la semana o días de excepción en un calendario.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [WeekDay(int dayType)](#WeekDay-int-) | Inicializa una nueva instancia de la clase [WeekDay](../../com.aspose.tasks/weekday) con el tipo de día especificado. |
| [WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes)](#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--) | Inicializa una nueva instancia de la clase [WeekDay](../../com.aspose.tasks/weekday) con el tipo de día especificado y la lista de períodos de tiempo laborables. |
| [WeekDay(int dayType, WorkingTime[] workingTimes)](#WeekDay-int-com.aspose.tasks.WorkingTime...-) | Inicializa una nueva instancia de la clase [WeekDay](../../com.aspose.tasks/weekday) con el tipo de día especificado y los períodos de tiempo laborables. |
| [WeekDay()](#WeekDay--) | Inicializa una nueva instancia de la clase [WeekDay](../../com.aspose.tasks/weekday). |
## Métodos

| Método | Descripción |
| --- | --- |
| [castToDayType(int dw)](#castToDayType-int-) | Convierte el [DayOfWeek](../../com.aspose.tasks/dayofweek) de .Net a `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)). |
| [createDefaultWorkingDay(int dayType)](#createDefaultWorkingDay-int-) | Crea un día laborable predeterminado. |
| [deepClone()](#deepClone--) | Devuelve una copia profunda del día de la semana. |
| [equals(Object obj)](#equals-java.lang.Object-) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [getDayType()](#getDayType--) | Obtiene el tipo de un día. |
| [getDayWorking()](#getDayWorking--) | Obtiene un valor que indica si la fecha o el tipo de día especificado es laborable. |
| [getFromDate()](#getFromDate--) | Obtiene el inicio de un tiempo de excepción. |
| [getToDate()](#getToDate--) | Obtiene el final de un tiempo de excepción. |
| [getWorkingTime()](#getWorkingTime--) | Devuelve el tiempo laborable para un día de la semana. |
| [getWorkingTimes()](#getWorkingTimes--) | Obtiene WorkingTimeCollection para esta instancia de WeekDay. |
| [hashCode()](#hashCode--) | Devuelve un valor de código hash para la instancia de la clase [WeekDay](../../com.aspose.tasks/weekday). |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Establece un valor que indica si la fecha o el tipo de día especificado es laborable. |
| [setDefaultWorkingTime(WeekDay day)](#setDefaultWorkingTime-com.aspose.tasks.WeekDay-) | Establece períodos de tiempo predeterminados para el día de la semana especificado. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | Establece el inicio de un tiempo de excepción. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | Establece el final de un tiempo de excepción. |
### WeekDay(int dayType) {#WeekDay-int-}
```
public WeekDay(int dayType)
```


Inicializa una nueva instancia de la clase [WeekDay](../../com.aspose.tasks/weekday) con el tipo de día especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dayType | int | El tipo de día especificado. |

### WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes) {#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--}
```
public WeekDay(int dayType, List<WorkingTime> workingTimes)
```


Inicializa una nueva instancia de la clase [WeekDay](../../com.aspose.tasks/weekday) con el tipo de día especificado y la lista de períodos de tiempo laborables.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dayType | int | El tipo de día especificado. |
| workingTimes | java.util.List&lt;com.aspose.tasks.WorkingTime&gt; | Lista de períodos de tiempo laborables. |

### WeekDay(int dayType, WorkingTime[] workingTimes) {#WeekDay-int-com.aspose.tasks.WorkingTime...-}
```
public WeekDay(int dayType, WorkingTime[] workingTimes)
```


Inicializa una nueva instancia de la clase [WeekDay](../../com.aspose.tasks/weekday) con el tipo de día especificado y los períodos de tiempo laborables.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dayType | int | El tipo de día especificado. |
| workingTimes | [WorkingTime\[\]](../../com.aspose.tasks/workingtime) | Matriz de períodos de tiempo laborables. |

### WeekDay() {#WeekDay--}
```
public WeekDay()
```


Inicializa una nueva instancia de la clase [WeekDay](../../com.aspose.tasks/weekday).

### castToDayType(int dw) {#castToDayType-int-}
```
public static int castToDayType(int dw)
```


Convierte el [DayOfWeek](../../com.aspose.tasks/dayofweek) de .Net a `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dw | int | El día de la semana del cual convertir. |

**Returns:**
int - Un tipo de día convertido.
### createDefaultWorkingDay(int dayType) {#createDefaultWorkingDay-int-}
```
public static WeekDay createDefaultWorkingDay(int dayType)
```


Crea un día laborable predeterminado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dayType | int | El tipo de día del cual crear el día laborable predeterminado. |

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - A default working day with working times 8-12 and 13-17.
### deepClone() {#deepClone--}
```
public final WeekDay deepClone()
```


Devuelve una copia profunda del día de la semana.

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - Returns the deep copy of the week day.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | El objeto para comparar con esta instancia. |

**Returns:**
boolean - **True** si el objeto especificado es un WeekDay que tiene los mismos valores FromDate, ToDate y WorkingTimes que esta instancia; de lo contrario, **false**.
### getDayType() {#getDayType--}
```
public final int getDayType()
```


Obtiene el tipo de un día.

**Returns:**
int - el tipo de un día.
### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Obtiene un valor que indica si la fecha o el tipo de día especificado es laborable.

**Returns:**
boolean - un valor que indica si la fecha o tipo de día especificado está trabajando.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


Obtiene el inicio de un tiempo de excepción.

**Returns:**
java.util.Date - el comienzo de un tiempo de excepción.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


Obtiene el final de un tiempo de excepción.

**Returns:**
java.util.Date - el final de un tiempo de excepción.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Devuelve el tiempo laborable para un día de la semana.

**Returns:**
double - Tiempo de trabajo.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


Obtiene WorkingTimeCollection para esta instancia de WeekDay. La colección de tiempos de trabajo que define el tiempo trabajado en el día de la semana.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - WorkingTimeCollection for this WeekDay instance.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Devuelve un valor de código hash para la instancia de la clase [WeekDay](../../com.aspose.tasks/weekday).

**Returns:**
int - devuelve un valor de código hash para este objeto.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Establece un valor que indica si la fecha o el tipo de día especificado es laborable.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si la fecha o tipo de día especificado está trabajando. |

### setDefaultWorkingTime(WeekDay day) {#setDefaultWorkingTime-com.aspose.tasks.WeekDay-}
```
public static void setDefaultWorkingTime(WeekDay day)
```


Establece períodos de tiempo predeterminados para el día de la semana especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| day | [WeekDay](../../com.aspose.tasks/weekday) | El día de la semana en el que establecer el día laborable predeterminado. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


Establece el inicio de un tiempo de excepción.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | el comienzo de un tiempo de excepción. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


Establece el final de un tiempo de excepción.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | el final de un tiempo de excepción. |

