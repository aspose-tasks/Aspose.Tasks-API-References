---
title: "TaskCollection"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een collectie van objecten voor."
type: docs
weight: 293
url: /nl/java/com.aspose.tasks/taskcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskCollection extends AbstractList<Task>
```

Stelt een verzameling van [Task](../../com.aspose.tasks/task) objecten voor.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [add()](#add--) | Voegt een nieuwe taak toe aan de projecttaken‑collectie op hetzelfde outline‑niveau als de laatste taak. |
| [add(RecurringTaskParameters parameters)](#add-com.aspose.tasks.RecurringTaskParameters-) | Voegt een nieuwe taak in vóór een taak met de opgegeven id en op hetzelfde outline‑niveau. |
| [add(Task item)](#add-com.aspose.tasks.Task-) | Voeg de opgegeven taak toe aan de instantie van de [TaskCollection](../../com.aspose.tasks/taskcollection) klasse. |
| [add(String taskName)](#add-java.lang.String-) | Voegt een nieuwe taak toe aan de collectie van onderliggende taken. |
| [add(String taskName, int beforeTaskId)](#add-java.lang.String-int-) | Voegt een nieuwe terugkerende taak toe aan de collectie van onderliggende taken. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Task item)](#contains-com.aspose.tasks.Task-) | Controleert of de collectie het opgegeven item bevat. |
| [get(int index)](#get-int-) | (@inheritDoc\\} |
| [getById(int id)](#getById-int-) | Retourneert een taak met de opgegeven Id waarvan de voorouder de bovenliggende taak van deze collectie is. |
| [getByUid(int uid)](#getByUid-int-) | Retourneert een taak met de opgegeven Uid waarvan de voorouder de bovenliggende taak van deze collectie is. |
| [getParentProject()](#getParentProject--) | Haalt het bovenliggende project op van het TaskCollection‑object. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Haalt een waarde op die aangeeft of deze collectie alleen-lezen is. |
| [iterator()](#iterator--) | Retourneert een enumerator voor deze collectie. |
| [remove(Object item)](#remove-java.lang.Object-) | Dit is de stub‑implementatie van de Remove‑methode van ICollection, die alleen UnsupportedOperationException gooit. |
| [size()](#size--) | Haalt het aantal objecten op dat in de TaskCollection zit. |
| [sort(Comparator&lt;? super Task&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.Task--) | \{@inheritDoc\} |
| [toList()](#toList--) | Converteert het TaskCollection‑object naar een lijst van [Task](../../com.aspose.tasks/task) objecten. |
### add() {#add--}
```
public final Task add()
```


Voegt een nieuwe taak toe aan de projecttaken‑collectie op hetzelfde outline‑niveau als de laatste taak.

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(RecurringTaskParameters parameters) {#add-com.aspose.tasks.RecurringTaskParameters-}
```
public final Task add(RecurringTaskParameters parameters)
```


Voegt een nieuwe taak in vóór een taak met de opgegeven id en op hetzelfde outline‑niveau.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| parameters | [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) | De opgegeven parameters voor het aanmaken van een terugkerende taak. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(Task item) {#add-com.aspose.tasks.Task-}
```
public final boolean add(Task item)
```


Voeg de opgegeven taak toe aan de instantie van de [TaskCollection](../../com.aspose.tasks/taskcollection) klasse. Als ParentProject.CalculationMode None is, moet de gebruiker Project.Recalculate() aanroepen na het gebruiken van deze methode (Dit zal alle projecttaken opnieuw plannen (start-/einddatums, stelt vroege/late datums in) en de afhankelijke velden berekenen, zoals speling, werk- en kostengegevens, id's en outline-niveaus). Als ParentProject.CalculationMode Manual is, berekent de methode alleen taak-id, outline-niveau en outline-nummers automatisch. Als ParentProject.CalculationMode Automatic is, plant de methode alle taken van het project automatisch opnieuw (start-/einddatums, stelt vroege/late datums in, berekent speling, werk- en kostengegevens, herberekent id's en outline-niveaus).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | de opgegeven taak die aan deze taakverzameling moet worden toegevoegd. |

**Returns:**
boolean - true als de bewerking succesvol was.
### add(String taskName) {#add-java.lang.String-}
```
public final Task add(String taskName)
```


Voegt een nieuwe taak toe aan de collectie van onderliggende taken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| taskName | java.lang.String | de opgegeven taaknaam. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(String taskName, int beforeTaskId) {#add-java.lang.String-int-}
```
public final Task add(String taskName, int beforeTaskId)
```


Voegt een nieuwe terugkerende taak toe aan de collectie van onderliggende taken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| taskName | java.lang.String | de opgegeven taaknaam. |
| beforeTaskId | int | De opgegeven id van een taak vóór welke een nieuwe taak wordt ingevoegd. |

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


Controleert of de collectie het opgegeven item bevat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | Het te controleren item. |

**Returns:**
boolean - true, als de collectie een item bevat, anders false.
### get(int index) {#get-int-}
```
public Task get(int index)
```


(@inheritDoc\\}

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Task](../../com.aspose.tasks/task) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Task getById(int id)
```


Retourneert een taak met de opgegeven Id waarvan de voorouder de bovenliggende taak van deze collectie is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| id | int | TaskEntity Id |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified id whose ancestor is parent task of this collection.
### getByUid(int uid) {#getByUid-int-}
```
public final Task getByUid(int uid)
```


Retourneert een taak met de opgegeven Uid waarvan de voorouder de bovenliggende taak van deze collectie is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| uid | int | TaskEntity Uid. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified uid whose ancestor is parent task of this collection.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Haalt het bovenliggende project op van het TaskCollection‑object.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the TaskCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Haalt een waarde op die aangeeft of deze collectie alleen-lezen is.

**Returns:**
boolean - een waarde die aangeeft of deze collectie alleen-lezen is.
### iterator() {#iterator--}
```
public final Iterator<Task> iterator()
```


Retourneert een enumerator voor deze collectie.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Task&gt; - een enumerator voor deze collectie.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Dit is de stub‑implementatie van de Remove‑methode van ICollection, die alleen UnsupportedOperationException gooit.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | java.lang.Object | Het item om te verwijderen. |

**Returns:**
boolean - `true` als het item is verwijderd; `false` anders.
### size() {#size--}
```
public final int size()
```


Haalt het aantal objecten op dat in de TaskCollection zit.

**Returns:**
int - het aantal objecten dat in de TaskCollection zit.
### sort(Comparator&lt;? super Task&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.Task--}
```
public final void sort(Comparator<? super Task> c)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.Task&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Task> toList()
```


Converteert het TaskCollection‑object naar een lijst van [Task](../../com.aspose.tasks/task) objecten.

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - retourneert een lijst die de [Task](../../com.aspose.tasks/task) klasse‑instanties van deze collectie bevat.
