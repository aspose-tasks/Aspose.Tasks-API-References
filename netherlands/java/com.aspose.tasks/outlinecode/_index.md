---
title: "OutlineCode"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een waarde van een outline-code voor."
type: docs
weight: 167
url: /nl/java/com.aspose.tasks/outlinecode/
---

**Inheritance:**
java.lang.Object
```
public class OutlineCode
```

Stelt een waarde van een outline-code voor.

--------------------

Twee gegevensstukken zijn nodig - een verwijzing naar de outline-code tabel die wordt gespecificeerd door de FieldId, en de waarde die wordt gespecificeerd door ofwel de ValueId of de ValueGuid verwijzing naar de waardelijst.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [OutlineCode()](#OutlineCode--) | Initialiseert een nieuw exemplaar van de [OutlineCode](../../com.aspose.tasks/outlinecode) klasse. |
| [OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)](#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-) | Initialiseert een nieuw exemplaar van de [OutlineCode](../../com.aspose.tasks/outlinecode) klasse met de opgegeven Outline Code en een van zijn waarden. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getFieldId()](#getFieldId--) | Haalt de numerieke waarde op van het aangepaste veld project-ID. |
| [getValueGuid()](#getValueGuid--) | Haalt de GUID op van de waarde in de waardelijst. |
| [getValueId()](#getValueId--) | Haalt de Id op in de waardelijst die gekoppeld is aan de definitie in de outline-code collectie. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | Stelt de numerieke waarde in van het aangepaste veld project-ID. |
| [setValueGuid(String value)](#setValueGuid-java.lang.String-) | Stelt de GUID in van de waarde in de waardelijst. |
| [setValueId(int value)](#setValueId-int-) | Stelt de Id in in de waardelijst die gekoppeld is aan de definitie in de outline-code collectie. |
### OutlineCode() {#OutlineCode--}
```
public OutlineCode()
```


Initialiseert een nieuw exemplaar van de [OutlineCode](../../com.aspose.tasks/outlinecode) klasse.

### OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue) {#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-}
```
public OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)
```


Initialiseert een nieuw exemplaar van de [OutlineCode](../../com.aspose.tasks/outlinecode) klasse met de opgegeven Outline Code en een van zijn waarden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| codeDefinition | [OutlineCodeDefinition](../../com.aspose.tasks/outlinecodedefinition) | outline code definitie. |
| outlineValue | [OutlineValue](../../com.aspose.tasks/outlinevalue) | een van de outline code definitiewaarden. |

### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Haalt de numerieke waarde op van het aangepaste veld project-ID.

**Returns:**
java.lang.String - de numerieke waarde van het aangepaste veld project Id.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


Haalt de GUID op van de waarde in de waardelijst. De ValueGuid komt overeen met de FieldGuid in de waardelijst.

**Returns:**
java.lang.String - de GUID van de waarde in de waardelijst.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


Haalt de Id op in de waardelijst die gekoppeld is aan de definitie in de outline-code collectie.

**Returns:**
int - de Id in de waardelijst die is gekoppeld aan de definitie in de outline code collectie.
### setFieldId(String value) {#setFieldId-java.lang.String-}
```
public final void setFieldId(String value)
```


Stelt de numerieke waarde in van het aangepaste veld project-ID.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de numerieke waarde van het aangepaste veld project Id. |

### setValueGuid(String value) {#setValueGuid-java.lang.String-}
```
public final void setValueGuid(String value)
```


Stelt de GUID in van de waarde in de waardelijst. De ValueGuid komt overeen met de FieldGuid in de waardelijst.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de GUID van de waarde in de waardelijst. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


Stelt de Id in in de waardelijst die gekoppeld is aan de definitie in de outline-code collectie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de Id in de waardelijst die is gekoppeld aan de definitie in de outline code collectie. |

