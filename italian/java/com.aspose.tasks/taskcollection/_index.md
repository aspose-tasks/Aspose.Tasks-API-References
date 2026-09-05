---
title: "TaskCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una raccolta di oggetti."
type: docs
weight: 293
url: /it/java/com.aspose.tasks/taskcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskCollection extends AbstractList<Task>
```

Rappresenta una raccolta di oggetti [Task](../../com.aspose.tasks/task).
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add()](#add--) | Aggiunge un nuovo task alla raccolta di task del progetto allo stesso livello di outline dell'ultimo task. |
| [add(RecurringTaskParameters parameters)](#add-com.aspose.tasks.RecurringTaskParameters-) | Inserisce un nuovo task prima di un task con l'ID specificato e allo stesso livello di outline. |
| [add(Task item)](#add-com.aspose.tasks.Task-) | Aggiunge il task specificato all'istanza della classe [TaskCollection](../../com.aspose.tasks/taskcollection). |
| [add(String taskName)](#add-java.lang.String-) | Aggiunge un nuovo task alla raccolta di task figli. |
| [add(String taskName, int beforeTaskId)](#add-java.lang.String-int-) | Aggiunge un nuovo task ricorrente alla raccolta di task figli. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Task item)](#contains-com.aspose.tasks.Task-) | Verifica se la collezione contiene l'elemento specificato. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | Restituisce un task con l'Id specificato il cui antenato è il task genitore di questa raccolta. |
| [getByUid(int uid)](#getByUid-int-) | Restituisce un task con l'Uid specificato il cui antenato è il task genitore di questa raccolta. |
| [getParentProject()](#getParentProject--) | Ottiene il progetto genitore dell'oggetto TaskCollection. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Ottiene un valore che indica se questa collezione è di sola lettura. |
| [iterator()](#iterator--) | Restituisce un enumeratore per questa collezione. |
| [remove(Object item)](#remove-java.lang.Object-) | Questa è l'implementazione stub del metodo Remove di ICollection, che lancia solo UnsupportedOperationException. |
| [size()](#size--) | Ottiene il numero di oggetti contenuti nella TaskCollection. |
| [sort(Comparator&lt;? super Task&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.Task--) | \{@inheritDoc\} |
| [toList()](#toList--) | Converte l'oggetto TaskCollection in un elenco di oggetti [Task](../../com.aspose.tasks/task). |
### add() {#add--}
```
public final Task add()
```


Aggiunge un nuovo task alla raccolta di task del progetto allo stesso livello di outline dell'ultimo task.

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(RecurringTaskParameters parameters) {#add-com.aspose.tasks.RecurringTaskParameters-}
```
public final Task add(RecurringTaskParameters parameters)
```


Inserisce un nuovo task prima di un task con l'ID specificato e allo stesso livello di outline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| parameters | [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) | I parametri specificati per la creazione di un task ricorrente. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(Task item) {#add-com.aspose.tasks.Task-}
```
public final boolean add(Task item)
```


Aggiungi l'attività specificata all'istanza della classe [TaskCollection](../../com.aspose.tasks/taskcollection). Se ParentProject.CalculationMode è None l'utente dovrebbe invocare Project.Recalculate() dopo aver usato questo metodo (Riprogrammerà tutte le attività del progetto (date di inizio/fine, imposta le date anticipate/posticipate) e calcolerà i campi dipendenti come slacks, campi di lavoro e costo, ID e livelli di outline). Se ParentProject.CalculationMode è Manual il metodo calcolerà solo l'ID dell'attività, il livello di outline e i numeri di outline automaticamente. Se ParentProject.CalculationMode è Automatic il metodo riprogramma automaticamente tutte le attività del progetto (date di inizio/fine, imposta le date anticipate/posticipate, calcola slacks, campi di lavoro e costo, ricalcola ID e livelli di outline).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | l'attività specificata che dovrebbe essere aggiunta a questa collezione di attività. |

**Returns:**
boolean - true se l'operazione è riuscita.
### add(String taskName) {#add-java.lang.String-}
```
public final Task add(String taskName)
```


Aggiunge un nuovo task alla raccolta di task figli.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| taskName | java.lang.String | il nome dell'attività specificata. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(String taskName, int beforeTaskId) {#add-java.lang.String-int-}
```
public final Task add(String taskName, int beforeTaskId)
```


Aggiunge un nuovo task ricorrente alla raccolta di task figli.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| taskName | java.lang.String | il nome dell'attività specificata. |
| beforeTaskId | int | L'ID specificato di un'attività prima della quale verrà inserita una nuova attività. |

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


Verifica se la collezione contiene l'elemento specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | L'elemento da verificare. |

**Returns:**
boolean - true, se la collezione contiene un elemento, false altrimenti.
### get(int index) {#get-int-}
```
public Task get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Task](../../com.aspose.tasks/task) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Task getById(int id)
```


Restituisce un task con l'Id specificato il cui antenato è il task genitore di questa raccolta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| id | int | TaskEntity Id |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified id whose ancestor is parent task of this collection.
### getByUid(int uid) {#getByUid-int-}
```
public final Task getByUid(int uid)
```


Restituisce un task con l'Uid specificato il cui antenato è il task genitore di questa raccolta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | int | TaskEntity Uid. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified uid whose ancestor is parent task of this collection.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Ottiene il progetto genitore dell'oggetto TaskCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the TaskCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Ottiene un valore che indica se questa collezione è di sola lettura.

**Returns:**
boolean - un valore che indica se questa collezione è di sola lettura.
### iterator() {#iterator--}
```
public final Iterator<Task> iterator()
```


Restituisce un enumeratore per questa collezione.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Task&gt; - un enumeratore per questa collezione.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Questa è l'implementazione stub del metodo Remove di ICollection, che lancia solo UnsupportedOperationException.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elemento | java.lang.Object | L'elemento da rimuovere. |

**Returns:**
boolean - `true` se l'elemento è stato rimosso; `false` altrimenti.
### size() {#size--}
```
public final int size()
```


Ottiene il numero di oggetti contenuti nella TaskCollection.

**Returns:**
int - il numero di oggetti contenuti nella TaskCollection.
### sort(Comparator&lt;? super Task&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.Task--}
```
public final void sort(Comparator<? super Task> c)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.Task&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Task> toList()
```


Converte l'oggetto TaskCollection in un elenco di oggetti [Task](../../com.aspose.tasks/task).

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - restituisce un elenco che contiene le istanze della classe [Task](../../com.aspose.tasks/task) di questa collezione.
