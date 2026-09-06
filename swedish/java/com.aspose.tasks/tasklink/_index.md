---
title: "TaskLink"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en föregångarlänk."
type: docs
weight: 295
url: /sv/java/com.aspose.tasks/tasklink/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public final class TaskLink implements System.IEquatable<TaskLink>
```

Representerar en föregångarlänk.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(TaskLink other)](#equals-com.aspose.tasks.TaskLink-) | Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt. |
| [getCrossProjectName()](#getCrossProjectName--) | Hämtar det externa föregående projektet. |
| [getLagFormat()](#getLagFormat--) | Hämtar formatet för att uttrycka lagformatet. |
| [getLinkLag()](#getLinkLag--) | Hämtar fördröjningen i tiondelar av en minut eller i procent. |
| [getLinkLagTimeSpan()](#getLinkLagTimeSpan--) | Hämtar fördröjningens varaktighet, beroende på LagFormat. |
| [getLinkType()](#getLinkType--) | Hämtar typen av en länk. |
| [getPredTask()](#getPredTask--) | Hämtar föregående uppgift. |
| [getSuccTask()](#getSuccTask--) | Hämtar efterföljande uppgift. |
| [hashCode()](#hashCode--) | Returnerar ett hashkodvärde för instansen av klassen [TaskLink](../../com.aspose.tasks/tasklink). |
| [isCrossProject()](#isCrossProject--) | Hämtar ett värde som indikerar om en föregångare är en del av ett annat projekt. |
| [setCrossProject(boolean value)](#setCrossProject-boolean-) | Ställer in ett värde som indikerar om en föregångare är en del av ett annat projekt. |
| [setCrossProjectName(String value)](#setCrossProjectName-java.lang.String-) | Ställer in det externa föregående projektet. |
| [setLagFormat(byte value)](#setLagFormat-byte-) | Ställer in formatet för att uttrycka lagformatet. |
| [setLinkLag(int value)](#setLinkLag-int-) | Ställer in fördröjningen i tiondelar av en minut eller procent. |
| [setLinkLagTimeSpan(double value)](#setLinkLagTimeSpan-double-) | Ställer in fördröjningens varaktighet, beroende på LagFormat. |
| [setLinkType(int value)](#setLinkType-int-) | Ställer in typen av en länk. |
| [setPredTask(Task value)](#setPredTask-com.aspose.tasks.Task-) | Ställer in föregående uppgift. |
| [setSuccTask(Task value)](#setSuccTask-com.aspose.tasks.Task-) | Ställer in efterföljande uppgift. |
| [toString()](#toString--) | Returnerar strängrepresentation av en TaskLink. |
### equals(TaskLink other) {#equals-com.aspose.tasks.TaskLink-}
```
public final boolean equals(TaskLink other)
```


Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [TaskLink](../../com.aspose.tasks/tasklink) | Den angivna instansen av klassen [TaskLink](../../com.aspose.tasks/tasklink) för att jämföra med denna instans. |

**Returns:**
boolean - **True** om den angivna instansen av klassen [TaskLink](../../com.aspose.tasks/tasklink) har samma föregående och efterföljande uppgifter som denna instans; annars, **false**.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | Objektet att jämföra med denna instans. |

**Returns:**
boolean - **True** om det angivna objektet är en TaskLink som har samma föregående och efterföljande som denna instans; annars, **false**.
### getCrossProjectName() {#getCrossProjectName--}
```
public final String getCrossProjectName()
```


Hämtar det externa föregående projektet.

**Returns:**
java.lang.String - det externa föregående projektet.
### getLagFormat() {#getLagFormat--}
```
public final byte getLagFormat()
```


Hämtar formatet för att uttrycka lagformatet.

**Returns:**
byte - formatet för att uttrycka fördröjningsformatet.
### getLinkLag() {#getLinkLag--}
```
public final int getLinkLag()
```


Hämtar fördröjningen i tiondelar av en minut eller i procent.

**Returns:**
int - fördröjningen i tiondelar av en minut eller procent.
### getLinkLagTimeSpan() {#getLinkLagTimeSpan--}
```
public final double getLinkLagTimeSpan()
```


Hämtar fördröjningens varaktighet, beroende på LagFormat.

**Returns:**
double - fördröjningens varaktighet, beroende på LagFormat.
### getLinkType() {#getLinkType--}
```
public final int getLinkType()
```


Hämtar typen av en länk.

**Returns:**
int - typen av en länk.
### getPredTask() {#getPredTask--}
```
public final Task getPredTask()
```


Hämtar föregående uppgift.

**Returns:**
[Task](../../com.aspose.tasks/task) - the predecessor task.
### getSuccTask() {#getSuccTask--}
```
public final Task getSuccTask()
```


Hämtar efterföljande uppgift.

**Returns:**
[Task](../../com.aspose.tasks/task) - the successor task.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returnerar ett hashkodvärde för instansen av klassen [TaskLink](../../com.aspose.tasks/tasklink).

**Returns:**
int - returnerar ett hash‑kodvärde för detta objekt.
### isCrossProject() {#isCrossProject--}
```
public final boolean isCrossProject()
```


Hämtar ett värde som indikerar om en föregångare är en del av ett annat projekt.

**Returns:**
boolean - ett värde som indikerar om en föregående är en del av ett annat projekt.
### setCrossProject(boolean value) {#setCrossProject-boolean-}
```
public final void setCrossProject(boolean value)
```


Ställer in ett värde som indikerar om en föregångare är en del av ett annat projekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om en föregående är en del av ett annat projekt. |

### setCrossProjectName(String value) {#setCrossProjectName-java.lang.String-}
```
public final void setCrossProjectName(String value)
```


Ställer in det externa föregående projektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | det externa föregående projektet. |

### setLagFormat(byte value) {#setLagFormat-byte-}
```
public final void setLagFormat(byte value)
```


Ställer in formatet för att uttrycka lagformatet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | byte | formatet för att uttrycka fördröjningsformatet. |

### setLinkLag(int value) {#setLinkLag-int-}
```
public final void setLinkLag(int value)
```


Ställer in fördröjningen i tiondelar av en minut eller procent.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | fördröjningen i tiondelar av en minut eller procent. |

### setLinkLagTimeSpan(double value) {#setLinkLagTimeSpan-double-}
```
public final void setLinkLagTimeSpan(double value)
```


Ställer in fördröjningens varaktighet, beroende på LagFormat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | fördröjningens varaktighet, beroende på LagFormat. |

### setLinkType(int value) {#setLinkType-int-}
```
public final void setLinkType(int value)
```


Ställer in typen av en länk.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | typen av en länk. |

### setPredTask(Task value) {#setPredTask-com.aspose.tasks.Task-}
```
public final void setPredTask(Task value)
```


Ställer in föregående uppgift.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | föregående uppgift. |

### setSuccTask(Task value) {#setSuccTask-com.aspose.tasks.Task-}
```
public final void setSuccTask(Task value)
```


Ställer in efterföljande uppgift.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | efterföljande uppgift. |

### toString() {#toString--}
```
public String toString()
```


Returnerar strängrepresentation av en TaskLink. De exakta detaljerna för representationen är ospecificerade och kan komma att ändras.

**Returns:**
java.lang.String - sträng som representerar TaskLink-objekt.
