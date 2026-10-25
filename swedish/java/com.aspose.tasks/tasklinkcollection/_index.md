---
title: "TaskLinkCollection"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en samling av  objekt."
type: docs
weight: 296
url: /sv/java/com.aspose.tasks/tasklinkcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskLinkCollection extends AbstractList<TaskLink>
```

Representerar en samling av [Task](../../com.aspose.tasks/task) objekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(Task pred, Task succ)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-) | Returnerar en instans av Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) som har lagts till i TaskLinkCollection-objektet. |
| [add(Task pred, Task succ, int linkType)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-) | Returnerar en instans av [TaskLink](../../com.aspose.tasks/tasklink) som har lagts till i TaskLinkCollection-objektet. |
| [add(Task pred, Task succ, int linkType, Duration lag)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-) | Returnerar en instans av [TaskLink](../../com.aspose.tasks/tasklink) som har lagts till i TaskLinkCollection-objektet. |
| [add(TaskLink e)](#add-com.aspose.tasks.TaskLink-) | Detta är stub-implementationen av ICollection:s Add‑metod, som endast kastar UnsupportedOperationException. |
| [clear()](#clear--) | Reserverad för intern användning. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getParentProject()](#getParentProject--) | Hämtar föräldraprojektet för ResourceAssignmentCollection-objektet. |
| [remove(int index)](#remove-int-) | Tar bort elementet på den angivna positionen i denna samling och returnerar elementet som togs bort från samlingen. |
| [remove(Object item)](#remove-java.lang.Object-) | Tar bort uppgiftslänk från ett projekt. |
| [size()](#size--) | Returnerar antalet objekt som finns i detta `TaskLinkCollection`-objekt. |
| [sort(Comparator&lt;? super TaskLink&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--) | \{@inheritDoc\} |
| [toList()](#toList--) | Konverterar TaskLinkCollection-objektet till en lista av [TaskLink](../../com.aspose.tasks/tasklink) objekt. |
### add(Task pred, Task succ) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-}
```
public final TaskLink add(Task pred, Task succ)
```


Returnerar en instans av Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) som har lagts till i TaskLinkCollection-objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Föregående uppgift. |
| succ | [Task](../../com.aspose.tasks/task) | Efterföljande uppgift. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-}
```
public final TaskLink add(Task pred, Task succ, int linkType)
```


Returnerar en instans av [TaskLink](../../com.aspose.tasks/tasklink) som har lagts till i TaskLinkCollection-objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Föregående uppgift. |
| succ | [Task](../../com.aspose.tasks/task) | Efterföljande uppgift. |
| linkType | int | Länktyp [TaskLinkType](../../com.aspose.tasks/tasklinktype) |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType, Duration lag) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-}
```
public final TaskLink add(Task pred, Task succ, int linkType, Duration lag)
```


Returnerar en instans av [TaskLink](../../com.aspose.tasks/tasklink) som har lagts till i TaskLinkCollection-objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Föregående uppgift. |
| succ | [Task](../../com.aspose.tasks/task) | Efterföljande uppgift. |
| linkType | int | Länktyp [TaskLinkType](../../com.aspose.tasks/tasklinktype) |
| lag | [Duration](../../com.aspose.tasks/duration) | Länkfördröjning [Duration](../../com.aspose.tasks/duration). |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link which has been added to this object.
### add(TaskLink e) {#add-com.aspose.tasks.TaskLink-}
```
public final boolean add(TaskLink e)
```


Detta är stub-implementationen av ICollection:s Add‑metod, som endast kastar UnsupportedOperationException.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| e | [TaskLink](../../com.aspose.tasks/tasklink) | Objektet att lägga till. |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


Reserverad för intern användning.

### get(int index) {#get-int-}
```
public TaskLink get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - \{@inheritDoc\}
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Hämtar föräldraprojektet för ResourceAssignmentCollection-objektet.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent `Project` for this object.
### remove(int index) {#remove-int-}
```
public final TaskLink remove(int index)
```


Tar bort elementet på den angivna positionen i denna samling och returnerar elementet som togs bort från samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | den angivna positionen för att ta bort elementet vid. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - the element that was removed from the collection.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Tar bort uppgiftslänk från ett projekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objekt | java.lang.Object | den angivna instansen av `TaskLink`-klassen att ta bort. |

**Returns:**
boolean - returnerar instansen av `TaskLink`-klassen som togs bort från denna samling.
### size() {#size--}
```
public final int size()
```


Returnerar antalet objekt som finns i detta `TaskLinkCollection`-objekt. Endast läs `int`.

**Returns:**
int - returnerar antalet objekt som finns i denna samling.
### sort(Comparator&lt;? super TaskLink&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--}
```
public void sort(Comparator<? super TaskLink> c)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.TaskLink&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<TaskLink> toList()
```


Konverterar TaskLinkCollection-objektet till en lista av [TaskLink](../../com.aspose.tasks/tasklink) objekt.

**Returns:**
java.util.List&lt;com.aspose.tasks.TaskLink&gt; - Lista över [TaskLink](../../com.aspose.tasks/tasklink) objekt.
