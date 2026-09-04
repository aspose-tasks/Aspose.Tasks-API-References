---
title: "TaskLink"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt einen Vorgängerlink dar."
type: docs
weight: 295
url: /de/java/com.aspose.tasks/tasklink/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public final class TaskLink implements System.IEquatable<TaskLink>
```

Stellt einen Vorgängerlink dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(TaskLink other)](#equals-com.aspose.tasks.TaskLink-) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [equals(Object obj)](#equals-java.lang.Object-) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [getCrossProjectName()](#getCrossProjectName--) | Ruft das externe Vorgängerprojekt ab. |
| [getLagFormat()](#getLagFormat--) | Ruft das Format zum Ausdruck des Verzugsformats ab. |
| [getLinkLag()](#getLinkLag--) | Ruft den Verzug in Zehntel einer Minute oder Prozent ab. |
| [getLinkLagTimeSpan()](#getLinkLagTimeSpan--) | Ruft die Verzugsdauer ab, abhängig vom LagFormat. |
| [getLinkType()](#getLinkType--) | Ruft den Typ eines Links ab. |
| [getPredTask()](#getPredTask--) | Ruft die Vorgängeraufgabe ab. |
| [getSuccTask()](#getSuccTask--) | Gibt die Nachfolgeraufgabe zurück. |
| [hashCode()](#hashCode--) | Gibt einen Hashcode-Wert für die Instanz der [TaskLink](../../com.aspose.tasks/tasklink)-Klasse zurück. |
| [isCrossProject()](#isCrossProject--) | Liefert einen Wert, der angibt, ob ein Vorgänger Teil eines anderen Projekts ist. |
| [setCrossProject(boolean value)](#setCrossProject-boolean-) | Setzt einen Wert, der angibt, ob ein Vorgänger Teil eines anderen Projekts ist. |
| [setCrossProjectName(String value)](#setCrossProjectName-java.lang.String-) | Setzt das externe Vorgängerprojekt. |
| [setLagFormat(byte value)](#setLagFormat-byte-) | Setzt das Format zur Angabe des Verzugs. |
| [setLinkLag(int value)](#setLinkLag-int-) | Setzt den Verzug in Zehntel einer Minute oder Prozent. |
| [setLinkLagTimeSpan(double value)](#setLinkLagTimeSpan-double-) | Setzt die Verzugsdauer, abhängig vom LagFormat. |
| [setLinkType(int value)](#setLinkType-int-) | Setzt den Typ einer Verknüpfung. |
| [setPredTask(Task value)](#setPredTask-com.aspose.tasks.Task-) | Setzt die Vorgängeraufgabe. |
| [setSuccTask(Task value)](#setSuccTask-com.aspose.tasks.Task-) | Setzt die Nachfolgeraufgabe. |
| [toString()](#toString--) | Gibt die Zeichenkettenrepräsentation eines TaskLink zurück. |
### equals(TaskLink other) {#equals-com.aspose.tasks.TaskLink-}
```
public final boolean equals(TaskLink other)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [TaskLink](../../com.aspose.tasks/tasklink) | Die angegebene Instanz der [TaskLink](../../com.aspose.tasks/tasklink)-Klasse zum Vergleich mit dieser Instanz. |

**Returns:**
boolean - **True**, wenn die angegebene Instanz der [TaskLink](../../com.aspose.tasks/tasklink)-Klasse dieselben Vorgänger- und Nachfolgeraufgaben wie diese Instanz hat; andernfalls **false**.
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
boolean - **True**, wenn das angegebene Objekt ein TaskLink ist, das dieselben Vorgänger- und Nachfolger wie diese Instanz hat; andernfalls **false**.
### getCrossProjectName() {#getCrossProjectName--}
```
public final String getCrossProjectName()
```


Ruft das externe Vorgängerprojekt ab.

**Returns:**
java.lang.String - das externe Vorgängerprojekt.
### getLagFormat() {#getLagFormat--}
```
public final byte getLagFormat()
```


