---
title: "ExtendedAttribute"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta gli attributi estesi."
type: docs
weight: 81
url: /it/java/com.aspose.tasks/extendedattribute/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttribute
```

Rappresenta gli attributi estesi.

--------------------

Attualmente supportati tutti i tipi di attributi estesi letti da MSP Xml 2003/2007 e mpp 2003. Per MSP mpp 2007 tutti gli attributi estesi sono supportati, eccetto durate e flag.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getAttributeDefinition()](#getAttributeDefinition--) | Ottiene la definizione dell'attributo. |
| [getDateValue()](#getDateValue--) | Ottiene un valore per gli attributi di tipo data (Date, Start, Finish). |
| [getDurationValue()](#getDurationValue--) | Ottiene il valore per gli attributi di tipo 'Duration'. |
| [getFieldId()](#getFieldId--) | Ottiene l'id di un campo. |
| [getFlagValue()](#getFlagValue--) | Ottiene un valore che indica se un flag è impostato per un attributo di tipo 'Flag'. |
| [getNumericValue()](#getNumericValue--) | Ottiene un valore per gli attributi di tipo numerico (Cost, Number). |
| [getTextValue()](#getTextValue--) | Ottiene un valore per gli attributi di tipo 'Text'. |
| [getValueGuid()](#getValueGuid--) | Ottiene il guid di un valore di ricerca. |
| [getValueReadOnly()](#getValueReadOnly--) | Ottiene un valore che indica se il valore di questa istanza di [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) è di sola lettura. |
| [isErrorValue()](#isErrorValue--) | Ottiene se il calcolo del valore dell'attributo esteso ha generato un errore. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | Imposta un valore per gli attributi di tipo data (Date, Start, Finish). |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | Imposta il valore per gli attributi di tipo 'Duration'. |
| [setFlagValue(boolean value)](#setFlagValue-boolean-) | Imposta un valore che indica se un flag è impostato per un attributo di tipo 'Flag'. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Imposta un valore per gli attributi di tipo numerico (Cost, Number). |
| [setTextValue(String value)](#setTextValue-java.lang.String-) | Imposta un valore per gli attributi di tipo 'Text'. |
| [toString()](#toString--) | Restituisce la rappresentazione stringa breve di un attributo esteso. |
### getAttributeDefinition() {#getAttributeDefinition--}
```
public final ExtendedAttributeDefinition getAttributeDefinition()
```


Ottiene la definizione dell'attributo.

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - the attribute definition.
### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


Ottiene un valore per gli attributi di tipo data (Date, Start, Finish).

**Returns:**
java.util.Date - un valore per gli attributi di tipo data (Date, Start, Finish).
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


Ottiene il valore per gli attributi di tipo 'Duration'.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - value for attributes with 'Duration' type.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Ottiene l'id di un campo.

**Returns:**
java.lang.String - l'id di un campo.
### getFlagValue() {#getFlagValue--}
```
public final boolean getFlagValue()
```


Ottiene un valore che indica se un flag è impostato per un attributo di tipo 'Flag'.

**Returns:**
boolean - un valore che indica se un flag è impostato per un attributo di tipo 'Flag'.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Ottiene un valore per gli attributi di tipo numerico (Cost, Number).

**Returns:**
java.math.BigDecimal - un valore per gli attributi di tipo numerico (Cost, Number).
### getTextValue() {#getTextValue--}
```
public final String getTextValue()
```


Ottiene un valore per gli attributi di tipo 'Text'.

**Returns:**
java.lang.String - un valore per gli attributi di tipo 'Text'.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


Ottiene il guid di un valore di ricerca.

--------------------

Non dovrebbe essere impostato direttamente, invece utilizzare ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) per creare un attributo esteso con un valore di ricerca.

**Returns:**
java.lang.String - il guid di un valore di ricerca.
### getValueReadOnly() {#getValueReadOnly--}
```
public final boolean getValueReadOnly()
```


Ottiene un valore che indica se il valore di questa istanza di [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) è di sola lettura.

Value: restituisce true se una formula o un rollup è definito nella [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) per questo oggetto.

**Returns:**
boolean - un valore che indica se il valore di questa istanza di [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) è di sola lettura.
### isErrorValue() {#isErrorValue--}
```
public final boolean isErrorValue()
```


Ottiene se il calcolo del valore dell'attributo esteso ha generato un errore.

**Returns:**
boolean - se il calcolo del valore dell'attributo esteso ha generato un errore.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


Imposta un valore per gli attributi di tipo data (Date, Start, Finish).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | un valore per gli attributi di tipo data (Date, Start, Finish). |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


Imposta il valore per gli attributi di tipo 'Duration'.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | valore per gli attributi di tipo 'Duration'. |

### setFlagValue(boolean value) {#setFlagValue-boolean-}
```
public final void setFlagValue(boolean value)
```


Imposta un valore che indica se un flag è impostato per un attributo di tipo 'Flag'.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se un flag è impostato per un attributo di tipo 'Flag'. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Imposta un valore per gli attributi di tipo numerico (Cost, Number).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | un valore per gli attributi di tipo numerico (Cost, Number). |

### setTextValue(String value) {#setTextValue-java.lang.String-}
```
public final void setTextValue(String value)
```


Imposta un valore per gli attributi di tipo 'Text'.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un valore per gli attributi di tipo 'Text'. |

### toString() {#toString--}
```
public String toString()
```


Restituisce la rappresentazione stringa breve di un attributo esteso.

**Returns:**
java.lang.String - La rappresentazione stringa dell'attributo esteso.
