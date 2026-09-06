---
title: "OutlineValue"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar ett outline-värde."
type: docs
weight: 173
url: /sv/java/com.aspose.tasks/outlinevalue/
---

**Inheritance:**
java.lang.Object
```
public class OutlineValue
```

Representerar ett outline-värde.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [OutlineValue()](#OutlineValue--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getDescription()](#getDescription--) | Hämtar beskrivningen av ett konturvärde. |
| [getDurationValue()](#getDurationValue--) | Hämtar varaktigheten om Type är Duration. |
| [getParentValueId()](#getParentValueId--) | Hämtar Id för en föräldraknutt av en konturkod. |
| [getType()](#getType--) | Hämtar konturkodens typ. |
| [getValue()](#getValue--) | Hämtar det faktiska värdet. |
| [getValueGuid()](#getValueGuid--) | Hämtar en GUID som identifierar detta värde bland andra i hela projektet. |
| [getValueId()](#getValueId--) | Hämtar det unika Id:t för ett konturkodsvärde inom ett projekt. |
| [isCollapsed()](#isCollapsed--) | Hämtar ett värde som indikerar om konturvärdet är kollapsat eller inte. |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | Ställer in ett värde som indikerar om konturvärdet är kollapsat eller inte. |
| [setDescription(String value)](#setDescription-java.lang.String-) | Ställer in beskrivningen av ett konturvärde. |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | Ställer in varaktigheten om Type är Duration. |
| [setParentValueId(int value)](#setParentValueId-int-) | Ställer in Id för en föräldraknutt av en konturkod. |
| [setType(int value)](#setType-int-) | Ställer in konturkodens typ. |
| [setValue(String value)](#setValue-java.lang.String-) | Ställer in det faktiska värdet. |
| [setValueId(int value)](#setValueId-int-) | Ställer in det unika Id:t för ett konturkodvärde inom ett projekt. |
### OutlineValue() {#OutlineValue--}
```
public OutlineValue()
```


### getDescription() {#getDescription--}
```
public final String getDescription()
```


Hämtar beskrivningen av ett konturvärde.

**Returns:**
java.lang.String - beskrivningen av ett konturvärde.
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


Hämtar varaktigheten om Type är Duration.

--------------------

Föredra denna egenskap framför `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)), när du behöver ange värdet för OutlineValues med Duration-typ.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration if Type is Duration.
### getParentValueId() {#getParentValueId--}
```
public final int getParentValueId()
```


Hämtar Id för en föräldraknutt av en konturkod.

**Returns:**
int - Id:t för en föräldranod i en konturkod.
### getType() {#getType--}
```
public final int getType()
```


Hämtar konturkodens typ.

**Returns:**
int - konturkodstypen.
### getValue() {#getValue--}
```
public final String getValue()
```


Hämtar det faktiska värdet.

**Returns:**
java.lang.String - det faktiska värdet.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


Hämtar en GUID som identifierar detta värde bland andra i hela projektet.

**Returns:**
java.util.UUID - ett GUID som identifierar detta värde bland andra i hela projektet.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


Hämtar det unika Id:t för ett konturkodsvärde inom ett projekt.

**Returns:**
int - det unika Id:t för ett konturkodvärde inom ett projekt.
### isCollapsed() {#isCollapsed--}
```
public final boolean isCollapsed()
```


Hämtar ett värde som indikerar om konturvärdet är kollapsat eller inte.

--------------------

Detta är nytt för MS Project 2010‑egenskapen.

**Returns:**
boolean - ett värde som indikerar om konturvärdet är kollapsat eller inte.
### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public final void setCollapsed(boolean value)
```


Ställer in ett värde som indikerar om konturvärdet är kollapsat eller inte.

--------------------

Detta är nytt för MS Project 2010‑egenskapen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | Ett värde som indikerar om konturvärdet är kollapsat eller inte. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


Ställer in beskrivningen av ett konturvärde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Beskrivningen av ett konturvärde. |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


Ställer in varaktigheten om Type är Duration.

--------------------

Föredra denna egenskap framför `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)), när du behöver ange värdet för OutlineValues med Duration-typ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Varaktigheten om typen är Duration. |

### setParentValueId(int value) {#setParentValueId-int-}
```
public final void setParentValueId(int value)
```


Ställer in Id för en föräldraknutt av en konturkod.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | Id:t för en föräldranod i en konturkod. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Ställer in konturkodens typ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | Konturkodstypen. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


Ställer in det faktiska värdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Det faktiska värdet. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


Ställer in det unika Id:t för ett konturkodvärde inom ett projekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | Det unika Id:t för ett konturkodvärde inom ett projekt. |

