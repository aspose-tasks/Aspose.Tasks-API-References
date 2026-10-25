---
title: "SimpleSaveOptions"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Esta es una clase base abstracta que permite al usuario especificar opciones básicas al guardar un proyecto en un formato particular."
type: docs
weight: 277
url: /es/java/com.aspose.tasks/simplesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SimpleSaveOptions
```

Esta es una clase base abstracta que permite al usuario especificar opciones básicas al guardar un proyecto en un formato particular.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [SimpleSaveOptions()](#SimpleSaveOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [getSaveFormat()](#getSaveFormat--) | Obtiene el formato en el que se guardará el documento si se utiliza este objeto de opciones de guardado. |
| [getTasksComparer()](#getTasksComparer--) | Obtiene el comparador para ordenar tareas en el diagrama de Gantt y en el diagrama de hoja de tareas. |
| [getTasksFilter()](#getTasksFilter--) | Obtiene la condición que se usa para filtrar tareas representadas en los diagramas de Gantt, hoja de tareas y uso de tareas. |
| [setTasksComparer(Comparator&lt;Task&gt; value)](#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--) | Establece el comparador para ordenar tareas en el diagrama de Gantt y en el diagrama de hoja de tareas. |
| [setTasksFilter(ICondition&lt;Task&gt; value)](#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Establece la condición que se usa para filtrar tareas representadas en los diagramas de Gantt, hoja de tareas y uso de tareas. |
### SimpleSaveOptions() {#SimpleSaveOptions--}
```
public SimpleSaveOptions()
```


### getSaveFormat() {#getSaveFormat--}
```
public final int getSaveFormat()
```


Obtiene el formato en el que se guardará el documento si se utiliza este objeto de opciones de guardado.

**Returns:**
int - el [SaveFileFormat](../../com.aspose.tasks/savefileformat) en el que se guardará el documento.
### getTasksComparer() {#getTasksComparer--}
```
public final Comparator<Task> getTasksComparer()
```


Obtiene el comparador para ordenar tareas en el diagrama de Gantt y en el diagrama de hoja de tareas.

**Returns:**
java.util.Comparator&lt;com.aspose.tasks.Task&gt; - el comparador para ordenar tareas en el diagrama de Gantt y en el diagrama de hoja de tareas.
### getTasksFilter() {#getTasksFilter--}
```
public final ICondition<Task> getTasksFilter()
```


Obtiene la condición que se usa para filtrar tareas representadas en los diagramas de Gantt, hoja de tareas y uso de tareas.

--------------------

Si no se especifica un valor, se utiliza el filtro predeterminado que elimina las tareas no visibles -- es decir, las tareas descendientes de tareas colapsadas.

**Returns:**
[ICondition](../../com.aspose.tasks/icondition) - the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts.
### setTasksComparer(Comparator&lt;Task&gt; value) {#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--}
```
public final void setTasksComparer(Comparator<Task> value)
```


Establece el comparador para ordenar tareas en el diagrama de Gantt y en el diagrama de hoja de tareas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Comparator&lt;com.aspose.tasks.Task&gt; | el comparador para ordenar tareas en el diagrama de Gantt y en el diagrama de hoja de tareas. |

### setTasksFilter(ICondition&lt;Task&gt; value) {#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public final void setTasksFilter(ICondition<Task> value)
```


Establece la condición que se usa para filtrar tareas representadas en los diagramas de Gantt, hoja de tareas y uso de tareas.

--------------------

Si no se especifica un valor, se utiliza el filtro predeterminado que elimina las tareas no visibles -- es decir, las tareas descendientes de tareas colapsadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | la condición que se usa para filtrar tareas mostradas en los gráficos de Gantt, Hoja de tareas y Uso de tareas. |

