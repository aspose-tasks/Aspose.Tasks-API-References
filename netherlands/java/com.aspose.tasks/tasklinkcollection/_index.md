---
title: "TaskLinkCollection"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een collectie van objecten voor."
type: docs
weight: 296
url: /nl/java/com.aspose.tasks/tasklinkcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskLinkCollection extends AbstractList<TaskLink>
```

Stelt een verzameling van [Task](../../com.aspose.tasks/task) objecten voor.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [add(Task pred, Task succ)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-) | Retourneert een instantie van Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) die is toegevoegd aan het TaskLinkCollection-object. |
| [add(Task pred, Task succ, int linkType)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-) | Retourneert een instantie van [TaskLink](../../com.aspose.tasks/tasklink) die is toegevoegd aan het TaskLinkCollection-object. |
| [add(Task pred, Task succ, int linkType, Duration lag)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-) | Retourneert een instantie van [TaskLink](../../com.aspose.tasks/tasklink) die is toegevoegd aan het TaskLinkCollection-object. |
| [add(TaskLink e)](#add-com.aspose.tasks.TaskLink-) | Dit is de stub‑implementatie van de Add‑methode van ICollection, die alleen UnsupportedOperationException gooit. |
| [clear()](#clear--) | Gereserveerd voor intern gebruik. |
| [get(int index)](#get-int-) | (@inheritDoc\\} |
| [getParentProject()](#getParentProject--) | Haalt het bovenliggende project op van het ResourceAssignmentCollection-object. |
| [remove(int index)](#remove-int-) | Verwijdert het element op de opgegeven positie in deze collectie en retourneert het element dat uit de collectie is verwijderd. |
| [remove(Object item)](#remove-java.lang.Object-) | Verwijdert een taakkoppeling uit een project. |
| [size()](#size--) | Retourneert het aantal objecten dat zich in dit `TaskLinkCollection`-object bevindt. |
| [sort(Comparator&lt;? super TaskLink&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--) | \{@inheritDoc\} |
| [toList()](#toList--) | Converteert het TaskLinkCollection-object naar een lijst van [TaskLink](../../com.aspose.tasks/tasklink) objecten. |
### add(Task pred, Task succ) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-}
```
public final TaskLink add(Task pred, Task succ)
```


Retourneert een instantie van Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) die is toegevoegd aan het TaskLinkCollection-object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Voorgaande taak. |
| succ | [Task](../../com.aspose.tasks/task) | Volgende taak. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-}
```
public final TaskLink add(Task pred, Task succ, int linkType)
```


Retourneert een instantie van [TaskLink](../../com.aspose.tasks/tasklink) die is toegevoegd aan het TaskLinkCollection-object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Voorgaande taak. |
| succ | [Task](../../com.aspose.tasks/task) | Volgende taak. |
| linkType | int | Koppelingstype [TaskLinkType](../../com.aspose.tasks/tasklinktype) |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType, Duration lag) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-}
```
public final TaskLink add(Task pred, Task succ, int linkType, Duration lag)
```


Retourneert een instantie van [TaskLink](../../com.aspose.tasks/tasklink) die is toegevoegd aan het TaskLinkCollection-object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Voorgaande taak. |
| succ | [Task](../../com.aspose.tasks/task) | Volgende taak. |
| linkType | int | Koppelingstype [TaskLinkType](../../com.aspose.tasks/tasklinktype) |
| lag | [Duration](../../com.aspose.tasks/duration) | Koppelingvertraging [Duration](../../com.aspose.tasks/duration). |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link which has been added to this object.
### add(TaskLink e) {#add-com.aspose.tasks.TaskLink-}
```
public final boolean add(TaskLink e)
```


Dit is de stub‑implementatie van de Add‑methode van ICollection, die alleen UnsupportedOperationException gooit.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| e | [TaskLink](../../com.aspose.tasks/tasklink) | Het toe te voegen item. |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


Gereserveerd voor intern gebruik.

### get(int index) {#get-int-}
```
public TaskLink get(int index)
```


(@inheritDoc\\}

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - \{@inheritDoc\}
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Haalt het bovenliggende project op van het ResourceAssignmentCollection-object.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent `Project` for this object.
### remove(int index) {#remove-int-}
```
public final TaskLink remove(int index)
```


Verwijdert het element op de opgegeven positie in deze collectie en retourneert het element dat uit de collectie is verwijderd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | de opgegeven positie om het element te verwijderen. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - the element that was removed from the collection.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Verwijdert een taakkoppeling uit een project.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | java.lang.Object | de opgegeven instantie van de `TaskLink`-klasse om te verwijderen. |

**Returns:**
boolean - retourneert de instantie van de `TaskLink`-klasse die uit deze collectie is verwijderd.
### size() {#size--}
```
public final int size()
```


Retourneert het aantal objecten dat zich in dit `TaskLinkCollection`-object bevindt. Alleen-lezen `int`.

**Returns:**
int - retourneert het aantal objecten dat zich in deze collectie bevindt.
### sort(Comparator&lt;? super TaskLink&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--}
```
public void sort(Comparator<? super TaskLink> c)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.TaskLink&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<TaskLink> toList()
```


Converteert het TaskLinkCollection-object naar een lijst van [TaskLink](../../com.aspose.tasks/tasklink) objecten.

**Returns:**
java.util.List&lt;com.aspose.tasks.TaskLink&gt; - Lijst van [TaskLink](../../com.aspose.tasks/tasklink) objecten.
