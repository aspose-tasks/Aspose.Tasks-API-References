---
title: "TaskLinkCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una raccolta di oggetti."
type: docs
weight: 296
url: /it/java/com.aspose.tasks/tasklinkcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskLinkCollection extends AbstractList<TaskLink>
```

Rappresenta una raccolta di oggetti [Task](../../com.aspose.tasks/task).
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(Task pred, Task succ)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-) | Restituisce un'istanza di Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) che è stata aggiunta all'oggetto TaskLinkCollection. |
| [add(Task pred, Task succ, int linkType)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-) | Restituisce un'istanza di [TaskLink](../../com.aspose.tasks/tasklink) che è stata aggiunta all'oggetto TaskLinkCollection. |
| [add(Task pred, Task succ, int linkType, Duration lag)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-) | Restituisce un'istanza di [TaskLink](../../com.aspose.tasks/tasklink) che è stata aggiunta all'oggetto TaskLinkCollection. |
| [add(TaskLink e)](#add-com.aspose.tasks.TaskLink-) | Questa è l'implementazione stub del metodo Add di ICollection, che lancia solo UnsupportedOperationException |
| [clear()](#clear--) | Riservato per uso interno. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getParentProject()](#getParentProject--) | Ottiene il progetto padre dell'oggetto ResourceAssignmentCollection. |
| [remove(int index)](#remove-int-) | Rimuove l'elemento nella posizione specificata in questa raccolta e restituisce l'elemento che è stato rimosso dalla raccolta. |
| [remove(Object item)](#remove-java.lang.Object-) | Rimuove il collegamento di attività da un progetto. |
| [size()](#size--) | Restituisce il numero di oggetti contenuti in questo oggetto `TaskLinkCollection`. |
| [sort(Comparator&lt;? super TaskLink&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--) | \{@inheritDoc\} |
| [toList()](#toList--) | Converte l'oggetto TaskLinkCollection in un elenco di oggetti [TaskLink](../../com.aspose.tasks/tasklink). |
### add(Task pred, Task succ) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-}
```
public final TaskLink add(Task pred, Task succ)
```


Restituisce un'istanza di Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) che è stata aggiunta all'oggetto TaskLinkCollection.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Attività predecessore. |
| succ | [Task](../../com.aspose.tasks/task) | Attività successore. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-}
```
public final TaskLink add(Task pred, Task succ, int linkType)
```


Restituisce un'istanza di [TaskLink](../../com.aspose.tasks/tasklink) che è stata aggiunta all'oggetto TaskLinkCollection.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Attività predecessore. |
| succ | [Task](../../com.aspose.tasks/task) | Attività successore. |
| linkType | int | Tipo di collegamento [TaskLinkType](../../com.aspose.tasks/tasklinktype) |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType, Duration lag) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-}
```
public final TaskLink add(Task pred, Task succ, int linkType, Duration lag)
```


Restituisce un'istanza di [TaskLink](../../com.aspose.tasks/tasklink) che è stata aggiunta all'oggetto TaskLinkCollection.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Attività predecessore. |
| succ | [Task](../../com.aspose.tasks/task) | Attività successore. |
| linkType | int | Tipo di collegamento [TaskLinkType](../../com.aspose.tasks/tasklinktype) |
| lag | [Duration](../../com.aspose.tasks/duration) | Ritardo del collegamento [Duration](../../com.aspose.tasks/duration). |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link which has been added to this object.
### add(TaskLink e) {#add-com.aspose.tasks.TaskLink-}
```
public final boolean add(TaskLink e)
```


Questa è l'implementazione stub del metodo Add di ICollection, che lancia solo UnsupportedOperationException

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| e | [TaskLink](../../com.aspose.tasks/tasklink) | L'elemento da aggiungere. |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


Riservato per uso interno.

### get(int index) {#get-int-}
```
public TaskLink get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - \{@inheritDoc\}
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Ottiene il progetto padre dell'oggetto ResourceAssignmentCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent `Project` for this object.
### remove(int index) {#remove-int-}
```
public final TaskLink remove(int index)
```


Rimuove l'elemento nella posizione specificata in questa raccolta e restituisce l'elemento che è stato rimosso dalla raccolta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | la posizione specificata per rimuovere l'elemento. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - the element that was removed from the collection.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Rimuove il collegamento di attività da un progetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elemento | java.lang.Object | l'istanza specificata della classe `TaskLink` da rimuovere. |

**Returns:**
boolean - restituisce l'istanza della classe `TaskLink` che è stata rimossa da questa collezione.
### size() {#size--}
```
public final int size()
```


Restituisce il numero di oggetti contenuti in questo oggetto `TaskLinkCollection`. Solo lettura `int`.

**Returns:**
int - restituisce il numero di oggetti contenuti in questa collezione.
### sort(Comparator&lt;? super TaskLink&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--}
```
public void sort(Comparator<? super TaskLink> c)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.TaskLink&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<TaskLink> toList()
```


Converte l'oggetto TaskLinkCollection in un elenco di oggetti [TaskLink](../../com.aspose.tasks/tasklink).

**Returns:**
java.util.List&lt;com.aspose.tasks.TaskLink&gt; - Elenco di oggetti [TaskLink](../../com.aspose.tasks/tasklink).
