---
title: "TaskLink"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un enlace de predecesor."
type: docs
weight: 295
url: /es/java/com.aspose.tasks/tasklink/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public final class TaskLink implements System.IEquatable<TaskLink>
```

Representa un enlace de predecesor.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(TaskLink other)](#equals-com.aspose.tasks.TaskLink-) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [equals(Object obj)](#equals-java.lang.Object-) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [getCrossProjectName()](#getCrossProjectName--) | Obtiene el proyecto predecesor externo. |
| [getLagFormat()](#getLagFormat--) | Obtiene el formato para expresar el formato de retardo. |
| [getLinkLag()](#getLinkLag--) | Obtiene el retardo en décimas de minuto o porcentaje. |
| [getLinkLagTimeSpan()](#getLinkLagTimeSpan--) | Obtiene la duración del retardo, según LagFormat. |
| [getLinkType()](#getLinkType--) | Obtiene el tipo de un enlace. |
| [getPredTask()](#getPredTask--) | Obtiene la tarea predecesora. |
| [getSuccTask()](#getSuccTask--) | Obtiene la tarea sucesora. |
| [hashCode()](#hashCode--) | Devuelve un valor de código hash para la instancia de la clase [TaskLink](../../com.aspose.tasks/tasklink). |
| [isCrossProject()](#isCrossProject--) | Obtiene un valor que indica si un predecesor forma parte de otro proyecto. |
| [setCrossProject(boolean value)](#setCrossProject-boolean-) | Establece un valor que indica si un predecesor forma parte de otro proyecto. |
| [setCrossProjectName(String value)](#setCrossProjectName-java.lang.String-) | Establece el proyecto predecesor externo. |
| [setLagFormat(byte value)](#setLagFormat-byte-) | Establece el formato para expresar el formato de retardo. |
| [setLinkLag(int value)](#setLinkLag-int-) | Establece el retardo en décimas de minuto o porcentaje. |
| [setLinkLagTimeSpan(double value)](#setLinkLagTimeSpan-double-) | Establece la duración del retardo, según LagFormat. |
| [setLinkType(int value)](#setLinkType-int-) | Establece el tipo de un enlace. |
| [setPredTask(Task value)](#setPredTask-com.aspose.tasks.Task-) | Establece la tarea predecesora. |
| [setSuccTask(Task value)](#setSuccTask-com.aspose.tasks.Task-) | Establece la tarea sucesora. |
| [toString()](#toString--) | Devuelve la representación en cadena de un TaskLink. |
### equals(TaskLink other) {#equals-com.aspose.tasks.TaskLink-}
```
public final boolean equals(TaskLink other)
```


Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | [TaskLink](../../com.aspose.tasks/tasklink) | La instancia especificada de la clase [TaskLink](../../com.aspose.tasks/tasklink) para comparar con esta instancia. |

**Returns:**
boolean - **True** si la instancia especificada de la clase [TaskLink](../../com.aspose.tasks/tasklink) tiene las mismas tareas predecesoras y sucesoras que esta instancia; de lo contrario, **false**.
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
boolean - **True** si el objeto especificado es un TaskLink que tiene el mismo predecesor y sucesor que esta instancia; de lo contrario, **false**.
### getCrossProjectName() {#getCrossProjectName--}
```
public final String getCrossProjectName()
```


Obtiene el proyecto predecesor externo.

**Returns:**
java.lang.String - el proyecto predecesor externo.
### getLagFormat() {#getLagFormat--}
```
public final byte getLagFormat()
```


Obtiene el formato para expresar el formato de retardo.

**Returns:**
byte - el formato para expresar el formato de retraso.
### getLinkLag() {#getLinkLag--}
```
public final int getLinkLag()
```


Obtiene el retardo en décimas de minuto o porcentaje.

**Returns:**
int - el retraso en décimas de minuto o porcentaje.
### getLinkLagTimeSpan() {#getLinkLagTimeSpan--}
```
public final double getLinkLagTimeSpan()
```


Obtiene la duración del retardo, según LagFormat.

**Returns:**
double - duración del retraso, según LagFormat.
### getLinkType() {#getLinkType--}
```
public final int getLinkType()
```


Obtiene el tipo de un enlace.

**Returns:**
int - el tipo de un enlace.
### getPredTask() {#getPredTask--}
```
public final Task getPredTask()
```


Obtiene la tarea predecesora.

**Returns:**
[Task](../../com.aspose.tasks/task) - the predecessor task.
### getSuccTask() {#getSuccTask--}
```
public final Task getSuccTask()
```


Obtiene la tarea sucesora.

**Returns:**
[Task](../../com.aspose.tasks/task) - the successor task.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Devuelve un valor de código hash para la instancia de la clase [TaskLink](../../com.aspose.tasks/tasklink).

**Returns:**
int - devuelve un valor de código hash para este objeto.
### isCrossProject() {#isCrossProject--}
```
public final boolean isCrossProject()
```


Obtiene un valor que indica si un predecesor forma parte de otro proyecto.

**Returns:**
boolean - un valor que indica si un predecesor forma parte de otro proyecto.
### setCrossProject(boolean value) {#setCrossProject-boolean-}
```
public final void setCrossProject(boolean value)
```


Establece un valor que indica si un predecesor forma parte de otro proyecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si un predecesor forma parte de otro proyecto. |

### setCrossProjectName(String value) {#setCrossProjectName-java.lang.String-}
```
public final void setCrossProjectName(String value)
```


Establece el proyecto predecesor externo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el proyecto predecesor externo. |

### setLagFormat(byte value) {#setLagFormat-byte-}
```
public final void setLagFormat(byte value)
```


Establece el formato para expresar el formato de retardo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | byte | el formato para expresar el formato de retraso. |

### setLinkLag(int value) {#setLinkLag-int-}
```
public final void setLinkLag(int value)
```


Establece el retardo en décimas de minuto o porcentaje.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el retraso en décimas de minuto o porcentaje. |

### setLinkLagTimeSpan(double value) {#setLinkLagTimeSpan-double-}
```
public final void setLinkLagTimeSpan(double value)
```


Establece la duración del retardo, según LagFormat.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | duración del retraso, según LagFormat. |

### setLinkType(int value) {#setLinkType-int-}
```
public final void setLinkType(int value)
```


Establece el tipo de un enlace.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el tipo de un enlace. |

### setPredTask(Task value) {#setPredTask-com.aspose.tasks.Task-}
```
public final void setPredTask(Task value)
```


Establece la tarea predecesora.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | la tarea predecesora. |

### setSuccTask(Task value) {#setSuccTask-com.aspose.tasks.Task-}
```
public final void setSuccTask(Task value)
```


Establece la tarea sucesora.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | la tarea sucesora. |

### toString() {#toString--}
```
public String toString()
```


Devuelve la representación en cadena de un TaskLink. Los detalles exactos de la representación no están especificados y pueden cambiar.

**Returns:**
java.lang.String - cadena que representa el objeto TaskLink.
