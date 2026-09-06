---
title: "ICalendar"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una abstracción de calendario que puede usarse para varios cálculos de fechas y duraciones."
type: docs
weight: 376
url: /es/java/com.aspose.tasks/icalendar/
---
```
public interface ICalendar
```

Representa una abstracción de calendario que puede usarse para varios cálculos de fechas y duraciones.
## Métodos

| Método | Descripción |
| --- | --- |
| [getFinishDateByStartAndWork(Date start, Duration work)](#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-) | Calcula la fecha en que el tiempo de trabajo especificado transcurrirá según el calendario. |
| [getFinishDateByStartAndWork(Date start, double work)](#getFinishDateByStartAndWork-java.util.Date-double-) | Calcula la fecha en que el tiempo de trabajo especificado transcurrirá según el calendario. |
| [getNextWorkingDayStart(Date date)](#getNextWorkingDayStart-java.util.Date-) | Calcula el inicio del siguiente día laborable para la fecha especificada. |
| [getPreviousWorkingDayEnd(Date date)](#getPreviousWorkingDayEnd-java.util.Date-) | Calcula el fin de la fecha laborable anterior a partir de la fecha especificada. |
| [getStartDateFromFinishAndDuration(Date finish, Duration duration)](#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-) | Devuelve la fecha de inicio basada en la fecha de finalización y duración especificadas. |
| [getStartDateFromFinishAndDuration(Date finish, double duration)](#getStartDateFromFinishAndDuration-java.util.Date-double-) | Devuelve la fecha de inicio basada en la fecha de finalización y duración especificadas. |
| [getTaskFinishDateFromDuration(Task task, double duration)](#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-) | Calcula la fecha y hora de finalización de la tarea a partir de su fecha de inicio, partes divididas y la duración del trabajo. |
| [getWorkStart(Date date)](#getWorkStart-java.util.Date-) | Calcula el inicio del siguiente tiempo laborable a partir de la fecha y hora especificadas. |
| [getWorkingHours(Date dt)](#getWorkingHours-java.util.Date-) | Devuelve la cantidad de horas laborables en la fecha especificada. |
| [getWorkingHours(Date start, Date finish)](#getWorkingHours-java.util.Date-java.util.Date-) | Devuelve WorkUnit - Inicio, Fin y Duración de las horas laborables para el intervalo de fecha y hora especificado. |
| [getWorkingHoursTimeSpan(Date start, Date finish)](#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-) | Devuelve la cantidad de horas laborables entre las fechas especificadas. |
| [getWorkingTimes(Date dt)](#getWorkingTimes-java.util.Date-) | Devuelve [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) de tiempos laborables para la fecha especificada. |
| [isDayWorking(Date dt)](#isDayWorking-java.util.Date-) | Determina si el día especificado es laborable según el calendario. |
| [isEmpty()](#isEmpty--) | Devuelve si el calendario no tiene horas laborables definidas. |
### getFinishDateByStartAndWork(Date start, Duration work) {#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getFinishDateByStartAndWork(Date start, Duration work)
```


Calcula la fecha en que el tiempo de trabajo especificado transcurrirá según el calendario.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | java.util.Date | Fecha de inicio. |
| work | [Duration](../../com.aspose.tasks/duration) | Duración del trabajo. |

**Returns:**
java.util.Date - Fecha de finalización.
### getFinishDateByStartAndWork(Date start, double work) {#getFinishDateByStartAndWork-java.util.Date-double-}
```
public abstract Date getFinishDateByStartAndWork(Date start, double work)
```


Calcula la fecha en que el tiempo de trabajo especificado transcurrirá según el calendario.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | java.util.Date | Fecha de inicio. |
| trabajo | double | Duración del trabajo. |

**Returns:**
java.util.Date - Fecha de finalización.
### getNextWorkingDayStart(Date date) {#getNextWorkingDayStart-java.util.Date-}
```
public abstract Date getNextWorkingDayStart(Date date)
```


Calcula el inicio del siguiente día laborable para la fecha especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fecha | java.util.Date | La fecha para obtener el inicio del siguiente día laborable. |

**Returns:**
java.util.Date - Inicio del siguiente día laborable System.DateTime.
### getPreviousWorkingDayEnd(Date date) {#getPreviousWorkingDayEnd-java.util.Date-}
```
public abstract Date getPreviousWorkingDayEnd(Date date)
```


Calcula el fin de la fecha laborable anterior a partir de la fecha especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fecha | java.util.Date | la fecha para calcular el final del día laborable anterior. |

**Returns:**
java.util.Date - El final del día laborable anterior
### getStartDateFromFinishAndDuration(Date finish, Duration duration) {#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, Duration duration)
```


Devuelve la fecha de inicio basada en la fecha de finalización y duración especificadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| finalizar | java.util.Date | La fecha de finalización especificada. |
| duration | [Duration](../../com.aspose.tasks/duration) | La duración especificada. |

**Returns:**
java.util.Date - Fecha de inicio calculada.
### getStartDateFromFinishAndDuration(Date finish, double duration) {#getStartDateFromFinishAndDuration-java.util.Date-double-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, double duration)
```


Devuelve la fecha de inicio basada en la fecha de finalización y duración especificadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| finalizar | java.util.Date | La fecha de finalización especificada. |
| duración | double | La duración especificada. |

**Returns:**
java.util.Date - Fecha de inicio calculada.
### getTaskFinishDateFromDuration(Task task, double duration) {#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-}
```
public abstract Date getTaskFinishDateFromDuration(Task task, double duration)
```


Calcula la fecha y hora de finalización de la tarea a partir de su fecha de inicio, partes divididas y la duración del trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | La tarea para la cual calcular la fecha de finalización. |
|  | duración | double | La duración a calcular. |

Devuelve DateTime.MinValue si la tarea es un resumen, nula o su fecha de inicio no está establecida. |

**Returns:**
java.util.Date - Fecha de finalización de la tarea para la fecha de inicio y duración dadas.
### getWorkStart(Date date) {#getWorkStart-java.util.Date-}
```
public abstract Date getWorkStart(Date date)
```


Calcula el inicio del siguiente tiempo laborable a partir de la fecha y hora especificadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fecha | java.util.Date | La fecha y hora. |

**Returns:**
java.util.Date - El inicio del tiempo laborable más cercano.
### getWorkingHours(Date dt) {#getWorkingHours-java.util.Date-}
```
public abstract double getWorkingHours(Date dt)
```


Devuelve la cantidad de horas laborables en la fecha especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dt | java.util.Date | La fecha para obtener las horas laborables. |

**Returns:**
double - Horas laborables en la fecha especificada.
### getWorkingHours(Date start, Date finish) {#getWorkingHours-java.util.Date-java.util.Date-}
```
public abstract WorkUnit getWorkingHours(Date start, Date finish)
```


Devuelve WorkUnit - Inicio, Fin y Duración de las horas laborables para el intervalo de fecha y hora especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | java.util.Date | Fecha de inicio del intervalo. |
| finalizar | java.util.Date | Fecha de finalización del intervalo. |

**Returns:**
[WorkUnit](../../com.aspose.tasks/workunit) - Instance of [WorkUnit](../../com.aspose.tasks/workunit) class containing Start, Finish and Duration of working hours.
### getWorkingHoursTimeSpan(Date start, Date finish) {#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-}
```
public abstract double getWorkingHoursTimeSpan(Date start, Date finish)
```


Devuelve la cantidad de horas laborables entre las fechas especificadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | java.util.Date | Fecha de inicio del intervalo. |
| finalizar | java.util.Date | Fecha de finalización del intervalo. |

**Returns:**
double - Cantidad de horas laborables según la instancia del calendario.
### getWorkingTimes(Date dt) {#getWorkingTimes-java.util.Date-}
```
public abstract WorkingTimeCollection getWorkingTimes(Date dt)
```


Devuelve [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) de tiempos laborables para la fecha especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dt | java.util.Date | La fecha para obtener los horarios laborables. |

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - Collection of [WorkingTime](../../com.aspose.tasks/workingtime) instances.
### isDayWorking(Date dt) {#isDayWorking-java.util.Date-}
```
public abstract boolean isDayWorking(Date dt)
```


Determina si el día especificado es laborable según el calendario.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dt | java.util.Date | La fecha para comprobar si el día es laborable. |

**Returns:**
boolean - Verdadero si el día es laborable.
### isEmpty() {#isEmpty--}
```
public abstract boolean isEmpty()
```


Devuelve si el calendario no tiene horas laborables definidas.

**Returns:**
boolean - Verdadero si el calendario no tiene horas laborables definidas.
