---
title: "TaskCollection"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una colección de objetos."
type: docs
weight: 293
url: /es/java/com.aspose.tasks/taskcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskCollection extends AbstractList<Task>
```

Representa una colección de [Task](../../com.aspose.tasks/task) objetos.
## Métodos

| Método | Descripción |
| --- | --- |
| [add()](#add--) | Agrega una nueva tarea a la colección de tareas del proyecto en el mismo nivel de esquema que la última tarea. |
| [add(RecurringTaskParameters parameters)](#add-com.aspose.tasks.RecurringTaskParameters-) | Inserta una nueva tarea antes de una tarea con el id especificado y en el mismo nivel de esquema. |
| [add(Task item)](#add-com.aspose.tasks.Task-) | Agrega la tarea especificada a la instancia de la clase [TaskCollection](../../com.aspose.tasks/taskcollection). |
| [add(String taskName)](#add-java.lang.String-) | Agrega una nueva tarea a la colección de tareas hijas. |
| [add(String taskName, int beforeTaskId)](#add-java.lang.String-int-) | Agrega una nueva tarea recurrente a la colección de tareas hijas. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Task item)](#contains-com.aspose.tasks.Task-) | Comprueba si la colección contiene el elemento especificado. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | Devuelve una tarea con el Id especificado cuyo ancestro es la tarea padre de esta colección. |
| [getByUid(int uid)](#getByUid-int-) | Devuelve una tarea con el Uid especificado cuyo ancestro es la tarea padre de esta colección. |
| [getParentProject()](#getParentProject--) | Obtiene el proyecto padre del objeto TaskCollection. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Obtiene un valor que indica si esta colección es de solo lectura. |
| [iterator()](#iterator--) | Devuelve un enumerador para esta colección. |
| [remove(Object item)](#remove-java.lang.Object-) | Esta es la implementación de sustituto del método Remove de ICollection, que solo lanza UnsupportedOperationException |
| [size()](#size--) | Obtiene el número de objetos contenidos en el TaskCollection. |
| [sort(Comparator&lt;? super Task&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.Task--) | \{@inheritDoc\} |
| [toList()](#toList--) | Convierte el objeto TaskCollection en una lista de objetos [Task](../../com.aspose.tasks/task). |
### add() {#add--}
```
public final Task add()
```


Agrega una nueva tarea a la colección de tareas del proyecto en el mismo nivel de esquema que la última tarea.

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(RecurringTaskParameters parameters) {#add-com.aspose.tasks.RecurringTaskParameters-}
```
public final Task add(RecurringTaskParameters parameters)
```


Inserta una nueva tarea antes de una tarea con el id especificado y en el mismo nivel de esquema.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| parameters | [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) | Los parámetros especificados para la creación de una tarea recurrente. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(Task item) {#add-com.aspose.tasks.Task-}
```
public final boolean add(Task item)
```


Agregue la tarea especificada a la instancia de la clase [TaskCollection](../../com.aspose.tasks/taskcollection). Si ParentProject.CalculationMode es None, el usuario debe invocar Project.Recalculate() después de usar este método (Reprogramará todas las tareas del proyecto (fechas de inicio/fin, establece fechas tempranas/tardías) y calculará los campos dependientes como holguras, campos de trabajo y costo, IDs y niveles de esquema). Si ParentProject.CalculationMode es Manual, el método calculará solo el ID de la tarea, el nivel de esquema y los números de esquema automáticamente. Si ParentProject.CalculationMode es Automatic, el método reprograma automáticamente todas las tareas del proyecto (fechas de inicio/fin, establece fechas tempranas/tardías, calcula holguras, campos de trabajo y costo, recalcula IDs y niveles de esquema).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | la tarea especificada que debe agregarse a esta colección de tareas. |

**Returns:**
boolean - true si la operación fue exitosa.
### add(String taskName) {#add-java.lang.String-}
```
public final Task add(String taskName)
```


Agrega una nueva tarea a la colección de tareas hijas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| taskName | java.lang.String | el nombre de la tarea especificada. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(String taskName, int beforeTaskId) {#add-java.lang.String-int-}
```
public final Task add(String taskName, int beforeTaskId)
```


Agrega una nueva tarea recurrente a la colección de tareas hijas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| taskName | java.lang.String | el nombre de la tarea especificada. |
| beforeTaskId | int | El ID especificado de una tarea antes del cual se insertará una nueva tarea. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns a task which was inserted before a task with the specified id.
### clear() {#clear--}
```
public final void clear()
```




### contains(Task item) {#contains-com.aspose.tasks.Task-}
```
public final boolean contains(Task item)
```


Comprueba si la colección contiene el elemento especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | El elemento a comprobar. |

**Returns:**
boolean - true, si la colección contiene un elemento, false en caso contrario.
### get(int index) {#get-int-}
```
public Task get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | \{@inheritDoc\} |

**Returns:**
[Task](../../com.aspose.tasks/task) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Task getById(int id)
```


Devuelve una tarea con el Id especificado cuyo ancestro es la tarea padre de esta colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| id | int | TaskEntity Id |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified id whose ancestor is parent task of this collection.
### getByUid(int uid) {#getByUid-int-}
```
public final Task getByUid(int uid)
```


Devuelve una tarea con el Uid especificado cuyo ancestro es la tarea padre de esta colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | int | TaskEntity Uid. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified uid whose ancestor is parent task of this collection.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Obtiene el proyecto padre del objeto TaskCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the TaskCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Obtiene un valor que indica si esta colección es de solo lectura.

**Returns:**
boolean - un valor que indica si esta colección es de solo lectura.
### iterator() {#iterator--}
```
public final Iterator<Task> iterator()
```


Devuelve un enumerador para esta colección.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Task&gt; - un enumerador para esta colección.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Esta es la implementación de sustituto del método Remove de ICollection, que solo lanza UnsupportedOperationException

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | java.lang.Object | El elemento a eliminar. |

**Returns:**
boolean - `true` si el elemento fue eliminado; `false` de lo contrario.
### size() {#size--}
```
public final int size()
```


Obtiene el número de objetos contenidos en el TaskCollection.

**Returns:**
int - el número de objetos contenidos en la TaskCollection.
### sort(Comparator&lt;? super Task&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.Task--}
```
public final void sort(Comparator<? super Task> c)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.Task&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Task> toList()
```


Convierte el objeto TaskCollection en una lista de objetos [Task](../../com.aspose.tasks/task).

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - devuelve una lista que contiene las instancias de la clase [Task](../../com.aspose.tasks/task) de esta colección.
