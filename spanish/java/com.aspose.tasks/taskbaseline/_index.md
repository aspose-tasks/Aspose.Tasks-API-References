---
title: "TaskBaseline"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa la línea base de una tarea."
type: docs
weight: 291
url: /es/java/com.aspose.tasks/taskbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)

**All Implemented Interfaces:**
java.lang.Comparable
```
public class TaskBaseline extends Baseline implements Comparable<Baseline>
```

Representa la línea base de una tarea.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [TaskBaseline(Task task)](#TaskBaseline-com.aspose.tasks.Task-) | Inicializa una nueva instancia de la clase [TaskBaseline](../../com.aspose.tasks/taskbaseline). |
## Métodos

| Método | Descripción |
| --- | --- |
| [compareTo(TaskBaseline other)](#compareTo-com.aspose.tasks.TaskBaseline-) | Implementación de la interfaz IComparable. |
| [equals(TaskBaseline other)](#equals-com.aspose.tasks.TaskBaseline-) | Devuelve un valor que indica si esta instancia es igual al objeto TaskBaseline especificado. |
| [equals(Object obj)](#equals-java.lang.Object-) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [getDuration()](#getDuration--) | Obtiene la duración programada de la tarea cuando se guardó la línea base. |
| [getEstimatedDuration()](#getEstimatedDuration--) | Obtiene un valor que indica si la duración de la línea base de la tarea fue estimada. |
| [getFinish()](#getFinish--) | Obtiene la fecha de finalización programada de la tarea cuando se guardó la línea base. |
| [getFixedCost()](#getFixedCost--) | Obtiene un costo fijo de la tarea cuando se guardó la línea base. |
| [getInterim()](#getInterim--) | Obtiene un valor que indica si esta es una línea base intermedia. |
| [getStart()](#getStart--) | Obtiene la fecha de inicio programada de la tarea cuando se guardó la línea base. |
| [getTimephasedData()](#getTimephasedData--) | Obtiene una instancia de TimephasedDataCollection para este objeto. |
| [hashCode()](#hashCode--) | Devuelve un valor de código hash para la instancia de la clase [TaskBaseline](../../com.aspose.tasks/taskbaseline). |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Establece la duración programada de la tarea cuando se guardó la línea base. |
| [setEstimatedDuration(boolean value)](#setEstimatedDuration-boolean-) | Establece un valor que indica si la duración de la línea base de la tarea fue estimada. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Establece la fecha de finalización programada de la tarea cuando se guardó la línea base. |
| [setFixedCost(double value)](#setFixedCost-double-) | Establece un costo fijo de la tarea cuando se guardó la línea base. |
| [setInterim(boolean value)](#setInterim-boolean-) | Establece un valor que indica si esta es una Línea Base Intermedia. |
| [setStart(Date value)](#setStart-java.util.Date-) | Establece la fecha de inicio programada de la tarea cuando se guardó la línea base. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Establece una instancia de TimephasedDataCollection para este objeto. |
### TaskBaseline(Task task) {#TaskBaseline-com.aspose.tasks.Task-}
```
public TaskBaseline(Task task)
```


Inicializa una nueva instancia de la clase [TaskBaseline](../../com.aspose.tasks/taskbaseline).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Tarea principal de la línea base. |

### compareTo(TaskBaseline other) {#compareTo-com.aspose.tasks.TaskBaseline-}
```
public final int compareTo(TaskBaseline other)
```


Implementación de la interfaz IComparable. Compara esta instancia con el objeto Baseline especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | el objeto Baseline especificado con el que comparar esta instancia. |

**Returns:**
int - devuelve -1 si esta instancia es menor que el objeto especificado, 1 si esta instancia es mayor que el objeto especificado; de lo contrario devuelve 0
### equals(TaskBaseline other) {#equals-com.aspose.tasks.TaskBaseline-}
```
public final boolean equals(TaskBaseline other)
```


Devuelve un valor que indica si esta instancia es igual al objeto TaskBaseline especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | el objeto AssignmentBaseline especificado para comparar con esta instancia. |

**Returns:**
boolean - devuelve true si esta instancia es igual al objeto TaskBaseline especificado; de lo contrario, false.
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
boolean - **True** si el objeto especificado es un TaskBaseline que tiene el mismo valor UID que esta instancia; de lo contrario, **false**.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Obtiene la duración programada de la tarea cuando se guardó la línea base.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the scheduled duration of the task when the baseline was saved.
### getEstimatedDuration() {#getEstimatedDuration--}
```
public final boolean getEstimatedDuration()
```


Obtiene un valor que indica si la duración de la línea base de la tarea fue estimada.

**Returns:**
boolean - un valor que indica si la duración de la línea base de la tarea fue estimada.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Obtiene la fecha de finalización programada de la tarea cuando se guardó la línea base.

**Returns:**
java.util.Date - la fecha de finalización programada de la tarea cuando se guardó la línea base.
### getFixedCost() {#getFixedCost--}
```
public final double getFixedCost()
```


Obtiene un costo fijo de la tarea cuando se guardó la línea base.

**Returns:**
double - un costo fijo de la tarea cuando se guardó la línea base.
### getInterim() {#getInterim--}
```
public final boolean getInterim()
```


Obtiene un valor que indica si esta es una línea base intermedia.

**Returns:**
boolean - un valor que indica si esta es una Línea Base Intermedia.
### getStart() {#getStart--}
```
public final Date getStart()
```


Obtiene la fecha de inicio programada de la tarea cuando se guardó la línea base.

**Returns:**
java.util.Date - la fecha de inicio programada de la tarea cuando se guardó la línea base.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Obtiene una instancia de TimephasedDataCollection para este objeto. Los datos temporales asociados con la línea base de la tarea.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - a TimephasedDataCollection instance for this object.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Devuelve un valor de código hash para la instancia de la clase [TaskBaseline](../../com.aspose.tasks/taskbaseline).

**Returns:**
int - devuelve un valor de código hash para este objeto.
### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Establece la duración programada de la tarea cuando se guardó la línea base.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | la duración programada de la tarea cuando se guardó la línea base. |

### setEstimatedDuration(boolean value) {#setEstimatedDuration-boolean-}
```
public final void setEstimatedDuration(boolean value)
```


Establece un valor que indica si la duración de la línea base de la tarea fue estimada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si la duración de la línea base de la tarea fue estimada. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Establece la fecha de finalización programada de la tarea cuando se guardó la línea base.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | la fecha de finalización programada de la tarea cuando se guardó la línea base. |

### setFixedCost(double value) {#setFixedCost-double-}
```
public final void setFixedCost(double value)
```


Establece un costo fijo de la tarea cuando se guardó la línea base.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | un costo fijo de la tarea cuando se guardó la línea base. |

### setInterim(boolean value) {#setInterim-boolean-}
```
public final void setInterim(boolean value)
```


Establece un valor que indica si esta es una Línea Base Intermedia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si esta es una Línea Base Intermedia. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Establece la fecha de inicio programada de la tarea cuando se guardó la línea base.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | la fecha de inicio programada de la tarea cuando se guardó la línea base. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Establece una instancia de TimephasedDataCollection para este objeto. Los datos temporales asociados con la línea base de la tarea.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | una instancia de TimephasedDataCollection para este objeto. |

