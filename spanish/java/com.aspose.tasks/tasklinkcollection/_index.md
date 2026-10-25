---
title: "TaskLinkCollection"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una colección de objetos."
type: docs
weight: 296
url: /es/java/com.aspose.tasks/tasklinkcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskLinkCollection extends AbstractList<TaskLink>
```

Representa una colección de [Task](../../com.aspose.tasks/task) objetos.
## Métodos

| Método | Descripción |
| --- | --- |
| [add(Task pred, Task succ)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-) | Devuelve una instancia de Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) que ha sido añadida al objeto TaskLinkCollection. |
| [add(Task pred, Task succ, int linkType)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-) | Devuelve una instancia de [TaskLink](../../com.aspose.tasks/tasklink) que ha sido añadida al objeto TaskLinkCollection. |
| [add(Task pred, Task succ, int linkType, Duration lag)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-) | Devuelve una instancia de [TaskLink](../../com.aspose.tasks/tasklink) que ha sido añadida al objeto TaskLinkCollection. |
| [add(TaskLink e)](#add-com.aspose.tasks.TaskLink-) | Esta es la implementación de sustituto del método Add de ICollection, que solo lanza UnsupportedOperationException |
| [clear()](#clear--) | Reservado para uso interno. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getParentProject()](#getParentProject--) | Obtiene el proyecto padre del objeto ResourceAssignmentCollection. |
| [remove(int index)](#remove-int-) | Elimina el elemento en la posición especificada de esta colección y devuelve el elemento que fue eliminado de la colección. |
| [remove(Object item)](#remove-java.lang.Object-) | Elimina el enlace de tarea de un proyecto. |
| [size()](#size--) | Devuelve el número de objetos contenidos en este objeto `TaskLinkCollection`. |
| [sort(Comparator&lt;? super TaskLink&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--) | \{@inheritDoc\} |
| [toList()](#toList--) | Convierte el objeto TaskLinkCollection en una lista de objetos [TaskLink](../../com.aspose.tasks/tasklink). |
### add(Task pred, Task succ) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-}
```
public final TaskLink add(Task pred, Task succ)
```


Devuelve una instancia de Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) que ha sido añadida al objeto TaskLinkCollection.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Tarea predecesora. |
| succ | [Task](../../com.aspose.tasks/task) | Tarea sucesora. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-}
```
public final TaskLink add(Task pred, Task succ, int linkType)
```


Devuelve una instancia de [TaskLink](../../com.aspose.tasks/tasklink) que ha sido añadida al objeto TaskLinkCollection.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Tarea predecesora. |
| succ | [Task](../../com.aspose.tasks/task) | Tarea sucesora. |
| linkType | int | Tipo de enlace [TaskLinkType](../../com.aspose.tasks/tasklinktype) |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType, Duration lag) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-}
```
public final TaskLink add(Task pred, Task succ, int linkType, Duration lag)
```


Devuelve una instancia de [TaskLink](../../com.aspose.tasks/tasklink) que ha sido añadida al objeto TaskLinkCollection.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Tarea predecesora. |
| succ | [Task](../../com.aspose.tasks/task) | Tarea sucesora. |
| linkType | int | Tipo de enlace [TaskLinkType](../../com.aspose.tasks/tasklinktype) |
| lag | [Duration](../../com.aspose.tasks/duration) | Retardo del enlace [Duration](../../com.aspose.tasks/duration). |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link which has been added to this object.
### add(TaskLink e) {#add-com.aspose.tasks.TaskLink-}
```
public final boolean add(TaskLink e)
```


Esta es la implementación de sustituto del método Add de ICollection, que solo lanza UnsupportedOperationException

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| e | [TaskLink](../../com.aspose.tasks/tasklink) | El elemento a añadir. |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


Reservado para uso interno.

### get(int index) {#get-int-}
```
public TaskLink get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | \{@inheritDoc\} |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - \{@inheritDoc\}
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Obtiene el proyecto padre del objeto ResourceAssignmentCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent `Project` for this object.
### remove(int index) {#remove-int-}
```
public final TaskLink remove(int index)
```


Elimina el elemento en la posición especificada de esta colección y devuelve el elemento que fue eliminado de la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | la posición especificada para eliminar el elemento. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - the element that was removed from the collection.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Elimina el enlace de tarea de un proyecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | java.lang.Object | la instancia especificada de la clase `TaskLink` a eliminar. |

**Returns:**
boolean - devuelve la instancia de la clase `TaskLink` que fue eliminada de esta colección.
### size() {#size--}
```
public final int size()
```


Devuelve el número de objetos contenidos en este objeto `TaskLinkCollection`. Solo lectura `int`.

**Returns:**
int - devuelve el número de objetos contenidos en esta colección.
### sort(Comparator&lt;? super TaskLink&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--}
```
public void sort(Comparator<? super TaskLink> c)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.TaskLink&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<TaskLink> toList()
```


Convierte el objeto TaskLinkCollection en una lista de objetos [TaskLink](../../com.aspose.tasks/tasklink).

**Returns:**
java.util.List&lt;com.aspose.tasks.TaskLink&gt; - Lista de objetos [TaskLink](../../com.aspose.tasks/tasklink).
