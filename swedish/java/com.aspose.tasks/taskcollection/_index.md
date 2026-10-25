---
title: "TaskCollection"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en samling av  objekt."
type: docs
weight: 293
url: /sv/java/com.aspose.tasks/taskcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskCollection extends AbstractList<Task>
```

Representerar en samling av [Task](../../com.aspose.tasks/task) objekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add()](#add--) | Lägger till en ny uppgift i projektets uppgiftslista på samma rubriknivå som den sista uppgiften. |
| [add(RecurringTaskParameters parameters)](#add-com.aspose.tasks.RecurringTaskParameters-) | Infogar en ny uppgift före en uppgift med det angivna id:t och på samma rubriknivå. |
| [add(Task item)](#add-com.aspose.tasks.Task-) | Lägg till den angivna uppgiften till en instans av klassen [TaskCollection](../../com.aspose.tasks/taskcollection). |
| [add(String taskName)](#add-java.lang.String-) | Lägger till en ny uppgift i underuppgiftslistan. |
| [add(String taskName, int beforeTaskId)](#add-java.lang.String-int-) | Lägger till en ny återkommande uppgift i samlingen av underordnade uppgifter. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Task item)](#contains-com.aspose.tasks.Task-) | Kontrollerar om samlingen innehåller det angivna objektet. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | Returnerar en uppgift med det angivna Id som har som förfader den överordnade uppgiften för denna samling. |
| [getByUid(int uid)](#getByUid-int-) | Returnerar en uppgift med den angivna Uid som har som förfader den överordnade uppgiften för denna samling. |
| [getParentProject()](#getParentProject--) | Hämtar det överordnade projektet för TaskCollection-objektet. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Hämtar ett värde som indikerar om denna samling är skrivskyddad. |
| [iterator()](#iterator--) | Returnerar en enumerator för denna samling. |
| [remove(Object item)](#remove-java.lang.Object-) | Detta är stub-implementationen av ICollection:s Remove‑metod, som endast kastar UnsupportedOperationException. |
| [size()](#size--) | Hämtar antalet objekt som finns i TaskCollection. |
| [sort(Comparator&lt;? super Task&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.Task--) | \{@inheritDoc\} |
| [toList()](#toList--) | Konverterar TaskCollection‑objektet till en lista med [Task](../../com.aspose.tasks/task)-objekt. |
### add() {#add--}
```
public final Task add()
```


Lägger till en ny uppgift i projektets uppgiftslista på samma rubriknivå som den sista uppgiften.

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(RecurringTaskParameters parameters) {#add-com.aspose.tasks.RecurringTaskParameters-}
```
public final Task add(RecurringTaskParameters parameters)
```


Infogar en ny uppgift före en uppgift med det angivna id:t och på samma rubriknivå.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| parameters | [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) | Parametrarna för skapandet av en återkommande uppgift. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(Task item) {#add-com.aspose.tasks.Task-}
```
public final boolean add(Task item)
```


Lägg till den angivna uppgiften i en instans av klassen [TaskCollection](../../com.aspose.tasks/taskcollection). Om ParentProject.CalculationMode är None bör användaren anropa Project.Recalculate() efter att ha använt denna metod (Den kommer att omplanera alla projektuppgifter (start-/slutdatum, sätter tidiga/sena datum) och beräkna de beroende fälten såsom slack, arbete och kostnadsfält, id:n och outline‑nivåer). Om ParentProject.CalculationMode är Manual kommer metoden endast att beräkna uppgifts‑id, outline‑nivå och outline‑nummer automatiskt. Om ParentProject.CalculationMode är Automatic omplaneras alla projektets uppgifter automatiskt (start-/slutdatum, sätter tidiga/sena datum, beräknar slack, arbete och kostnadsfält, omberäknar id:n och outline‑nivåer).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | den angivna uppgiften som ska läggas till i denna uppgiftskollektion. |

**Returns:**
boolean - true om operationen lyckades.
### add(String taskName) {#add-java.lang.String-}
```
public final Task add(String taskName)
```


Lägger till en ny uppgift i underuppgiftslistan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| taskName | java.lang.String | det angivna uppgiftsnamnet. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(String taskName, int beforeTaskId) {#add-java.lang.String-int-}
```
public final Task add(String taskName, int beforeTaskId)
```


Lägger till en ny återkommande uppgift i samlingen av underordnade uppgifter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| taskName | java.lang.String | det angivna uppgiftsnamnet. |
| beforeTaskId | int | Det angivna id‑t för en uppgift före vilken en ny uppgift kommer att infogas. |

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


Kontrollerar om samlingen innehåller det angivna objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | Objektet att kontrollera. |

**Returns:**
boolean - true, om samlingen innehåller ett objekt, annars false.
### get(int index) {#get-int-}
```
public Task get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Task](../../com.aspose.tasks/task) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Task getById(int id)
```


Returnerar en uppgift med det angivna Id som har som förfader den överordnade uppgiften för denna samling.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| id | int | TaskEntity Id |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified id whose ancestor is parent task of this collection.
### getByUid(int uid) {#getByUid-int-}
```
public final Task getByUid(int uid)
```


Returnerar en uppgift med den angivna Uid som har som förfader den överordnade uppgiften för denna samling.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | int | TaskEntity Uid. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified uid whose ancestor is parent task of this collection.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Hämtar det överordnade projektet för TaskCollection-objektet.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the TaskCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int – \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Hämtar ett värde som indikerar om denna samling är skrivskyddad.

**Returns:**
boolean - ett värde som indikerar om denna samling är skrivskyddad.
### iterator() {#iterator--}
```
public final Iterator<Task> iterator()
```


Returnerar en enumerator för denna samling.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Task&gt; - en enumerator för denna samling.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Detta är stub-implementationen av ICollection:s Remove‑metod, som endast kastar UnsupportedOperationException.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objekt | java.lang.Object | Objektet som ska tas bort. |

**Returns:**
boolean - `true` om objektet togs bort; `false` annars.
### size() {#size--}
```
public final int size()
```


Hämtar antalet objekt som finns i TaskCollection.

**Returns:**
int - antalet objekt som finns i TaskCollection.
### sort(Comparator&lt;? super Task&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.Task--}
```
public final void sort(Comparator<? super Task> c)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.Task&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Task> toList()
```


Konverterar TaskCollection‑objektet till en lista med [Task](../../com.aspose.tasks/task)-objekt.

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - returnerar en lista som innehåller [Task](../../com.aspose.tasks/task)-klassinstanser för denna samling.
