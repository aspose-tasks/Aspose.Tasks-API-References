---
title: "CalendarException"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa períodos de tiempo excepcionales en un calendario."
type: docs
weight: 43
url: /es/java/com.aspose.tasks/calendarexception/
---

**Inheritance:**
java.lang.Object
```
public final class CalendarException
```

Representa períodos de tiempo excepcionales en un calendario.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [CalendarException()](#CalendarException--) | Inicializa una nueva instancia de la clase [CalendarException](../../com.aspose.tasks/calendarexception). |
## Métodos

| Método | Descripción |
| --- | --- |
| [checkException(Date dt)](#checkException-java.util.Date-) | Devuelve true si la instancia especificada de la estructura java.util.Date es el día de excepción. |
| [delete()](#delete--) | Elimina la instancia Exception del objeto CalendarExceptionCollection del calendario principal. |
| [getDayWorking()](#getDayWorking--) | Obtiene un valor que indica si la fecha o el tipo de día especificado es laborable. |
| [getDaysOfWeek()](#getDaysOfWeek--) | Obtiene la DayTypeCollection de este objeto. |
| [getEnteredByOccurrences()](#getEnteredByOccurrences--) | Obtiene un valor que indica si el rango de recurrencia se define ingresando un número de ocurrencias. |
| [getExceptionDates()](#getExceptionDates--) | Devuelve las fechas en las que la excepción del calendario es aplicable. |
| [getFromDate()](#getFromDate--) | Obtiene el comienzo del tiempo de excepción. |
| [getMonth()](#getMonth--) | Obtiene el mes para el cual se programa una recurrencia de excepción. |
| [getMonthDay()](#getMonthDay--) | Obtiene el día del mes en el que se programa una recurrencia de excepción. |
| [getMonthItem()](#getMonthItem--) | Obtiene el elemento de mes para el cual se programa una recurrencia de excepción. |
| [getMonthPosition()](#getMonthPosition--) | Obtiene la posición de un elemento de mes dentro de un mes. |
| [getName()](#getName--) | Obtiene el nombre de la excepción. |
| [getOccurrences()](#getOccurrences--) | Obtiene el número de ocurrencias para las cuales la excepción del calendario es válida. |
| [getParentCalendar()](#getParentCalendar--) | Obtiene el calendario principal de este objeto. |
| [getPeriod()](#getPeriod--) | Obtiene el período de recurrencia de la excepción. |
| [getToDate()](#getToDate--) | Obtiene el final del tiempo de excepción. |
| [getType()](#getType--) | Obtiene el tipo de excepción. |
| [getWorkingTime()](#getWorkingTime--) | Devuelve el tiempo de trabajo para una excepción del calendario. |
| [getWorkingTimes()](#getWorkingTimes--) | Obtiene el objeto WorkingTimeCollection. |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Establece un valor que indica si la fecha o el tipo de día especificado es laborable. |
| [setEnteredByOccurrences(boolean value)](#setEnteredByOccurrences-boolean-) | Establece un valor que indica si el rango de recurrencia se define ingresando un número de ocurrencias. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | Establece el comienzo del tiempo de la excepción. |
| [setMonth(int value)](#setMonth-int-) | Establece el mes para el cual se programa una recurrencia de excepción. |
| [setMonthDay(int value)](#setMonthDay-int-) | Establece el día del mes en el que se programa una recurrencia de excepción. |
| [setMonthItem(int value)](#setMonthItem-int-) | Establece el elemento de mes para el cual se programa una recurrencia de excepción. |
| [setMonthPosition(int value)](#setMonthPosition-int-) | Establece la posición de un elemento de mes dentro de un mes. |
| [setName(String value)](#setName-java.lang.String-) | Establece el nombre de la excepción. |
| [setOccurrences(int value)](#setOccurrences-int-) | Establece el número de ocurrencias para las que la excepción del calendario es válida. |
| [setPeriod(int value)](#setPeriod-int-) | Establece el período de recurrencia de la excepción. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | Establece el final del tiempo de la excepción. |
| [setType(int value)](#setType-int-) | Establece el tipo de excepción. |
| [setWorkingTimes(WorkingTimeCollection value)](#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-) | Establece el objeto WorkingTimeCollection. |
### CalendarException() {#CalendarException--}
```
public CalendarException()
```


Inicializa una nueva instancia de la clase [CalendarException](../../com.aspose.tasks/calendarexception).

### checkException(Date dt) {#checkException-java.util.Date-}
```
public final boolean checkException(Date dt)
```


Devuelve true si la instancia especificada de la estructura java.util.Date es el día de excepción.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dt | java.util.Date | la instancia especificada de la estructura java.util.Date. |

**Returns:**
boolean - Devuelve true si el valor java.util.Date es el día de la excepción; de lo contrario, false.
### delete() {#delete--}
```
public final void delete()
```


Elimina la instancia Exception del objeto CalendarExceptionCollection del calendario principal.

### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Obtiene un valor que indica si la fecha o el tipo de día especificado es laborable.

**Returns:**
boolean - un valor que indica si la fecha o tipo de día especificado está trabajando.
### getDaysOfWeek() {#getDaysOfWeek--}
```
public final DayTypeCollection getDaysOfWeek()
```


Obtiene la DayTypeCollection para este objeto. Los días de la semana en los que la excepción es válida.

**Returns:**
[DayTypeCollection](../../com.aspose.tasks/daytypecollection) - the DayTypeCollection for this object.
### getEnteredByOccurrences() {#getEnteredByOccurrences--}
```
public final boolean getEnteredByOccurrences()
```


Obtiene un valor que indica si el rango de recurrencia se define ingresando un número de ocurrencias. False especifica que el rango de recurrencia se define ingresando una fecha de finalización.

**Returns:**
boolean - un valor que indica si el rango de recurrencia se define ingresando un número de ocurrencias.
### getExceptionDates() {#getExceptionDates--}
```
public final Iterable<Date> getExceptionDates()
```


Devuelve las fechas en las que la excepción del calendario es aplicable.

**Returns:**
java.lang.Iterable&lt;java.util.Date&gt; - fechas en las que la excepción del calendario es aplicable.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


Obtiene el comienzo del tiempo de excepción.

**Returns:**
java.util.Date - el comienzo del tiempo de la excepción.
### getMonth() {#getMonth--}
```
public final int getMonth()
```


Obtiene el mes para el cual se programa una recurrencia de excepción.

**Returns:**
int - el mes para el cual se programa una recurrencia de excepción.
### getMonthDay() {#getMonthDay--}
```
public final int getMonthDay()
```


Obtiene el día del mes en el que se programa una recurrencia de excepción.

**Returns:**
int - el día del mes en el que se programa una recurrencia de excepción.
### getMonthItem() {#getMonthItem--}
```
public final int getMonthItem()
```


Obtiene el elemento de mes para el cual se programa una recurrencia de excepción.

**Returns:**
int - el elemento de mes para el cual se programa una recurrencia de excepción.
### getMonthPosition() {#getMonthPosition--}
```
public final int getMonthPosition()
```


Obtiene la posición de un elemento de mes dentro de un mes.

**Returns:**
int - la posición de un elemento de mes dentro de un mes.
### getName() {#getName--}
```
public final String getName()
```


Obtiene el nombre de la excepción.

**Returns:**
java.lang.String - el nombre de la excepción.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Obtiene el número de ocurrencias para las cuales la excepción del calendario es válida.

**Returns:**
int - el número de ocurrencias para las que la excepción del calendario es válida.
### getParentCalendar() {#getParentCalendar--}
```
public final Calendar getParentCalendar()
```


Obtiene el calendario principal de este objeto.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - the parent calendar for this object.
### getPeriod() {#getPeriod--}
```
public final int getPeriod()
```


Obtiene el período de recurrencia de la excepción.

**Returns:**
int - el período de recurrencia de la excepción.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


Obtiene el final del tiempo de excepción.

**Returns:**
java.util.Date - el final del tiempo de la excepción.
### getType() {#getType--}
```
public final int getType()
```


Obtiene el tipo de excepción.

**Returns:**
int - el tipo de excepción.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Devuelve el tiempo de trabajo para una excepción del calendario.

**Returns:**
double - Devuelve el tiempo de trabajo para esta excepción de calendario.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


Obtiene el objeto WorkingTimeCollection. La colección de tiempos de trabajo que define el tiempo trabajado en el día de la semana.

--------------------

Debe haber al menos un tiempo de trabajo presente, y no puede haber más de cinco.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - the WorkingTimeCollection object.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Establece un valor que indica si la fecha o el tipo de día especificado es laborable.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si la fecha o tipo de día especificado está trabajando. |

### setEnteredByOccurrences(boolean value) {#setEnteredByOccurrences-boolean-}
```
public final void setEnteredByOccurrences(boolean value)
```


Establece un valor que indica si el rango de recurrencia se define ingresando un número de ocurrencias. False especifica que el rango de recurrencia se define ingresando una fecha de finalización.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si el rango de recurrencia se define ingresando un número de ocurrencias. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


Establece el comienzo del tiempo de la excepción.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | el comienzo del tiempo de la excepción. |

### setMonth(int value) {#setMonth-int-}
```
public final void setMonth(int value)
```


Establece el mes para el cual se programa una recurrencia de excepción.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el mes para el cual se programa una recurrencia de excepción. |

### setMonthDay(int value) {#setMonthDay-int-}
```
public final void setMonthDay(int value)
```


Establece el día del mes en el que se programa una recurrencia de excepción.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el día del mes en el que se programa una recurrencia de excepción. |

### setMonthItem(int value) {#setMonthItem-int-}
```
public final void setMonthItem(int value)
```


Establece el elemento de mes para el cual se programa una recurrencia de excepción.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el elemento de mes para el cual se programa una recurrencia de excepción. |

### setMonthPosition(int value) {#setMonthPosition-int-}
```
public final void setMonthPosition(int value)
```


Establece la posición de un elemento de mes dentro de un mes.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | la posición de un elemento de mes dentro de un mes. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Establece el nombre de la excepción.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el nombre de la excepción. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Establece el número de ocurrencias para las que la excepción del calendario es válida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el número de ocurrencias para las que la excepción de calendario es válida. |

### setPeriod(int value) {#setPeriod-int-}
```
public final void setPeriod(int value)
```


Establece el período de recurrencia de la excepción.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el período de recurrencia de la excepción. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


Establece el final del tiempo de la excepción.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | el final del tiempo de la excepción. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Establece el tipo de excepción.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el tipo de excepción. |

### setWorkingTimes(WorkingTimeCollection value) {#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-}
```
public final void setWorkingTimes(WorkingTimeCollection value)
```


Establece el objeto WorkingTimeCollection. La colección de tiempos de trabajo que define el tiempo trabajado en el día de la semana.

--------------------

Debe haber al menos un tiempo de trabajo presente, y no puede haber más de cinco.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) | el objeto WorkingTimeCollection. |

