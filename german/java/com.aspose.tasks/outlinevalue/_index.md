---
title: "OutlineValue"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt einen Gliederungswert dar."
type: docs
weight: 173
url: /de/java/com.aspose.tasks/outlinevalue/
---

**Inheritance:**
java.lang.Object
```
public class OutlineValue
```

Stellt einen Gliederungswert dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [OutlineValue()](#OutlineValue--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getDescription()](#getDescription--) | Ruft die Beschreibung eines Outline-Werts ab. |
| [getDurationValue()](#getDurationValue--) | Ruft die Dauer ab, wenn Typ Dauer ist. |
| [getParentValueId()](#getParentValueId--) | Ruft die Id eines übergeordneten Knotens eines Outline-Codes ab. |
| [getType()](#getType--) | Ruft den Outline-Code-Typ ab. |
| [getValue()](#getValue--) | Ruft den tatsächlichen Wert ab. |
| [getValueGuid()](#getValueGuid--) | Ruft eine GUID ab, die diesen Wert im gesamten Projekt unter anderen identifiziert. |
| [getValueId()](#getValueId--) | Ruft die eindeutige Id eines Outline-Code-Werts innerhalb eines Projekts ab. |
| [isCollapsed()](#isCollapsed--) | Ruft einen Wert ab, der angibt, ob der Outline-Wert zusammengeklappt ist oder nicht. |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | Setzt einen Wert, der angibt, ob der Outline-Wert zusammengeklappt ist oder nicht. |
| [setDescription(String value)](#setDescription-java.lang.String-) | Setzt die Beschreibung eines Outline-Werts. |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | Setzt die Dauer, wenn Typ Dauer ist. |
| [setParentValueId(int value)](#setParentValueId-int-) | Legt die Id eines übergeordneten Knotens eines Gliederungscodes fest. |
| [setType(int value)](#setType-int-) | Legt den Typ des Gliederungscodes fest. |
| [setValue(String value)](#setValue-java.lang.String-) | Legt den tatsächlichen Wert fest. |
| [setValueId(int value)](#setValueId-int-) | Legt die eindeutige Id eines Gliederungscodewerts innerhalb eines Projekts fest. |
### OutlineValue() {#OutlineValue--}
```
public OutlineValue()
```


### getDescription() {#getDescription--}
```
public final String getDescription()
```


Ruft die Beschreibung eines Outline-Werts ab.

**Returns:**
java.lang.String – die Beschreibung eines Gliederungswerts.
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


Ruft die Dauer ab, wenn Typ Dauer ist.

--------------------

Verwenden Sie diese Eigenschaft anstelle von `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)), wenn Sie den Wert für OutlineValues mit dem Typ Duration festlegen müssen.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration if Type is Duration.
### getParentValueId() {#getParentValueId--}
```
public final int getParentValueId()
```


Ruft die Id eines übergeordneten Knotens eines Outline-Codes ab.

**Returns:**
int – die Id eines übergeordneten Knotens eines Gliederungscodes.
### getType() {#getType--}
```
public final int getType()
```


Ruft den Outline-Code-Typ ab.

**Returns:**
int – der Typ des Gliederungscodes.
### getValue() {#getValue--}
```
public final String getValue()
```


Ruft den tatsächlichen Wert ab.

**Returns:**
java.lang.String – der tatsächliche Wert.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


Ruft eine GUID ab, die diesen Wert im gesamten Projekt unter anderen identifiziert.

**Returns:**
java.util.UUID - ein GUID, das diesen Wert im gesamten Projekt eindeutig identifiziert.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


Ruft die eindeutige Id eines Outline-Code-Werts innerhalb eines Projekts ab.

**Returns:**
int – die eindeutige Id eines Gliederungscodewerts innerhalb eines Projekts.
### isCollapsed() {#isCollapsed--}
```
public final boolean isCollapsed()
```


Ruft einen Wert ab, der angibt, ob der Outline-Wert zusammengeklappt ist oder nicht.

--------------------

Dies ist eine neue Eigenschaft für MS Project 2010.

**Returns:**
boolean – ein Wert, der angibt, ob der Gliederungswert zusammengeklappt ist oder nicht.
### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public final void setCollapsed(boolean value)
```


Setzt einen Wert, der angibt, ob der Outline-Wert zusammengeklappt ist oder nicht.

--------------------

Dies ist eine neue Eigenschaft für MS Project 2010.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob der Gliederungswert zusammengeklappt ist oder nicht. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


Setzt die Beschreibung eines Outline-Werts.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | die Beschreibung eines Gliederungswerts. |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


Setzt die Dauer, wenn Typ Dauer ist.

--------------------

Verwenden Sie diese Eigenschaft anstelle von `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)), wenn Sie den Wert für OutlineValues mit dem Typ Duration festlegen müssen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | die Dauer, wenn der Typ Duration ist. |

### setParentValueId(int value) {#setParentValueId-int-}
```
public final void setParentValueId(int value)
```


Legt die Id eines übergeordneten Knotens eines Gliederungscodes fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | die Id eines übergeordneten Knotens eines Gliederungscodes. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Legt den Typ des Gliederungscodes fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | der Typ des Gliederungscodes. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


Legt den tatsächlichen Wert fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | der tatsächliche Wert. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


Legt die eindeutige Id eines Gliederungscodewerts innerhalb eines Projekts fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | die eindeutige Id eines Gliederungscodewerts innerhalb eines Projekts. |

