---
title: "TaskLink"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een voorgangerkoppeling voor."
type: docs
weight: 295
url: /nl/java/com.aspose.tasks/tasklink/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public final class TaskLink implements System.IEquatable<TaskLink>
```

Stelt een voorgangerkoppeling voor.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [equals(TaskLink other)](#equals-com.aspose.tasks.TaskLink-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [getCrossProjectName()](#getCrossProjectName--) | Haalt het externe voorgangerproject op. |
| [getLagFormat()](#getLagFormat--) | Haalt het formaat op voor het uitdrukken van de vertraging. |
| [getLinkLag()](#getLinkLag--) | Haalt de vertraging op in tienden van een minuut of percentage. |
| [getLinkLagTimeSpan()](#getLinkLagTimeSpan--) | Haalt de duur van de vertraging op, afhankelijk van LagFormat. |
| [getLinkType()](#getLinkType--) | Haalt het type van een koppeling op. |
| [getPredTask()](#getPredTask--) | Haalt de voorganger-taak op. |
| [getSuccTask()](#getSuccTask--) | Haalt de opvolger-taak op. |
| [hashCode()](#hashCode--) | Retourneert een hashcode-waarde voor de instantie van de [TaskLink](../../com.aspose.tasks/tasklink) klasse. |
| [isCrossProject()](#isCrossProject--) | Haalt een waarde op die aangeeft of een voorganger deel uitmaakt van een ander project. |
| [setCrossProject(boolean value)](#setCrossProject-boolean-) | Stelt een waarde in die aangeeft of een voorganger deel uitmaakt van een ander project. |
| [setCrossProjectName(String value)](#setCrossProjectName-java.lang.String-) | Stelt het externe voorgangerproject in. |
| [setLagFormat(byte value)](#setLagFormat-byte-) | Stelt het formaat in voor het uitdrukken van de vertraging. |
| [setLinkLag(int value)](#setLinkLag-int-) | Stelt de vertraging in in tienden van een minuut of percentage. |
| [setLinkLagTimeSpan(double value)](#setLinkLagTimeSpan-double-) | Stelt de duur van de vertraging in, afhankelijk van LagFormat. |
| [setLinkType(int value)](#setLinkType-int-) | Stelt het type van een koppeling in. |
| [setPredTask(Task value)](#setPredTask-com.aspose.tasks.Task-) | Stelt de voorganger-taak in. |
| [setSuccTask(Task value)](#setSuccTask-com.aspose.tasks.Task-) | Stelt de opvolger-taak in. |
| [toString()](#toString--) | Retourneert de tekenreeksrepresentatie van een TaskLink. |
### equals(TaskLink other) {#equals-com.aspose.tasks.TaskLink-}
```
public final boolean equals(TaskLink other)
```


Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | [TaskLink](../../com.aspose.tasks/tasklink) | De opgegeven instantie van de [TaskLink](../../com.aspose.tasks/tasklink) klasse om te vergelijken met deze instantie. |

**Returns:**
boolean - **True** als de opgegeven instantie van de [TaskLink](../../com.aspose.tasks/tasklink) klasse dezelfde voorganger- en opvolgertaken heeft als deze instantie; anders, **false**.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | java.lang.Object | Het object om te vergelijken met deze instantie. |

**Returns:**
boolean - **True** als het opgegeven object een TaskLink is die dezelfde voorganger en opvolger heeft als deze instantie; anders **false**.
### getCrossProjectName() {#getCrossProjectName--}
```
public final String getCrossProjectName()
```


Haalt het externe voorgangerproject op.

**Returns:**
java.lang.String - het externe voorgangerproject.
### getLagFormat() {#getLagFormat--}
```
public final byte getLagFormat()
```


Haalt het formaat op voor het uitdrukken van de vertraging.

**Returns:**
byte - het formaat voor het uitdrukken van het vertragingformaat.
### getLinkLag() {#getLinkLag--}
```
public final int getLinkLag()
```


Haalt de vertraging op in tienden van een minuut of percentage.

**Returns:**
int - de vertraging in tienden van een minuut of percentage.
### getLinkLagTimeSpan() {#getLinkLagTimeSpan--}
```
public final double getLinkLagTimeSpan()
```


Haalt de duur van de vertraging op, afhankelijk van LagFormat.

**Returns:**
double - vertragingstijd, afhankelijk van LagFormat.
### getLinkType() {#getLinkType--}
```
public final int getLinkType()
```


Haalt het type van een koppeling op.

**Returns:**
int - het type van een koppeling.
### getPredTask() {#getPredTask--}
```
public final Task getPredTask()
```


Haalt de voorganger-taak op.

**Returns:**
[Task](../../com.aspose.tasks/task) - the predecessor task.
### getSuccTask() {#getSuccTask--}
```
public final Task getSuccTask()
```


Haalt de opvolger-taak op.

**Returns:**
[Task](../../com.aspose.tasks/task) - the successor task.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Retourneert een hashcode-waarde voor de instantie van de [TaskLink](../../com.aspose.tasks/tasklink) klasse.

**Returns:**
int - retourneert een hashcode-waarde voor dit object.
### isCrossProject() {#isCrossProject--}
```
public final boolean isCrossProject()
```


Haalt een waarde op die aangeeft of een voorganger deel uitmaakt van een ander project.

**Returns:**
boolean - een waarde die aangeeft of een voorganger deel uitmaakt van een ander project.
### setCrossProject(boolean value) {#setCrossProject-boolean-}
```
public final void setCrossProject(boolean value)
```


Stelt een waarde in die aangeeft of een voorganger deel uitmaakt van een ander project.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of een voorganger deel uitmaakt van een ander project. |

### setCrossProjectName(String value) {#setCrossProjectName-java.lang.String-}
```
public final void setCrossProjectName(String value)
```


Stelt het externe voorgangerproject in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | het externe voorgangerproject. |

### setLagFormat(byte value) {#setLagFormat-byte-}
```
public final void setLagFormat(byte value)
```


Stelt het formaat in voor het uitdrukken van de vertraging.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | byte | het formaat voor het uitdrukken van het vertragingformaat. |

### setLinkLag(int value) {#setLinkLag-int-}
```
public final void setLinkLag(int value)
```


Stelt de vertraging in in tienden van een minuut of percentage.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de vertraging in tienden van een minuut of percentage. |

### setLinkLagTimeSpan(double value) {#setLinkLagTimeSpan-double-}
```
public final void setLinkLagTimeSpan(double value)
```


Stelt de duur van de vertraging in, afhankelijk van LagFormat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | vertragingstijd, afhankelijk van LagFormat. |

### setLinkType(int value) {#setLinkType-int-}
```
public final void setLinkType(int value)
```


Stelt het type van een koppeling in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het type van een koppeling. |

### setPredTask(Task value) {#setPredTask-com.aspose.tasks.Task-}
```
public final void setPredTask(Task value)
```


Stelt de voorganger-taak in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | de voorganger-taak. |

### setSuccTask(Task value) {#setSuccTask-com.aspose.tasks.Task-}
```
public final void setSuccTask(Task value)
```


Stelt de opvolger-taak in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | de opvolger-taak. |

### toString() {#toString--}
```
public String toString()
```


Retourneert de tekenreeksrepresentatie van een TaskLink. De exacte details van de representatie zijn niet gespecificeerd en kunnen wijzigen.

**Returns:**
java.lang.String - tekenreeks die een TaskLink-object vertegenwoordigt.
