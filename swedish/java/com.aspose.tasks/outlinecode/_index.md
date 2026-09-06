---
title: "OutlineCode"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar ett värde för en outline-kod."
type: docs
weight: 167
url: /sv/java/com.aspose.tasks/outlinecode/
---

**Inheritance:**
java.lang.Object
```
public class OutlineCode
```

Representerar ett värde för en outline-kod.

--------------------

Två datadelar krävs – en pekare till outline‑kodtabellen som anges av FieldId, och värdet som anges antingen av ValueId eller ValueGuid‑pekaren till värdelistan.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [OutlineCode()](#OutlineCode--) | Initierar en ny instans av klassen [OutlineCode](../../com.aspose.tasks/outlinecode). |
| [OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)](#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-) | Initierar en ny instans av klassen [OutlineCode](../../com.aspose.tasks/outlinecode) med den angivna Outline Code och ett av dess värden. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getFieldId()](#getFieldId--) | Hämtar numeriskt värde för det anpassade fältet project Id. |
| [getValueGuid()](#getValueGuid--) | Hämtar GUID för värdet i värdelistan. |
| [getValueId()](#getValueId--) | Hämtar Id i värdelistan som är associerat med definitionen i outline-kodsamlingen. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | Ställer in numeriskt värde för det anpassade fältet project Id. |
| [setValueGuid(String value)](#setValueGuid-java.lang.String-) | Ställer in GUID för värdet i värdelistan. |
| [setValueId(int value)](#setValueId-int-) | Ställer in Id i värdelistan som är associerat med definitionen i outline-kodsamlingen. |
### OutlineCode() {#OutlineCode--}
```
public OutlineCode()
```


Initierar en ny instans av klassen [OutlineCode](../../com.aspose.tasks/outlinecode).

### OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue) {#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-}
```
public OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)
```


Initierar en ny instans av klassen [OutlineCode](../../com.aspose.tasks/outlinecode) med den angivna Outline Code och ett av dess värden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| codeDefinition | [OutlineCodeDefinition](../../com.aspose.tasks/outlinecodedefinition) | outline-koddefinition. |
| outlineValue | [OutlineValue](../../com.aspose.tasks/outlinevalue) | ett av outline-koddefinitionens värden. |

### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Hämtar numeriskt värde för det anpassade fältet project Id.

**Returns:**
java.lang.String - det numeriska värdet för det anpassade fältet project Id.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


Hämtar GUID för värdet i värdelistan. ValueGuid matchar FieldGuid i värdelistan.

**Returns:**
java.lang.String - GUID för värdet i värdelistan.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


Hämtar Id i värdelistan som är associerat med definitionen i outline-kodsamlingen.

**Returns:**
int - Id i värdelistan som är associerat med definitionen i outline-kodsamlingen.
### setFieldId(String value) {#setFieldId-java.lang.String-}
```
public final void setFieldId(String value)
```


Ställer in numeriskt värde för det anpassade fältet project Id.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | det numeriska värdet för det anpassade fältet project Id. |

### setValueGuid(String value) {#setValueGuid-java.lang.String-}
```
public final void setValueGuid(String value)
```


Ställer in GUID för värdet i värdelistan. ValueGuid matchar FieldGuid i värdelistan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | GUID för värdet i värdelistan. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


Ställer in Id i värdelistan som är associerat med definitionen i outline-kodsamlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | Id i värdelistan som är associerat med definitionen i outline-kodsamlingen. |

