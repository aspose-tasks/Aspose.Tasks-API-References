---
title: "ExtendedAttribute"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt erweiterte Attribute dar."
type: docs
weight: 81
url: /de/java/com.aspose.tasks/extendedattribute/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttribute
```

Stellt erweiterte Attribute dar.

--------------------

Derzeit werden alle Typen von Extended-Attributen aus MSP Xml 2003/2007 und mpp 2003 unterstützt. Für MSP mpp 2007 wird das Lesen aller Extended-Attribute unterstützt, außer Dauern und Flags.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getAttributeDefinition()](#getAttributeDefinition--) | Liefert die Attributdefinition. |
| [getDateValue()](#getDateValue--) | Liefert einen Wert für Attribute mit Datumstypen (Date, Start, Finish). |
| [getDurationValue()](#getDurationValue--) | Liefert den Wert für Attribute mit dem Typ 'Duration'. |
| [getFieldId()](#getFieldId--) | Liefert die ID eines Feldes. |
| [getFlagValue()](#getFlagValue--) | Liefert einen Wert, der angibt, ob ein Flag für ein Attribut mit dem Typ 'Flag' gesetzt ist. |
| [getNumericValue()](#getNumericValue--) | Liefert einen Wert für Attribute mit numerischen Typen (Cost, Number). |
| [getTextValue()](#getTextValue--) | Liefert einen Wert für Attribute mit dem Typ 'Text'. |
| [getValueGuid()](#getValueGuid--) | Liefert die GUID eines Lookup-Werts. |
| [getValueReadOnly()](#getValueReadOnly--) | Liefert einen Wert, der angibt, ob ein Wert dieser [ExtendedAttribute](../../com.aspose.tasks/extendedattribute)-Instanz schreibgeschützt ist. |
| [isErrorValue()](#isErrorValue--) | Liefert, ob die Berechnung des Werts des erweiterten Attributs zu einem Fehler geführt hat. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | Setzt einen Wert für Attribute mit Datumstypen (Date, Start, Finish). |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | Setzt den Wert für Attribute mit dem Typ 'Duration'. |
| [setFlagValue(boolean value)](#setFlagValue-boolean-) | Setzt einen Wert, der angibt, ob ein Flag für ein Attribut vom Typ 'Flag' gesetzt ist. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Setzt einen Wert für Attribute mit numerischen Typen (Cost, Number). |
| [setTextValue(String value)](#setTextValue-java.lang.String-) | Setzt einen Wert für Attribute vom Typ 'Text'. |
| [toString()](#toString--) | Gibt die kurze Zeichenkettenrepräsentation eines erweiterten Attributs zurück. |
### getAttributeDefinition() {#getAttributeDefinition--}
```
public final ExtendedAttributeDefinition getAttributeDefinition()
```


Liefert die Attributdefinition.

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - the attribute definition.
### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


Liefert einen Wert für Attribute mit Datumstypen (Date, Start, Finish).

**Returns:**
java.util.Date - ein Wert für Attribute mit Datumstypen (Date, Start, Finish).
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


Liefert den Wert für Attribute mit dem Typ 'Duration'.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - value for attributes with 'Duration' type.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Liefert die ID eines Feldes.

**Returns:**
java.lang.String - die ID eines Feldes.
### getFlagValue() {#getFlagValue--}
```
public final boolean getFlagValue()
```


Liefert einen Wert, der angibt, ob ein Flag für ein Attribut mit dem Typ 'Flag' gesetzt ist.

**Returns:**
boolean - ein Wert, der angibt, ob ein Flag für ein Attribut vom Typ 'Flag' gesetzt ist.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Liefert einen Wert für Attribute mit numerischen Typen (Cost, Number).

**Returns:**
java.math.BigDecimal - ein Wert für Attribute mit numerischen Typen (Cost, Number).
### getTextValue() {#getTextValue--}
```
public final String getTextValue()
```


Liefert einen Wert für Attribute mit dem Typ 'Text'.

**Returns:**
java.lang.String - ein Wert für Attribute vom Typ 'Text'.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


Liefert die GUID eines Lookup-Werts.

--------------------

Sollte nicht direkt gesetzt werden, sondern stattdessen ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) verwenden, um ein erweitertes Attribut mit einem Lookup-Wert zu erstellen.

**Returns:**
java.lang.String - die GUID eines Lookup-Werts.
### getValueReadOnly() {#getValueReadOnly--}
```
public final boolean getValueReadOnly()
```


Liefert einen Wert, der angibt, ob ein Wert dieser [ExtendedAttribute](../../com.aspose.tasks/extendedattribute)-Instanz schreibgeschützt ist.

Wert: gibt true zurück, wenn eine Formel oder Rollup in der [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) für dieses Objekt definiert ist.

**Returns:**
boolean - ein Wert, der angibt, ob ein Wert dieser [ExtendedAttribute](../../com.aspose.tasks/extendedattribute)-Instanz schreibgeschützt ist.
### isErrorValue() {#isErrorValue--}
```
public final boolean isErrorValue()
```


Liefert, ob die Berechnung des Werts des erweiterten Attributs zu einem Fehler geführt hat.

**Returns:**
boolean - ob die Berechnung des Werts des erweiterten Attributs zu einem Fehler geführt hat.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


Setzt einen Wert für Attribute mit Datumstypen (Date, Start, Finish).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | Ein Wert für Attribute mit Datumstypen (Date, Start, Finish). |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


Setzt den Wert für Attribute mit dem Typ 'Duration'.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Wert für Attribute vom Typ 'Duration'. |

### setFlagValue(boolean value) {#setFlagValue-boolean-}
```
public final void setFlagValue(boolean value)
```


Setzt einen Wert, der angibt, ob ein Flag für ein Attribut vom Typ 'Flag' gesetzt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | Ein Wert, der angibt, ob ein Flag für ein Attribut vom Typ 'Flag' gesetzt ist. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Setzt einen Wert für Attribute mit numerischen Typen (Cost, Number).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | Ein Wert für Attribute mit numerischen Typen (Cost, Number). |

### setTextValue(String value) {#setTextValue-java.lang.String-}
```
public final void setTextValue(String value)
```


Setzt einen Wert für Attribute vom Typ 'Text'.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Ein Wert für Attribute vom Typ 'Text'. |

### toString() {#toString--}
```
public String toString()
```


Gibt die kurze Zeichenkettenrepräsentation eines erweiterten Attributs zurück.

**Returns:**
java.lang.String - die Zeichenkettenrepräsentation des erweiterten Attributs.
