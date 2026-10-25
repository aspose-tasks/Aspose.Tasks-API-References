---
title: "TaskCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Sammlung von Objekten dar."
type: docs
weight: 293
url: /de/java/com.aspose.tasks/taskcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskCollection extends AbstractList<Task>
```

Stellt eine Sammlung von [Task](../../com.aspose.tasks/task)-Objekten dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add()](#add--) | Fügt eine neue Aufgabe zur Aufgabensammlung des Projekts auf derselben Gliederungsebene wie die letzte Aufgabe hinzu. |
| [add(RecurringTaskParameters parameters)](#add-com.aspose.tasks.RecurringTaskParameters-) | Fügt eine neue Aufgabe vor einer Aufgabe mit der angegebenen ID und auf derselben Gliederungsebene ein. |
| [add(Task item)](#add-com.aspose.tasks.Task-) | Füge die angegebene Aufgabe zur Instanz der [TaskCollection](../../com.aspose.tasks/taskcollection)-Klasse hinzu. |
| [add(String taskName)](#add-java.lang.String-) | Fügt eine neue Aufgabe zur Sammlung der Unteraufgaben hinzu. |
| [add(String taskName, int beforeTaskId)](#add-java.lang.String-int-) | Fügt eine neue wiederkehrende Aufgabe zur Sammlung der Unteraufgaben hinzu. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Task item)](#contains-com.aspose.tasks.Task-) | Überprüft, ob die Sammlung das angegebene Element enthält. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | Gibt eine Aufgabe mit der angegebenen ID zurück, deren Vorgänger die übergeordnete Aufgabe dieser Sammlung ist. |
| [getByUid(int uid)](#getByUid-int-) | Gibt eine Aufgabe mit der angegebenen UID zurück, deren Vorgänger die übergeordnete Aufgabe dieser Sammlung ist. |
| [getParentProject()](#getParentProject--) | Ermittelt das übergeordnete Projekt des TaskCollection-Objekts. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Liefert einen Wert, der angibt, ob diese Sammlung schreibgeschützt ist. |
| [iterator()](#iterator--) | Gibt einen Enumerator für diese Sammlung zurück. |
| [remove(Object item)](#remove-java.lang.Object-) | Dies ist die Stub-Implementierung der Remove-Methode von ICollection, die nur eine UnsupportedOperationException wirft. |
| [size()](#size--) | Ermittelt die Anzahl der im TaskCollection enthaltenen Objekte. |
| [sort(Comparator&lt;? super Task&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.Task--) | \{@inheritDoc\} |
| [toList()](#toList--) | Konvertiert das TaskCollection-Objekt in eine Liste von [Task](../../com.aspose.tasks/task)-Objekten. |
### add() {#add--}
```
public final Task add()
```


Fügt eine neue Aufgabe zur Aufgabensammlung des Projekts auf derselben Gliederungsebene wie die letzte Aufgabe hinzu.

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(RecurringTaskParameters parameters) {#add-com.aspose.tasks.RecurringTaskParameters-}
```
public final Task add(RecurringTaskParameters parameters)
```


Fügt eine neue Aufgabe vor einer Aufgabe mit der angegebenen ID und auf derselben Gliederungsebene ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| parameters | [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) | Die angegebenen Parameter für die Erstellung einer wiederkehrenden Aufgabe. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(Task item) {#add-com.aspose.tasks.Task-}
```
public final boolean add(Task item)
```


Füge die angegebene Aufgabe zur Instanz der [TaskCollection](../../com.aspose.tasks/taskcollection)-Klasse hinzu. Wenn ParentProject.CalculationMode None ist, sollte der Benutzer nach Aufruf dieser Methode Project.Recalculate() ausführen (dies wird alle Projektaufgaben neu planen (Start-/Enddaten, legt Früh-/Spättermine fest) und die abhängigen Felder wie Puffer, Arbeits- und Kostenfelder, IDs und Gliederungsebenen berechnen). Wenn ParentProject.CalculationMode Manual ist, berechnet die Methode nur die Aufgaben-ID, die Gliederungsebene und die Gliederungsnummern automatisch. Wenn ParentProject.CalculationMode Automatic ist, plant die Methode alle Projektaufgaben automatisch neu (Start-/Enddaten, legt Früh-/Spättermine fest, berechnet Puffer, Arbeits- und Kostenfelder, recalculiert IDs und Gliederungsebenen).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | die angegebene Aufgabe, die zu dieser Aufgabensammlung hinzugefügt werden soll. |

**Returns:**
boolean - true, wenn die Operation erfolgreich war.
### add(String taskName) {#add-java.lang.String-}
```
public final Task add(String taskName)
```


Fügt eine neue Aufgabe zur Sammlung der Unteraufgaben hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| taskName | java.lang.String | der angegebene Aufgabenname. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(String taskName, int beforeTaskId) {#add-java.lang.String-int-}
```
public final Task add(String taskName, int beforeTaskId)
```


Fügt eine neue wiederkehrende Aufgabe zur Sammlung der Unteraufgaben hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| taskName | java.lang.String | der angegebene Aufgabenname. |
| beforeTaskId | int | Die angegebene ID einer Aufgabe, vor der eine neue Aufgabe eingefügt wird. |

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


Überprüft, ob die Sammlung das angegebene Element enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | Das zu prüfende Element. |

**Returns:**
boolean - true, wenn die Sammlung ein Element enthält, sonst false.
### get(int index) {#get-int-}
```
public Task get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | \{@inheritDoc\} |

**Returns:**
[Task](../../com.aspose.tasks/task) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Task getById(int id)
```


Gibt eine Aufgabe mit der angegebenen ID zurück, deren Vorgänger die übergeordnete Aufgabe dieser Sammlung ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ID | int | TaskEntity Id |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified id whose ancestor is parent task of this collection.
### getByUid(int uid) {#getByUid-int-}
```
public final Task getByUid(int uid)
```


Gibt eine Aufgabe mit der angegebenen UID zurück, deren Vorgänger die übergeordnete Aufgabe dieser Sammlung ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | int | TaskEntity Uid. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified uid whose ancestor is parent task of this collection.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Ermittelt das übergeordnete Projekt des TaskCollection-Objekts.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the TaskCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Liefert einen Wert, der angibt, ob diese Sammlung schreibgeschützt ist.

**Returns:**
boolean - ein Wert, der angibt, ob diese Sammlung schreibgeschützt ist.
### iterator() {#iterator--}
```
public final Iterator<Task> iterator()
```


Gibt einen Enumerator für diese Sammlung zurück.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Task&gt; - ein Enumerator für diese Sammlung.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Dies ist die Stub-Implementierung der Remove-Methode von ICollection, die nur eine UnsupportedOperationException wirft.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Element | java.lang.Object | Das zu entfernende Element. |

**Returns:**
boolean - `true`, wenn das Element entfernt wurde; `false` andernfalls.
### size() {#size--}
```
public final int size()
```


Ermittelt die Anzahl der im TaskCollection enthaltenen Objekte.

**Returns:**
int - die Anzahl der Objekte, die in der TaskCollection enthalten sind.
### sort(Comparator&lt;? super Task&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.Task--}
```
public final void sort(Comparator<? super Task> c)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| c | java.util.Comparator<? super com.aspose.tasks.Task> | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Task> toList()
```


Konvertiert das TaskCollection-Objekt in eine Liste von [Task](../../com.aspose.tasks/task)-Objekten.

**Returns:**
java.util.List<com.aspose.tasks.Task> - gibt eine Liste zurück, die die [Task](../../com.aspose.tasks/task)-Klasseninstanzen dieser Sammlung enthält.
