---
title: "ExtendedAttribute"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar utökade attribut."
type: docs
weight: 81
url: /sv/java/com.aspose.tasks/extendedattribute/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttribute
```

Representerar utökade attribut.

--------------------

För närvarande stöds alla typer av Extended attributes som läses från MSP Xml 2003/2007 och mpp 2003. För MSP mpp 2007 stöds läsning av alla Extended attributes förutom varaktigheter och flaggor.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getAttributeDefinition()](#getAttributeDefinition--) | Hämtar attributdefinitionen. |
| [getDateValue()](#getDateValue--) | Hämtar ett värde för attribut med datumtyper (Date, Start, Finish). |
| [getDurationValue()](#getDurationValue--) | Hämtar värde för attribut med typen 'Duration'. |
| [getFieldId()](#getFieldId--) | Hämtar id för ett fält. |
| [getFlagValue()](#getFlagValue--) | Hämtar ett värde som indikerar om en flagga är satt för ett attribut med typen 'Flag'. |
| [getNumericValue()](#getNumericValue--) | Hämtar ett värde för attribut med numeriska typer (Cost, Number). |
| [getTextValue()](#getTextValue--) | Hämtar ett värde för attribut med typen 'Text'. |
| [getValueGuid()](#getValueGuid--) | Hämtar guid för ett uppslagsvärde. |
| [getValueReadOnly()](#getValueReadOnly--) | Hämtar ett värde som indikerar om ett värde för denna [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) instans är skrivskyddad. |
| [isErrorValue()](#isErrorValue--) | Hämtar om beräkning av extended attribute's värde resulterade i ett fel. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | Sätter ett värde för attribut med datumtyper (Date, Start, Finish). |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | Sätter värde för attribut med typen 'Duration'. |
| [setFlagValue(boolean value)](#setFlagValue-boolean-) | Sätter ett värde som indikerar om en flagga är satt för ett attribut med typen 'Flag'. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Sätter ett värde för attribut med numeriska typer (Cost, Number). |
| [setTextValue(String value)](#setTextValue-java.lang.String-) | Sätter ett värde för attribut med typen 'Text'. |
| [toString()](#toString--) | Returnerar kort strängrepresentation av ett extended attribute. |
### getAttributeDefinition() {#getAttributeDefinition--}
```
public final ExtendedAttributeDefinition getAttributeDefinition()
```


Hämtar attributdefinitionen.

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - the attribute definition.
### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


Hämtar ett värde för attribut med datumtyper (Date, Start, Finish).

**Returns:**
java.util.Date - ett värde för attribut med datumtyper (Date, Start, Finish).
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


Hämtar värde för attribut med typen 'Duration'.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - value for attributes with 'Duration' type.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Hämtar id för ett fält.

**Returns:**
java.lang.String - id för ett fält.
### getFlagValue() {#getFlagValue--}
```
public final boolean getFlagValue()
```


Hämtar ett värde som indikerar om en flagga är satt för ett attribut med typen 'Flag'.

**Returns:**
boolean - ett värde som indikerar om en flagga är satt för ett attribut med typen 'Flag'.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Hämtar ett värde för attribut med numeriska typer (Cost, Number).

**Returns:**
java.math.BigDecimal - ett värde för attribut med numeriska typer (Cost, Number).
### getTextValue() {#getTextValue--}
```
public final String getTextValue()
```


Hämtar ett värde för attribut med typen 'Text'.

**Returns:**
java.lang.String - ett värde för attribut med typen 'Text'.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


Hämtar guid för ett uppslagsvärde.

--------------------

Bör inte sättas direkt, använd istället ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) för att skapa ett utökat attribut med ett uppslagsvärde.

**Returns:**
java.lang.String - GUID för ett uppslagsvärde.
### getValueReadOnly() {#getValueReadOnly--}
```
public final boolean getValueReadOnly()
```


Hämtar ett värde som indikerar om ett värde för denna [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) instans är skrivskyddad.

Värde: returnerar true om en formel eller sammanställning är definierad i [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) för detta objekt.

**Returns:**
boolean - ett värde som indikerar om ett värde för denna [ExtendedAttribute](../../com.aspose.tasks/extendedattribute)-instans är skrivskyddat.
### isErrorValue() {#isErrorValue--}
```
public final boolean isErrorValue()
```


Hämtar om beräkning av extended attribute's värde resulterade i ett fel.

**Returns:**
boolean - om beräkning av det utökade attributets värde resulterade i ett fel.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


Sätter ett värde för attribut med datumtyper (Date, Start, Finish).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | ett värde för attribut med datumtyper (Date, Start, Finish). |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


Sätter värde för attribut med typen 'Duration'.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ett värde för attribut med typen 'Duration'. |

### setFlagValue(boolean value) {#setFlagValue-boolean-}
```
public final void setFlagValue(boolean value)
```


Sätter ett värde som indikerar om en flagga är satt för ett attribut med typen 'Flag'.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om en flagga är satt för ett attribut med typen 'Flag'. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Sätter ett värde för attribut med numeriska typer (Cost, Number).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | ett värde för attribut med numeriska typer (Cost, Number). |

### setTextValue(String value) {#setTextValue-java.lang.String-}
```
public final void setTextValue(String value)
```


Sätter ett värde för attribut med typen 'Text'.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett värde för attribut med typen 'Text'. |

### toString() {#toString--}
```
public String toString()
```


Returnerar kort strängrepresentation av ett extended attribute.

**Returns:**
java.lang.String - Strängrepresentationen av det utökade attributet.
