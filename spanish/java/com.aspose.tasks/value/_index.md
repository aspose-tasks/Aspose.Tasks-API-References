---
title: "Valor"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un valor en una lista de valores."
type: docs
weight: 333
url: /es/java/com.aspose.tasks/value/
---

**Inheritance:**
java.lang.Object
```
public class Value
```

Representa un valor en una lista de valores.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Value()](#Value--) | Inicializa una nueva instancia de la clase [Value](../../com.aspose/tasks/value). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getDateValue()](#getDateValue--) | Obtiene el valor real si puede representarse como DateTime. |
| [getDescription()](#getDescription--) | Obtiene la descripción de un valor. |
| [getDuration()](#getDuration--) | Obtiene el valor real que se usa para representar Duration. |
| [getId()](#getId--) | Obtiene el identificador único de un valor en todo un proyecto. |
| [getNumericValue()](#getNumericValue--) | Obtiene el valor real que se usa para representar un número o valor de costo. |
| [getPhonetic()](#getPhonetic--) | Obtiene la información fonética sobre el nombre del campo personalizado. |
| [getStringValue()](#getStringValue--) | Obtiene el valor real que se usa para representar una cadena de texto. |
| [getVal()](#getVal--) | Obtiene el valor real en representación interna. |
| [getValueGuid()](#getValueGuid--) | Obtiene un GUID que identifica este valor entre otros en todo el proyecto. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | Establece el valor real si puede representarse como DateTime. |
| [setDescription(String value)](#setDescription-java.lang.String-) | Establece la descripción de un valor. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Establece el valor real que se usa para representar Duration. |
| [setId(int value)](#setId-int-) | Establece el identificador único de un valor en todo un proyecto. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Establece el valor real que se usa para representar un número o valor de costo. |
| [setPhonetic(String value)](#setPhonetic-java.lang.String-) | Establece la información fonética sobre el nombre del campo personalizado. |
| [setStringValue(String value)](#setStringValue-java.lang.String-) | Establece el valor real que se usa para representar una cadena de texto. |
| [setVal(String value)](#setVal-java.lang.String-) | Establece el valor real en representación interna. |
### Value() {#Value--}
```
public Value()
```


Inicializa una nueva instancia de la clase [Value](../../com.aspose/tasks/value).

### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


Obtiene el valor real si puede representarse como DateTime. El valor predeterminado es DateTime\#MinValue.MinValue.

--------------------

Prefiera esta propiedad sobre `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), cuando necesite establecer el valor DateTime.

**Returns:**
java.util.Date - el valor real si puede representarse como DateTime.
### getDescription() {#getDescription--}
```
public final String getDescription()
```


Obtiene la descripción de un valor.

**Returns:**
java.lang.String - la descripción de un valor.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Obtiene el valor real que se usa para representar Duration.

--------------------

Prefiera esta propiedad sobre `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), cuando necesite establecer el valor Duration.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the actual value which is used to represent Duration.
### getId() {#getId--}
```
public final int getId()
```


Obtiene el identificador único de un valor en todo un proyecto.

Es importante no tener los mismos identificadores para diferentes instancias de [Value](../../com.aspose.tasks/value).

El valor mínimo de `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) es `1`.

**Returns:**
int - el identificador único de un valor en todo el proyecto.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Obtiene el valor real que se usa para representar un número o valor de costo.

--------------------

Prefiera esta propiedad sobre `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), cuando necesite establecer el valor Number o Cost.

**Returns:**
java.math.BigDecimal - el valor real que se utiliza para representar el valor numérico o de costo.
### getPhonetic() {#getPhonetic--}
```
public final String getPhonetic()
```


Obtiene la información fonética sobre el nombre del campo personalizado.

**Returns:**
java.lang.String - la información fonética sobre el nombre del campo personalizado.
### getStringValue() {#getStringValue--}
```
public final String getStringValue()
```


Obtiene el valor real que se usa para representar una cadena de texto.

--------------------

Prefiera esta propiedad sobre `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), cuando necesite establecer el valor Text.

**Returns:**
java.lang.String - el valor real que se usa para representar la cadena Text.
### getVal() {#getVal--}
```
public final String getVal()
```


Obtiene el valor real en representación interna. Prefiera usar propiedades tipadas fuertemente que se enumeran a continuación.

--------------------

Si desea establecer el valor Text, prefiera usar la propiedad tipada fuertemente `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)).

Si desea establecer el valor Number o Cost, prefiera usar la propiedad tipada fuertemente `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)).

Si desea establecer valores Date/Start/Finish, prefiera usar la propiedad tipada fuertemente `DateValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)).

Si desea establecer el valor Duration, prefiera usar la propiedad tipada fuertemente `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)).

Si su tipo no está listado, use la propiedad `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)).

**Returns:**
java.lang.String - el valor real en representación interna.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


Obtiene un GUID que identifica este valor entre otros en todo el proyecto.

**Returns:**
java.util.UUID - un GUID que identifica este valor entre otros en todo el proyecto.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


Establece el valor real si puede representarse como DateTime. El valor predeterminado es DateTime\#MinValue.MinValue.

--------------------

Prefiera esta propiedad sobre `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), cuando necesite establecer el valor DateTime.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | el valor real si puede representarse como DateTime. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


Establece la descripción de un valor.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | la descripción de un valor. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Establece el valor real que se usa para representar Duration.

--------------------

Prefiera esta propiedad sobre `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), cuando necesite establecer el valor Duration.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | el valor real que se usa para representar Duration. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Establece el identificador único de un valor en todo un proyecto.

Es importante no tener los mismos identificadores para diferentes instancias de [Value](../../com.aspose.tasks/value).

El valor mínimo de `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) es `1`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el identificador único de un valor en todo el proyecto. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Establece el valor real que se usa para representar un número o valor de costo.

--------------------

Prefiera esta propiedad sobre `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), cuando necesite establecer el valor Number o Cost.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.math.BigDecimal | el valor real que se utiliza para representar un número o valor de costo. |

### setPhonetic(String value) {#setPhonetic-java.lang.String-}
```
public final void setPhonetic(String value)
```


Establece la información fonética sobre el nombre del campo personalizado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | la información fonética sobre el nombre del campo personalizado. |

### setStringValue(String value) {#setStringValue-java.lang.String-}
```
public final void setStringValue(String value)
```


Establece el valor real que se usa para representar una cadena de texto.

--------------------

Prefiera esta propiedad sobre `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), cuando necesite establecer el valor Text.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el valor real que se utiliza para representar una cadena de texto. |

### setVal(String value) {#setVal-java.lang.String-}
```
public final void setVal(String value)
```


Establece el valor real en la representación interna. Prefiera usar propiedades fuertemente tipadas que se enumeran a continuación.

--------------------

Si desea establecer el valor Text, prefiera usar la propiedad tipada fuertemente `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)).

Si desea establecer el valor Number o Cost, prefiera usar la propiedad tipada fuertemente `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)).

Si desea establecer valores de Fecha/Inicio/Fin, prefiera usar la propiedad fuertemente tipada `DateTimeValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)).

Si desea establecer el valor Duration, prefiera usar la propiedad tipada fuertemente `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)).

Si su tipo no está listado, use la propiedad `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el valor real en la representación interna. |

