---
title: "TaskLinkCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Sammlung von Objekten dar."
type: docs
weight: 296
url: /de/java/com.aspose.tasks/tasklinkcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskLinkCollection extends AbstractList<TaskLink>
```

Stellt eine Sammlung von [Task](../../com.aspose.tasks/task)-Objekten dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(Task pred, Task succ)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-) | Gibt eine Instanz von Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) zurück, die dem TaskLinkCollection-Objekt hinzugefügt wurde. |
| [add(Task pred, Task succ, int linkType)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-) | Gibt eine Instanz von [TaskLink](../../com.aspose.tasks/tasklink) zurück, die dem TaskLinkCollection-Objekt hinzugefügt wurde. |
| [add(Task pred, Task succ, int linkType, Duration lag)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-) | Gibt eine Instanz von [TaskLink](../../com.aspose.tasks/tasklink) zurück, die dem TaskLinkCollection-Objekt hinzugefügt wurde. |
| [add(TaskLink e)](#add-com.aspose.tasks.TaskLink-) | Dies ist die Stub‑Implementierung der Add‑Methode von ICollection, die nur UnsupportedOperationException wirft. |
| [clear()](#clear--) | Für den internen Gebrauch reserviert. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getParentProject()](#getParentProject--) | Ermittelt das übergeordnete Projekt des ResourceAssignmentCollection-Objekts. |
| [remove(int index)](#remove-int-) | Entfernt das Element an der angegebenen Position in dieser Sammlung und gibt das entfernte Element zurück. |
| [remove(Object item)](#remove-java.lang.Object-) | Entfernt die Aufgabenverknüpfung aus einem Projekt. |
| [size()](#size--) | Gibt die Anzahl der in diesem `TaskLinkCollection`-Objekt enthaltenen Objekte zurück. |
| [sort(Comparator&lt;? super TaskLink&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--) | \{@inheritDoc\} |
| [toList()](#toList--) | Konvertiert das TaskLinkCollection-Objekt in eine Liste von [TaskLink](../../com.aspose.tasks/tasklink)-Objekten. |
### add(Task pred, Task succ) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-}
```
public final TaskLink add(Task pred, Task succ)
```


Gibt eine Instanz von Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) zurück, die dem TaskLinkCollection-Objekt hinzugefügt wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Vorgängeraufgabe. |
| succ | [Task](../../com.aspose.tasks/task) | Nachfolgeraufgabe. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-}
```
public final TaskLink add(Task pred, Task succ, int linkType)
```


Gibt eine Instanz von [TaskLink](../../com.aspose.tasks/tasklink) zurück, die dem TaskLinkCollection-Objekt hinzugefügt wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Vorgängeraufgabe. |
| succ | [Task](../../com.aspose.tasks/task) | Nachfolgeraufgabe. |
| linkType | int | Verknüpfungstyp [TaskLinkType](../../com.aspose.tasks/tasklinktype) |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType, Duration lag) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-}
```
public final TaskLink add(Task pred, Task succ, int linkType, Duration lag)
```


Gibt eine Instanz von [TaskLink](../../com.aspose.tasks/tasklink) zurück, die dem TaskLinkCollection-Objekt hinzugefügt wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Vorgängeraufgabe. |
| succ | [Task](../../com.aspose.tasks/task) | Nachfolgeraufgabe. |
| linkType | int | Verknüpfungstyp [TaskLinkType](../../com.aspose.tasks/tasklinktype) |
| lag | [Duration](../../com.aspose.tasks/duration) | Verknüpfungsverzögerung [Duration](../../com.aspose.tasks/duration). |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link which has been added to this object.
### add(TaskLink e) {#add-com.aspose.tasks.TaskLink-}
```
public final boolean add(TaskLink e)
```


Dies ist die Stub‑Implementierung der Add‑Methode von ICollection, die nur UnsupportedOperationException wirft.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| e | [TaskLink](../../com.aspose.tasks/tasklink) | Das hinzuzufügende Element. |

**Returns:**
boolean - \\{@inheritDoc\\}
### clear() {#clear--}
```
public final void clear()
```


Für den internen Gebrauch reserviert.

### get(int index) {#get-int-}
```
public TaskLink get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | \{@inheritDoc\} |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - \{@inheritDoc\}
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Ermittelt das übergeordnete Projekt des ResourceAssignmentCollection-Objekts.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent `Project` for this object.
### remove(int index) {#remove-int-}
```
public final TaskLink remove(int index)
```


Entfernt das Element an der angegebenen Position in dieser Sammlung und gibt das entfernte Element zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | die angegebene Position, an der das Element entfernt werden soll. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - the element that was removed from the collection.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Entfernt die Aufgabenverknüpfung aus einem Projekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Element | java.lang.Object | die angegebene Instanz der `TaskLink`-Klasse zum Entfernen. |

**Returns:**
boolescher Wert – gibt die Instanz der `TaskLink`-Klasse zurück, die aus dieser Sammlung entfernt wurde.
### size() {#size--}
```
public final int size()
```


Gibt die Anzahl der in diesem `TaskLinkCollection`-Objekt enthaltenen Objekte zurück. Nur lesbarer `int`.

**Returns:**
int - gibt die Anzahl der in dieser Sammlung enthaltenen Objekte zurück.
### sort(Comparator&lt;? super TaskLink&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--}
```
public void sort(Comparator<? super TaskLink> c)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.TaskLink&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<TaskLink> toList()
```


Konvertiert das TaskLinkCollection-Objekt in eine Liste von [TaskLink](../../com.aspose.tasks/tasklink)-Objekten.

**Returns:**
java.util.List&lt;com.aspose.tasks.TaskLink&gt; - Liste von [TaskLink](../../com.aspose.tasks/tasklink)-Objekten.
