---
title: "TaskBaseline"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt die Basislinie einer Aufgabe dar."
type: docs
weight: 291
url: /de/java/com.aspose.tasks/taskbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)

**All Implemented Interfaces:**
java.lang.Comparable
```
public class TaskBaseline extends Baseline implements Comparable<Baseline>
```

Stellt die Basislinie einer Aufgabe dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [TaskBaseline(Task task)](#TaskBaseline-com.aspose.tasks.Task-) | Initialisiert eine neue Instanz der [TaskBaseline](../../com.aspose.tasks/taskbaseline)-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [compareTo(TaskBaseline other)](#compareTo-com.aspose.tasks.TaskBaseline-) | Implementierung des IComparable-Interfaces. |
| [equals(TaskBaseline other)](#equals-com.aspose.tasks.TaskBaseline-) | Gibt einen Wert zurück, der angibt, ob diese Instanz dem angegebenen TaskBaseline-Objekt gleich ist. |
| [equals(Object obj)](#equals-java.lang.Object-) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [getDuration()](#getDuration--) | Liefert die geplante Dauer der Aufgabe, als die Basislinie gespeichert wurde. |
| [getEstimatedDuration()](#getEstimatedDuration--) | Liefert einen Wert, der angibt, ob die Basisliniendauer der Aufgabe geschätzt wurde. |
| [getFinish()](#getFinish--) | Liefert das geplante Enddatum der Aufgabe, als die Basislinie gespeichert wurde. |
| [getFixedCost()](#getFixedCost--) | Liefert die feste Kosten der Aufgabe, als die Basislinie gespeichert wurde. |
| [getInterim()](#getInterim--) | Liefert einen Wert, der angibt, ob dies eine Zwischenbasislinie ist. |
| [getStart()](#getStart--) | Liefert das geplante Startdatum der Aufgabe, als die Basislinie gespeichert wurde. |
| [getTimephasedData()](#getTimephasedData--) | Liefert eine TimephasedDataCollection-Instanz für dieses Objekt. |
| [hashCode()](#hashCode--) | Gibt einen Hashcode-Wert für die Instanz der [TaskBaseline](../../com.aspose.tasks/taskbaseline)-Klasse zurück. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Setzt die geplante Dauer der Aufgabe, als die Basislinie gespeichert wurde. |
| [setEstimatedDuration(boolean value)](#setEstimatedDuration-boolean-) | Setzt einen Wert, der angibt, ob die Basisliniendauer der Aufgabe geschätzt wurde. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Setzt das geplante Enddatum der Aufgabe, als die Basislinie gespeichert wurde. |
| [setFixedCost(double value)](#setFixedCost-double-) | Setzt die feste Kosten der Aufgabe, als die Basislinie gespeichert wurde. |
| [setInterim(boolean value)](#setInterim-boolean-) | Setzt einen Wert, der angibt, ob dies eine Zwischenbasislinie ist. |
| [setStart(Date value)](#setStart-java.util.Date-) | Setzt das geplante Startdatum der Aufgabe, als die Basislinie gespeichert wurde. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Setzt eine TimephasedDataCollection-Instanz für dieses Objekt. |
### TaskBaseline(Task task) {#TaskBaseline-com.aspose.tasks.Task-}
```
public TaskBaseline(Task task)
```


Initialisiert eine neue Instanz der [TaskBaseline](../../com.aspose.tasks/taskbaseline)-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Elternaufgabe der Basislinie. |

### compareTo(TaskBaseline other) {#compareTo-com.aspose.tasks.TaskBaseline-}
```
public final int compareTo(TaskBaseline other)
```


Implementierung des IComparable-Interfaces. Vergleicht diese Instanz mit dem angegebenen Baseline-Objekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | das angegebene Baseline-Objekt, mit dem diese Instanz verglichen wird. |

**Returns:**
int - gibt -1 zurück, wenn diese Instanz kleiner als das angegebene Objekt ist, 1 wenn sie größer ist; andernfalls wird 0 zurückgegeben.
### equals(TaskBaseline other) {#equals-com.aspose.tasks.TaskBaseline-}
```
public final boolean equals(TaskBaseline other)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz dem angegebenen TaskBaseline-Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | das angegebene AssignmentBaseline-Objekt, das mit dieser Instanz verglichen wird. |

**Returns:**
boolean - gibt true zurück, wenn diese Instanz dem angegebenen TaskBaseline-Objekt gleich ist; andernfalls false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | Das Objekt, das mit dieser Instanz verglichen wird. |

**Returns:**
boolean - **True** wenn das angegebene Objekt ein TaskBaseline ist, das denselben UID-Wert wie diese Instanz hat; andernfalls **false**.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Liefert die geplante Dauer der Aufgabe, als die Basislinie gespeichert wurde.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the scheduled duration of the task when the baseline was saved.
### getEstimatedDuration() {#getEstimatedDuration--}
```
public final boolean getEstimatedDuration()
```


Liefert einen Wert, der angibt, ob die Basisliniendauer der Aufgabe geschätzt wurde.

**Returns:**
boolean - ein Wert, der angibt, ob die Basisliniendauer der Aufgabe geschätzt wurde.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Liefert das geplante Enddatum der Aufgabe, als die Basislinie gespeichert wurde.

**Returns:**
java.util.Date - das geplante Enddatum der Aufgabe, als die Basislinie gespeichert wurde.
### getFixedCost() {#getFixedCost--}
```
public final double getFixedCost()
```


Liefert die feste Kosten der Aufgabe, als die Basislinie gespeichert wurde.

**Returns:**
double - ein fester Kostenwert der Aufgabe, als die Basislinie gespeichert wurde.
### getInterim() {#getInterim--}
```
public final boolean getInterim()
```


Liefert einen Wert, der angibt, ob dies eine Zwischenbasislinie ist.

**Returns:**
boolean - ein Wert, der angibt, ob dies eine Zwischenbasislinie ist.
### getStart() {#getStart--}
```
public final Date getStart()
```


Liefert das geplante Startdatum der Aufgabe, als die Basislinie gespeichert wurde.

**Returns:**
java.util.Date - das geplante Startdatum der Aufgabe, als die Basislinie gespeichert wurde.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Ruft eine TimephasedDataCollection-Instanz für dieses Objekt ab. Die zeitlich gestaffelten Daten, die mit der Aufgabenbasislinie verknüpft sind.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - a TimephasedDataCollection instance for this object.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Gibt einen Hashcode-Wert für die Instanz der [TaskBaseline](../../com.aspose.tasks/taskbaseline)-Klasse zurück.

**Returns:**
int - gibt einen Hashcode-Wert für dieses Objekt zurück.
### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Setzt die geplante Dauer der Aufgabe, als die Basislinie gespeichert wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | die geplante Dauer der Aufgabe, als die Basislinie gespeichert wurde. |

### setEstimatedDuration(boolean value) {#setEstimatedDuration-boolean-}
```
public final void setEstimatedDuration(boolean value)
```


Setzt einen Wert, der angibt, ob die Basisliniendauer der Aufgabe geschätzt wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob die Basisliniendauer der Aufgabe geschätzt wurde. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Setzt das geplante Enddatum der Aufgabe, als die Basislinie gespeichert wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | das geplante Enddatum der Aufgabe, als die Basislinie gespeichert wurde. |

### setFixedCost(double value) {#setFixedCost-double-}
```
public final void setFixedCost(double value)
```


Setzt die feste Kosten der Aufgabe, als die Basislinie gespeichert wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | eine feste Kostenangabe der Aufgabe, als die Basislinie gespeichert wurde. |

### setInterim(boolean value) {#setInterim-boolean-}
```
public final void setInterim(boolean value)
```


Setzt einen Wert, der angibt, ob dies eine Zwischenbasislinie ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob dies eine Zwischenbasislinie ist. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Setzt das geplante Startdatum der Aufgabe, als die Basislinie gespeichert wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | das geplante Startdatum der Aufgabe, als die Basislinie gespeichert wurde. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Setzt eine TimephasedDataCollection-Instanz für dieses Objekt. Die zeitlich gestaffelten Daten, die mit der Aufgabenbasislinie verknüpft sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | eine TimephasedDataCollection-Instanz für dieses Objekt. |

