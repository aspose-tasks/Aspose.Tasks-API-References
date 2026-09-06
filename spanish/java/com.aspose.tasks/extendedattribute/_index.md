---
title: "ExtendedAttribute"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa atributos extendidos."
type: docs
weight: 81
url: /es/java/com.aspose.tasks/extendedattribute/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttribute
```

Representa atributos extendidos.

--------------------

Actualmente se admiten todos los tipos de atributos extendidos leídos desde MSP Xml 2003/2007 y mpp 2003. Para MSP mpp 2007 se admiten todos los atributos extendidos excepto duraciones y banderas.
## Métodos

| Método | Descripción |
| --- | --- |
| [getAttributeDefinition()](#getAttributeDefinition--) | Obtiene la definición del atributo. |
| [getDateValue()](#getDateValue--) | Obtiene un valor para atributos con tipos de fecha (Date, Start, Finish). |
| [getDurationValue()](#getDurationValue--) | Obtiene el valor para atributos con tipo 'Duration'. |
| [getFieldId()](#getFieldId--) | Obtiene el id de un campo. |
| [getFlagValue()](#getFlagValue--) | Obtiene un valor que indica si una bandera está establecida para un atributo con tipo 'Flag'. |
| [getNumericValue()](#getNumericValue--) | Obtiene un valor para atributos con tipos numéricos (Cost, Number). |
| [getTextValue()](#getTextValue--) | Obtiene un valor para atributos con tipo 'Text'. |
| [getValueGuid()](#getValueGuid--) | Obtiene el guid de un valor de búsqueda. |
| [getValueReadOnly()](#getValueReadOnly--) | Obtiene un valor que indica si el valor de esta instancia de [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) es de solo lectura. |
| [isErrorValue()](#isErrorValue--) | Obtiene si el cálculo del valor del atributo extendido resultó en un error. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | Establece un valor para atributos con tipos de fecha (Date, Start, Finish). |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | Establece el valor para atributos con tipo 'Duration'. |
| [setFlagValue(boolean value)](#setFlagValue-boolean-) | Establece un valor que indica si una bandera está establecida para un atributo con tipo 'Flag'. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Establece un valor para atributos con tipos numéricos (Cost, Number). |
| [setTextValue(String value)](#setTextValue-java.lang.String-) | Establece un valor para atributos con tipo 'Text'. |
| [toString()](#toString--) | Devuelve la representación corta en cadena de un atributo extendido. |
### getAttributeDefinition() {#getAttributeDefinition--}
```
public final ExtendedAttributeDefinition getAttributeDefinition()
```


Obtiene la definición del atributo.

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - the attribute definition.
### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


Obtiene un valor para atributos con tipos de fecha (Date, Start, Finish).

**Returns:**
java.util.Date - un valor para atributos con tipos de fecha (Date, Start, Finish).
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


Obtiene el valor para atributos con tipo 'Duration'.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - value for attributes with 'Duration' type.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Obtiene el id de un campo.

**Returns:**
java.lang.String - el id de un campo.
### getFlagValue() {#getFlagValue--}
```
public final boolean getFlagValue()
```


Obtiene un valor que indica si una bandera está establecida para un atributo con tipo 'Flag'.

**Returns:**
boolean - un valor que indica si una bandera está establecida para un atributo con tipo 'Flag'.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Obtiene un valor para atributos con tipos numéricos (Cost, Number).

**Returns:**
java.math.BigDecimal - un valor para atributos con tipos numéricos (Cost, Number).
### getTextValue() {#getTextValue--}
```
public final String getTextValue()
```


Obtiene un valor para atributos con tipo 'Text'.

**Returns:**
java.lang.String - un valor para atributos con tipo 'Text'.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


Obtiene el guid de un valor de búsqueda.

--------------------

No debe establecerse directamente; en su lugar, use ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) para crear un atributo extendido con un valor de búsqueda.

**Returns:**
java.lang.String - el guid de un valor de búsqueda.
### getValueReadOnly() {#getValueReadOnly--}
```
public final boolean getValueReadOnly()
```


Obtiene un valor que indica si el valor de esta instancia de [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) es de solo lectura.

Valor: devuelve true si una fórmula o consolidación está definida en la [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) para este objeto.

**Returns:**
boolean - un valor que indica si el valor de esta instancia de [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) es de solo lectura.
### isErrorValue() {#isErrorValue--}
```
public final boolean isErrorValue()
```


Obtiene si el cálculo del valor del atributo extendido resultó en un error.

**Returns:**
boolean - si el cálculo del valor del atributo extendido resultó en un error.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


Establece un valor para atributos con tipos de fecha (Date, Start, Finish).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | un valor para atributos con tipos de fecha (Date, Start, Finish). |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


Establece el valor para atributos con tipo 'Duration'.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | valor para atributos con tipo 'Duration'. |

### setFlagValue(boolean value) {#setFlagValue-boolean-}
```
public final void setFlagValue(boolean value)
```


Establece un valor que indica si una bandera está establecida para un atributo con tipo 'Flag'.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si una bandera está establecida para un atributo con tipo 'Flag'. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Establece un valor para atributos con tipos numéricos (Cost, Number).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.math.BigDecimal | un valor para atributos con tipos numéricos (Cost, Number). |

### setTextValue(String value) {#setTextValue-java.lang.String-}
```
public final void setTextValue(String value)
```


Establece un valor para atributos con tipo 'Text'.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un valor para atributos con tipo 'Text'. |

### toString() {#toString--}
```
public String toString()
```


Devuelve la representación corta en cadena de un atributo extendido.

**Returns:**
java.lang.String - La representación en cadena del atributo extendido.
