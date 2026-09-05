---
title: "ExtendedAttribute"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt uitgebreide attributen voor."
type: docs
weight: 81
url: /nl/java/com.aspose.tasks/extendedattribute/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttribute
```

Stelt uitgebreide attributen voor.

--------------------

Momenteel worden alle typen uitgebreide attributen ondersteund die worden gelezen uit MSP Xml 2003/2007 en mpp 2003. Voor MSP mpp 2007 worden alle uitgebreide attributen gelezen, behalve duur en vlaggen.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getAttributeDefinition()](#getAttributeDefinition--) | Haalt de attribuutdefinitie op. |
| [getDateValue()](#getDateValue--) | Haalt een waarde op voor attributen met datumtypes (Date, Start, Finish). |
| [getDurationValue()](#getDurationValue--) | Haalt de waarde op voor attributen met het type 'Duration'. |
| [getFieldId()](#getFieldId--) | Haalt de id op van een veld. |
| [getFlagValue()](#getFlagValue--) | Haalt een waarde op die aangeeft of een vlag is ingesteld voor een attribuut met het type 'Flag'. |
| [getNumericValue()](#getNumericValue--) | Haalt een waarde op voor attributen met numerieke types (Cost, Number). |
| [getTextValue()](#getTextValue--) | Haalt een waarde op voor attributen met het type 'Text'. |
| [getValueGuid()](#getValueGuid--) | Haalt de guid op van een lookup-waarde. |
| [getValueReadOnly()](#getValueReadOnly--) | Haalt een waarde op die aangeeft of een waarde van deze [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) instantie alleen-lezen is. |
| [isErrorValue()](#isErrorValue--) | Haalt op of de berekening van de waarde van het uitgebreide attribuut in een fout is geëindigd. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | Stelt een waarde in voor attributen met datumtypes (Date, Start, Finish). |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | Stelt een waarde in voor attributen met het type 'Duration'. |
| [setFlagValue(boolean value)](#setFlagValue-boolean-) | Stelt een waarde in die aangeeft of een vlag is ingesteld voor een attribuut met het type 'Flag'. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Stelt een waarde in voor attributen met numerieke types (Cost, Number). |
| [setTextValue(String value)](#setTextValue-java.lang.String-) | Stelt een waarde in voor attributen met het type 'Text'. |
| [toString()](#toString--) | Retourneert een korte tekenreeksrepresentatie van een uitgebreid attribuut. |
### getAttributeDefinition() {#getAttributeDefinition--}
```
public final ExtendedAttributeDefinition getAttributeDefinition()
```


Haalt de attribuutdefinitie op.

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - the attribute definition.
### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


Haalt een waarde op voor attributen met datumtypes (Date, Start, Finish).

**Returns:**
java.util.Date - een waarde voor attributen met datumtypes (Date, Start, Finish).
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


Haalt de waarde op voor attributen met het type 'Duration'.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - value for attributes with 'Duration' type.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Haalt de id op van een veld.

**Returns:**
java.lang.String - de id van een veld.
### getFlagValue() {#getFlagValue--}
```
public final boolean getFlagValue()
```


Haalt een waarde op die aangeeft of een vlag is ingesteld voor een attribuut met het type 'Flag'.

**Returns:**
boolean - een waarde die aangeeft of een vlag is ingesteld voor een attribuut met het type 'Flag'.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Haalt een waarde op voor attributen met numerieke types (Cost, Number).

**Returns:**
java.math.BigDecimal - een waarde voor attributen met numerieke types (Cost, Number).
### getTextValue() {#getTextValue--}
```
public final String getTextValue()
```


Haalt een waarde op voor attributen met het type 'Text'.

**Returns:**
java.lang.String - een waarde voor attributen met het type 'Text'.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


Haalt de guid op van een lookup-waarde.

--------------------

Mag niet rechtstreeks worden ingesteld, gebruik in plaats daarvan ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) om een uitgebreid attribuut met een lookup-waarde te maken.

**Returns:**
java.lang.String - de guid van een lookup-waarde.
### getValueReadOnly() {#getValueReadOnly--}
```
public final boolean getValueReadOnly()
```


Haalt een waarde op die aangeeft of een waarde van deze [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) instantie alleen-lezen is.

Waarde: retourneert true als een formule of rollup is gedefinieerd in de [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) voor dit object.

**Returns:**
boolean - een waarde die aangeeft of een waarde van deze [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) instantie alleen-lezen is.
### isErrorValue() {#isErrorValue--}
```
public final boolean isErrorValue()
```


Haalt op of de berekening van de waarde van het uitgebreide attribuut in een fout is geëindigd.

**Returns:**
boolean - of de berekening van de waarde van het uitgebreide attribuut in een fout is geëindigd.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


Stelt een waarde in voor attributen met datumtypes (Date, Start, Finish).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | een waarde voor attributen met datumtypes (Date, Start, Finish). |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


Stelt een waarde in voor attributen met het type 'Duration'.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | waarde voor attributen met type 'Duration'. |

### setFlagValue(boolean value) {#setFlagValue-boolean-}
```
public final void setFlagValue(boolean value)
```


Stelt een waarde in die aangeeft of een vlag is ingesteld voor een attribuut met het type 'Flag'.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of een vlag is ingesteld voor een attribuut met type 'Flag'. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Stelt een waarde in voor attributen met numerieke types (Cost, Number).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | een waarde voor attributen met numerieke types (Cost, Number). |

### setTextValue(String value) {#setTextValue-java.lang.String-}
```
public final void setTextValue(String value)
```


Stelt een waarde in voor attributen met het type 'Text'.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een waarde voor attributen met type 'Text'. |

### toString() {#toString--}
```
public String toString()
```


Retourneert een korte tekenreeksrepresentatie van een uitgebreid attribuut.

**Returns:**
java.lang.String - De tekenreeksrepresentatie van het uitgebreide attribuut.
