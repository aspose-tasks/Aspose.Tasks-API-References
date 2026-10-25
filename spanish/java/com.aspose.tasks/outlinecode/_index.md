---
title: "OutlineCode"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un valor de un código de esquema."
type: docs
weight: 167
url: /es/java/com.aspose.tasks/outlinecode/
---

**Inheritance:**
java.lang.Object
```
public class OutlineCode
```

Representa un valor de un código de esquema.

--------------------

Se requieren dos datos: un puntero a la tabla de código de esquema especificada por FieldId, y el valor especificado ya sea por ValueId o por el puntero ValueGuid a la lista de valores.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [OutlineCode()](#OutlineCode--) | Inicializa una nueva instancia de la clase [OutlineCode](../../com.aspose.tasks/outlinecode). |
| [OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)](#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-) | Inicializa una nueva instancia de la clase [OutlineCode](../../com.aspose.tasks/outlinecode) usando el Código de esquema especificado y uno de sus valores. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getFieldId()](#getFieldId--) | Obtiene el valor numérico del campo personalizado Id del proyecto. |
| [getValueGuid()](#getValueGuid--) | Obtiene el GUID del valor en la lista de valores. |
| [getValueId()](#getValueId--) | Obtiene el Id en la lista de valores asociado con la definición en la colección de códigos de esquema. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | Establece el valor numérico del campo personalizado Id del proyecto. |
| [setValueGuid(String value)](#setValueGuid-java.lang.String-) | Establece el GUID del valor en la lista de valores. |
| [setValueId(int value)](#setValueId-int-) | Establece el Id en la lista de valores asociado con la definición en la colección de códigos de esquema. |
### OutlineCode() {#OutlineCode--}
```
public OutlineCode()
```


Inicializa una nueva instancia de la clase [OutlineCode](../../com.aspose.tasks/outlinecode).

### OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue) {#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-}
```
public OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)
```


Inicializa una nueva instancia de la clase [OutlineCode](../../com.aspose.tasks/outlinecode) usando el Código de esquema especificado y uno de sus valores.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| codeDefinition | [OutlineCodeDefinition](../../com.aspose.tasks/outlinecodedefinition) | definición de código de esquema. |
| outlineValue | [OutlineValue](../../com.aspose.tasks/outlinevalue) | uno de los valores de definición de código de esquema. |

### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Obtiene el valor numérico del campo personalizado Id del proyecto.

**Returns:**
java.lang.String - el valor numérico del campo personalizado Id del proyecto.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


Obtiene el GUID del valor en la lista de valores. El ValueGuid coincide con el FieldGuid en la lista de valores.

**Returns:**
java.lang.String - el GUID del valor en la lista de valores.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


Obtiene el Id en la lista de valores asociado con la definición en la colección de códigos de esquema.

**Returns:**
int - el Id en la lista de valores asociado con la definición en la colección de código de esquema.
### setFieldId(String value) {#setFieldId-java.lang.String-}
```
public final void setFieldId(String value)
```


Establece el valor numérico del campo personalizado Id del proyecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el valor numérico del campo personalizado Id del proyecto. |

### setValueGuid(String value) {#setValueGuid-java.lang.String-}
```
public final void setValueGuid(String value)
```


Establece el GUID del valor en la lista de valores. El ValueGuid coincide con el FieldGuid en la lista de valores.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el GUID del valor en la lista de valores. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


Establece el Id en la lista de valores asociado con la definición en la colección de códigos de esquema.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el Id en la lista de valores asociado con la definición en la colección de código de esquema. |

