---
title: "OutlineValue"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un valor de esquema."
type: docs
weight: 173
url: /es/java/com.aspose.tasks/outlinevalue/
---

**Inheritance:**
java.lang.Object
```
public class OutlineValue
```

Representa un valor de esquema.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [OutlineValue()](#OutlineValue--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [getDescription()](#getDescription--) | Obtiene la descripción de un valor de esquema. |
| [getDurationValue()](#getDurationValue--) | Obtiene la duración si el Tipo es Duración. |
| [getParentValueId()](#getParentValueId--) | Obtiene el Id de un nodo padre de un código de esquema. |
| [getType()](#getType--) | Obtiene el tipo de código de esquema. |
| [getValue()](#getValue--) | Obtiene el valor real. |
| [getValueGuid()](#getValueGuid--) | Obtiene un GUID que identifica este valor entre otros en todo el proyecto. |
| [getValueId()](#getValueId--) | Obtiene el Id único de un valor de código de esquema dentro de un proyecto. |
| [isCollapsed()](#isCollapsed--) | Obtiene un valor que indica si el valor de esquema está colapsado o no. |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | Establece un valor que indica si el valor de esquema está colapsado o no. |
| [setDescription(String value)](#setDescription-java.lang.String-) | Establece la descripción de un valor de esquema. |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | Establece la duración si el Tipo es Duración. |
| [setParentValueId(int value)](#setParentValueId-int-) | Establece el Id de un nodo padre de un código de esquema. |
| [setType(int value)](#setType-int-) | Establece el tipo de código de esquema. |
| [setValue(String value)](#setValue-java.lang.String-) | Establece el valor real. |
| [setValueId(int value)](#setValueId-int-) | Establece el Id único de un valor de código de esquema dentro de un proyecto. |
### OutlineValue() {#OutlineValue--}
```
public OutlineValue()
```


### getDescription() {#getDescription--}
```
public final String getDescription()
```


Obtiene la descripción de un valor de esquema.

**Returns:**
java.lang.String - la descripción de un valor de esquema.
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


Obtiene la duración si el Tipo es Duración.

--------------------

Prefiera esta propiedad sobre `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)), cuando necesite establecer el valor para OutlineValues con tipo Duration.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration if Type is Duration.
### getParentValueId() {#getParentValueId--}
```
public final int getParentValueId()
```


Obtiene el Id de un nodo padre de un código de esquema.

**Returns:**
int - el Id de un nodo padre de un código de esquema.
### getType() {#getType--}
```
public final int getType()
```


Obtiene el tipo de código de esquema.

**Returns:**
int - el tipo de código de esquema.
### getValue() {#getValue--}
```
public final String getValue()
```


Obtiene el valor real.

**Returns:**
java.lang.String - el valor real.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


Obtiene un GUID que identifica este valor entre otros en todo el proyecto.

**Returns:**
java.util.UUID - un GUID que identifica este valor entre otros en todo el proyecto.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


Obtiene el Id único de un valor de código de esquema dentro de un proyecto.

**Returns:**
int - el Id único de un valor de código de esquema dentro de un proyecto.
### isCollapsed() {#isCollapsed--}
```
public final boolean isCollapsed()
```


Obtiene un valor que indica si el valor de esquema está colapsado o no.

--------------------

Esta es una nueva propiedad para MS Project 2010.

**Returns:**
boolean - un valor que indica si el valor de esquema está colapsado o no.
### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public final void setCollapsed(boolean value)
```


Establece un valor que indica si el valor de esquema está colapsado o no.

--------------------

Esta es una nueva propiedad para MS Project 2010.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si el valor de esquema está colapsado o no. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


Establece la descripción de un valor de esquema.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | la descripción de un valor de esquema. |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


Establece la duración si el Tipo es Duración.

--------------------

Prefiera esta propiedad sobre `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)), cuando necesite establecer el valor para OutlineValues con tipo Duration.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | la duración si el Tipo es Duración. |

### setParentValueId(int value) {#setParentValueId-int-}
```
public final void setParentValueId(int value)
```


Establece el Id de un nodo padre de un código de esquema.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el Id de un nodo padre de un código de esquema. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Establece el tipo de código de esquema.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el tipo de código de esquema. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


Establece el valor real.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el valor real. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


Establece el Id único de un valor de código de esquema dentro de un proyecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el Id único de un valor de código de esquema dentro de un proyecto. |

