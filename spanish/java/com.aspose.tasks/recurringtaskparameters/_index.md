---
title: "RecurringTaskParameters"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa el conjunto de parámetros que se utilizan para crear una tarea recurrente en un proyecto."
type: docs
weight: 245
url: /es/java/com.aspose.tasks/recurringtaskparameters/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskParameters
```

Representa el conjunto de parámetros que se utilizan para crear una tarea recurrente en un proyecto.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [RecurringTaskParameters()](#RecurringTaskParameters--) | Inicializa una nueva instancia de la clase [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getDuration()](#getDuration--) | Obtiene la duración de una ocurrencia de la tarea recurrente. |
| [getIgnoreResourceCalendar()](#getIgnoreResourceCalendar--) | Obtiene un valor que indica si se debe programar la tarea recurrente incluso si no ocurre cuando hay recursos disponibles para trabajar en ella. |
| [getRecurrencePattern()](#getRecurrencePattern--) | Obtiene el patrón de recurrencia de la tarea recurrente. |
| [getTaskName()](#getTaskName--) | Obtiene el nombre de la tarea recurrente. |
| [setCalendar(Project project, String calendarName)](#setCalendar-com.aspose.tasks.Project-java.lang.String-) | Establece un calendario para la tarea recurrente. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Establece la duración de una ocurrencia de la tarea recurrente. |
| [setIgnoreResourceCalendar(boolean value)](#setIgnoreResourceCalendar-boolean-) | Establece un valor que indica si se debe programar la tarea recurrente incluso si no ocurre cuando hay recursos disponibles para trabajar en ella. |
| [setRecurrencePattern(RecurrencePatternBase value)](#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-) | Establece el patrón de recurrencia de la tarea recurrente. |
| [setTaskName(String value)](#setTaskName-java.lang.String-) | Establece el nombre de la tarea recurrente. |
### RecurringTaskParameters() {#RecurringTaskParameters--}
```
public RecurringTaskParameters()
```


Inicializa una nueva instancia de la clase [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters).

### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Obtiene la duración de una ocurrencia de la tarea recurrente.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - The instance of `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) class.
### getIgnoreResourceCalendar() {#getIgnoreResourceCalendar--}
```
public final boolean getIgnoreResourceCalendar()
```


Obtiene un valor que indica si se debe programar la tarea recurrente incluso si no ocurre cuando hay recursos disponibles para trabajar en ella.

**Returns:**
boolean - un valor que indica si programar la tarea recurrente incluso si no ocurre cuando hay recursos disponibles para trabajar en ella.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final RecurrencePatternBase getRecurrencePattern()
```


Obtiene el patrón de recurrencia de la tarea recurrente.

--------------------

Puede ser uno de los valores de `RecurrencePattern`([getRecurrencePattern()](../../com.aspose/tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose/tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)) enumeración.

**Returns:**
[RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) - the recurrence pattern of the recurring task.
### getTaskName() {#getTaskName--}
```
public final String getTaskName()
```


Obtiene el nombre de la tarea recurrente.

**Returns:**
java.lang.String - el nombre de la tarea recurrente.
### setCalendar(Project project, String calendarName) {#setCalendar-com.aspose.tasks.Project-java.lang.String-}
```
public final void setCalendar(Project project, String calendarName)
```


Establezca un calendario para la tarea recurrente. El calendario se selecciona de la colección de calendarios del proyecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | El proyecto con la colección de calendarios. |
| calendarName | java.lang.String | El nombre del calendario. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Establece la duración de una ocurrencia de la tarea recurrente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | La instancia de `Duration`([getDuration()](../../com.aspose/tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose/tasks/recurringtaskparameters\#setDuration-Duration-)) clase. |

### setIgnoreResourceCalendar(boolean value) {#setIgnoreResourceCalendar-boolean-}
```
public final void setIgnoreResourceCalendar(boolean value)
```


Establece un valor que indica si se debe programar la tarea recurrente incluso si no ocurre cuando hay recursos disponibles para trabajar en ella.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si programar la tarea recurrente incluso si no ocurre cuando hay recursos disponibles para trabajar en ella. |

### setRecurrencePattern(RecurrencePatternBase value) {#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-}
```
public final void setRecurrencePattern(RecurrencePatternBase value)
```


Establece el patrón de recurrencia de la tarea recurrente.

--------------------

Puede ser uno de los valores de `RecurrencePattern`([getRecurrencePattern()](../../com.aspose/tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose/tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)) enumeración.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) | el patrón de recurrencia de la tarea recurrente. |

### setTaskName(String value) {#setTaskName-java.lang.String-}
```
public final void setTaskName(String value)
```


Establece el nombre de la tarea recurrente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el nombre de la tarea recurrente. |