Ruft das Format zum Ausdruck des Verzugsformats ab.

**Returns:**
byte - das Format zur Angabe des Verzugs.
### getLinkLag() {#getLinkLag--}
```
public final int getLinkLag()
```


Ruft den Verzug in Zehntel einer Minute oder Prozent ab.

**Returns:**
int - der Verzug in Zehntel einer Minute oder Prozent.
### getLinkLagTimeSpan() {#getLinkLagTimeSpan--}
```
public final double getLinkLagTimeSpan()
```


Ruft die Verzugsdauer ab, abhängig vom LagFormat.

**Returns:**
double - Verzugsdauer, abhängig vom LagFormat.
### getLinkType() {#getLinkType--}
```
public final int getLinkType()
```


Ruft den Typ eines Links ab.

**Returns:**
int - der Typ einer Verknüpfung.
### getPredTask() {#getPredTask--}
```
public final Task getPredTask()
```


Ruft die Vorgängeraufgabe ab.

**Returns:**
[Task](../../com.aspose.tasks/task) - the predecessor task.
### getSuccTask() {#getSuccTask--}
```
public final Task getSuccTask()
```


Gibt die Nachfolgeraufgabe zurück.

**Returns:**
[Task](../../com.aspose.tasks/task) - the successor task.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Gibt einen Hashcode-Wert für die Instanz der [TaskLink](../../com.aspose.tasks/tasklink)-Klasse zurück.

**Returns:**
int - gibt einen Hashcode-Wert für dieses Objekt zurück.
### isCrossProject() {#isCrossProject--}
```
public final boolean isCrossProject()
```


Liefert einen Wert, der angibt, ob ein Vorgänger Teil eines anderen Projekts ist.

**Returns:**
boolean - ein Wert, der angibt, ob ein Vorgänger Teil eines anderen Projekts ist.
### setCrossProject(boolean value) {#setCrossProject-boolean-}
```
public final void setCrossProject(boolean value)
```


Setzt einen Wert, der angibt, ob ein Vorgänger Teil eines anderen Projekts ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob ein Vorgänger Teil eines anderen Projekts ist. |

### setCrossProjectName(String value) {#setCrossProjectName-java.lang.String-}
```
public final void setCrossProjectName(String value)
```


Setzt das externe Vorgängerprojekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | das externe Vorgängerprojekt. |

### setLagFormat(byte value) {#setLagFormat-byte-}
```
public final void setLagFormat(byte value)
```


Setzt das Format zur Angabe des Verzugs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte | das Format zur Angabe des Verzugs. |

### setLinkLag(int value) {#setLinkLag-int-}
```
public final void setLinkLag(int value)
```


Setzt den Verzug in Zehntel einer Minute oder Prozent.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | der Verzug in Zehntel einer Minute oder Prozent. |

### setLinkLagTimeSpan(double value) {#setLinkLagTimeSpan-double-}
```
public final void setLinkLagTimeSpan(double value)
```


Setzt die Verzugsdauer, abhängig vom LagFormat.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | Lagdauer, abhängig von LagFormat. |

### setLinkType(int value) {#setLinkType-int-}
```
public final void setLinkType(int value)
```


Setzt den Typ einer Verknüpfung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Der Typ eines Links. |

### setPredTask(Task value) {#setPredTask-com.aspose.tasks.Task-}
```
public final void setPredTask(Task value)
```


Setzt die Vorgängeraufgabe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | Die Vorgängeraufgabe. |

### setSuccTask(Task value) {#setSuccTask-com.aspose.tasks.Task-}
```
public final void setSuccTask(Task value)
```


Setzt die Nachfolgeraufgabe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | Die Nachfolgeraufgabe. |

### toString() {#toString--}
```
public String toString()
```


Gibt die Zeichenkettenrepräsentation eines TaskLink zurück. Die genauen Details der Darstellung sind nicht spezifiziert und können sich ändern.

**Returns:**
java.lang.String - Zeichenkette, die das TaskLink-Objekt darstellt.
