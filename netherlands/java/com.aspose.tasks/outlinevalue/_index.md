---
title: "OutlineValue"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een outline-waarde voor."
type: docs
weight: 173
url: /nl/java/com.aspose.tasks/outlinevalue/
---

**Inheritance:**
java.lang.Object
```
public class OutlineValue
```

Stelt een outline-waarde voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [OutlineValue()](#OutlineValue--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getDescription()](#getDescription--) | Haalt de beschrijving van een outline-waarde op. |
| [getDurationValue()](#getDurationValue--) | Haalt de duur op als Type Duration is. |
| [getParentValueId()](#getParentValueId--) | Haalt de Id op van een bovenliggend knooppunt van een outline-code. |
| [getType()](#getType--) | Haalt het outline-code type op. |
| [getValue()](#getValue--) | Haalt de werkelijke waarde op. |
| [getValueGuid()](#getValueGuid--) | Haalt een GUID op die deze waarde identificeert tussen andere in het gehele project. |
| [getValueId()](#getValueId--) | Haalt de unieke Id op van een outline-codewaarde binnen een project. |
| [isCollapsed()](#isCollapsed--) | Haalt een waarde op die aangeeft of de outline-waarde is samengevouwen of niet. |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | Stelt een waarde in die aangeeft of de outline-waarde is samengevouwen of niet. |
| [setDescription(String value)](#setDescription-java.lang.String-) | Stelt de beschrijving van een outline-waarde in. |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | Stelt de duur in als Type Duration is. |
| [setParentValueId(int value)](#setParentValueId-int-) | Stelt de Id in van een bovenliggend knooppunt van een outline-code. |
| [setType(int value)](#setType-int-) | Stelt het outline-code type in. |
| [setValue(String value)](#setValue-java.lang.String-) | Stelt de werkelijke waarde in. |
| [setValueId(int value)](#setValueId-int-) | Stelt de unieke Id in van een outline-codewaarde binnen een project. |
### OutlineValue() {#OutlineValue--}
```
public OutlineValue()
```


### getDescription() {#getDescription--}
```
public final String getDescription()
```


Haalt de beschrijving van een outline-waarde op.

**Returns:**
java.lang.String - de beschrijving van een outline-waarde.
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


Haalt de duur op als Type Duration is.

--------------------

Geef de voorkeur aan deze eigenschap boven de `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)), wanneer je de waarde moet instellen voor OutlineValues met Duration type.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration if Type is Duration.
### getParentValueId() {#getParentValueId--}
```
public final int getParentValueId()
```


Haalt de Id op van een bovenliggend knooppunt van een outline-code.

**Returns:**
int - de Id van een bovenliggend knooppunt van een outline-code.
### getType() {#getType--}
```
public final int getType()
```


Haalt het outline-code type op.

**Returns:**
int - het outline-code type.
### getValue() {#getValue--}
```
public final String getValue()
```


Haalt de werkelijke waarde op.

**Returns:**
java.lang.String - de werkelijke waarde.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


Haalt een GUID op die deze waarde identificeert tussen andere in het gehele project.

**Returns:**
java.util.UUID - een GUID die deze waarde identificeert tussen andere waarden in het gehele project.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


Haalt de unieke Id op van een outline-codewaarde binnen een project.

**Returns:**
int - de unieke Id van een outline-codewaarde binnen een project.
### isCollapsed() {#isCollapsed--}
```
public final boolean isCollapsed()
```


Haalt een waarde op die aangeeft of de outline-waarde is samengevouwen of niet.

--------------------

Dit is een nieuwe eigenschap voor MS Project 2010.

**Returns:**
boolean - een waarde die aangeeft of de outline-waarde is samengevouwen of niet.
### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public final void setCollapsed(boolean value)
```


Stelt een waarde in die aangeeft of de outline-waarde is samengevouwen of niet.

--------------------

Dit is een nieuwe eigenschap voor MS Project 2010.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de outline-waarde is samengevouwen of niet. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


Stelt de beschrijving van een outline-waarde in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de beschrijving van een outline-waarde. |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


Stelt de duur in als Type Duration is.

--------------------

Geef de voorkeur aan deze eigenschap boven de `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)), wanneer je de waarde moet instellen voor OutlineValues met Duration type.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | de duur als Type Duration is. |

### setParentValueId(int value) {#setParentValueId-int-}
```
public final void setParentValueId(int value)
```


Stelt de Id in van een bovenliggend knooppunt van een outline-code.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de Id van een bovenliggend knooppunt van een outline-code. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Stelt het outline-code type in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het type outline-code. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


Stelt de werkelijke waarde in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de werkelijke waarde. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


Stelt de unieke Id in van een outline-codewaarde binnen een project.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de unieke Id van een outline-codewaarde binnen een project. |

