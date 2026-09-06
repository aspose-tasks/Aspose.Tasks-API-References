---
title: "OutlineCodeDefinition"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una definición de código de esquema."
type: docs
weight: 169
url: /es/java/com.aspose.tasks/outlinecodedefinition/
---

**Inheritance:**
java.lang.Object
```
public final class OutlineCodeDefinition
```

Representa una definición de código de esquema.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [OutlineCodeDefinition()](#OutlineCodeDefinition--) | Inicializa una nueva instancia de la clase [OutlineCodeDefinition](../../com.aspose.tasks/outlinecodedefinition). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getAlias()](#getAlias--) | Obtiene el alias de un código de esquema personalizado. |
| [getAllLevelsRequired()](#getAllLevelsRequired--) | Obtiene un valor que indica si los códigos nuevos deben tener todos los niveles. |
| [getEnterprise()](#getEnterprise--) | Obtiene un valor que indica si un código de esquema personalizado es un código de esquema personalizado empresarial. |
| [getEnterpriseOutlineCodeAlias()](#getEnterpriseOutlineCodeAlias--) | Obtiene una referencia a otro campo personalizado para el cual esta definición de código de esquema es un alias. |
| [getFieldId()](#getFieldId--) | Obtiene el número de campo de un código de esquema. |
| [getFieldName()](#getFieldName--) | Obtiene el nombre de un código de esquema personalizado. |
| [getGuid()](#getGuid--) | Obtiene el GUID de un código de esquema. |
| [getLeafOnly()](#getLeafOnly--) | Obtiene un valor que indica si los valores especificados en este campo de código de esquema deben ser valores hoja. |
| [getMasks()](#getMasks--) | Obtiene el objeto OutlineMaskCollection. |
| [getOnlyTableValuesAllowed()](#getOnlyTableValuesAllowed--) | Obtiene un valor que indica si los valores especificados deben provenir de la tabla de valores. |
| [getPhoneticAlias()](#getPhoneticAlias--) | Obtiene la pronunciación fonética del alias del código de esquema personalizado. |
| [getResourceSubstitutionEnabled()](#getResourceSubstitutionEnabled--) | Obtiene un valor que indica si el código de esquema personalizado puede ser usado por el Asistente de Sustitución de Recursos en Microsoft Project. |
| [getShowIndent()](#getShowIndent--) | Obtiene un valor que indica si los sangrados de este código de esquema deben mostrarse. |
| [getValues()](#getValues--) | Obtiene el objeto OutlineValueCollection. |
| [setAlias(String value)](#setAlias-java.lang.String-) | Establece el alias de un código de esquema personalizado. |
| [setAllLevelsRequired(boolean value)](#setAllLevelsRequired-boolean-) | Establece un valor que indica si los códigos nuevos deben tener todos los niveles. |
| [setEnterprise(boolean value)](#setEnterprise-boolean-) | Establece un valor que indica si un código de esquema personalizado es un código de esquema personalizado empresarial. |
| [setEnterpriseOutlineCodeAlias(int value)](#setEnterpriseOutlineCodeAlias-int-) | Establece una referencia a otro campo personalizado para el cual esta definición de código de esquema es un alias. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | Establece el número de campo de un código de esquema. |
| [setFieldName(String value)](#setFieldName-java.lang.String-) | Establece el nombre de un código de esquema personalizado. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Establece el GUID de un código de esquema. |
| [setLeafOnly(boolean value)](#setLeafOnly-boolean-) | Establece un valor que indica si los valores especificados en este campo de código de esquema deben ser valores hoja. |
| [setOnlyTableValuesAllowed(boolean value)](#setOnlyTableValuesAllowed-boolean-) | Establece un valor que indica si los valores especificados deben provenir de la tabla de valores. |
| [setPhoneticAlias(String value)](#setPhoneticAlias-java.lang.String-) | Establece la pronunciación fonética del alias del código de esquema personalizado. |
| [setResourceSubstitutionEnabled(boolean value)](#setResourceSubstitutionEnabled-boolean-) | Establece un valor que indica si el código de esquema personalizado puede ser usado por el Asistente de sustitución de recursos en Microsoft Project. |
| [setShowIndent(boolean value)](#setShowIndent-boolean-) | Establece un valor que indica si los sangrados de este código de esquema deben mostrarse. |
### OutlineCodeDefinition() {#OutlineCodeDefinition--}
```
public OutlineCodeDefinition()
```


Inicializa una nueva instancia de la clase [OutlineCodeDefinition](../../com.aspose.tasks/outlinecodedefinition).

### getAlias() {#getAlias--}
```
public final String getAlias()
```


Obtiene el alias de un código de esquema personalizado.

**Returns:**
java.lang.String - el alias de un código de esquema personalizado.
### getAllLevelsRequired() {#getAllLevelsRequired--}
```
public final boolean getAllLevelsRequired()
```


Obtiene un valor que indica si los códigos nuevos deben tener todos los niveles. No disponible para códigos empresariales.

**Returns:**
boolean - un valor que indica si los códigos nuevos deben tener todos los niveles.
### getEnterprise() {#getEnterprise--}
```
public final boolean getEnterprise()
```


Obtiene un valor que indica si un código de esquema personalizado es un código de esquema personalizado empresarial.

**Returns:**
boolean - un valor que indica si un código de esquema personalizado es un código de esquema personalizado empresarial.
### getEnterpriseOutlineCodeAlias() {#getEnterpriseOutlineCodeAlias--}
```
public final int getEnterpriseOutlineCodeAlias()
```


Obtiene una referencia a otro campo personalizado para el cual esta definición de código de esquema es un alias.

**Returns:**
int - una referencia a otro campo personalizado para el cual esta definición de código de esquema es un alias.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Obtiene el número de campo de un código de esquema.

**Returns:**
java.lang.String - el número de campo de un código de esquema.
### getFieldName() {#getFieldName--}
```
public final String getFieldName()
```


Obtiene el nombre de un código de esquema personalizado.

**Returns:**
java.lang.String - el nombre de un código de esquema personalizado.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Obtiene el GUID de un código de esquema.

**Returns:**
java.lang.String - el GUID de un código de esquema.
### getLeafOnly() {#getLeafOnly--}
```
public final boolean getLeafOnly()
```


Obtiene un valor que indica si los valores especificados en este campo de código de esquema deben ser valores hoja.

**Returns:**
boolean - un valor que indica si los valores especificados en este campo de código de esquema deben ser valores hoja.
### getMasks() {#getMasks--}
```
public final OutlineMaskCollection getMasks()
```


Obtiene el objeto OutlineMaskCollection. La tabla de entradas que define la máscara del código de esquema. Instancia de solo lectura [OutlineMaskCollection](../../com.aspose.tasks/outlinemaskcollection).

**Returns:**
[OutlineMaskCollection](../../com.aspose.tasks/outlinemaskcollection) - the OutlineMaskCollection object.
### getOnlyTableValuesAllowed() {#getOnlyTableValuesAllowed--}
```
public final boolean getOnlyTableValuesAllowed()
```


Obtiene un valor que indica si los valores especificados deben provenir de la tabla de valores.

**Returns:**
boolean - un valor que indica si los valores especificados deben provenir de la tabla de valores.
### getPhoneticAlias() {#getPhoneticAlias--}
```
public final String getPhoneticAlias()
```


Obtiene la pronunciación fonética del alias del código de esquema personalizado.

**Returns:**
java.lang.String - la pronunciación fonética del alias del código de esquema personalizado.
### getResourceSubstitutionEnabled() {#getResourceSubstitutionEnabled--}
```
public final boolean getResourceSubstitutionEnabled()
```


Obtiene un valor que indica si el código de esquema personalizado puede ser usado por el Asistente de Sustitución de Recursos en Microsoft Project.

**Returns:**
boolean - un valor que indica si el código de esquema personalizado puede ser usado por el Asistente de sustitución de recursos en Microsoft Project.
### getShowIndent() {#getShowIndent--}
```
public final boolean getShowIndent()
```


Obtiene un valor que indica si los sangrados de este código de esquema deben mostrarse.

--------------------

Esta es una nueva propiedad para MS Project 2010.

**Returns:**
boolean - un valor que indica si los sangrados de este código de esquema deben mostrarse.
### getValues() {#getValues--}
```
public final OutlineValueCollection getValues()
```


Obtiene el objeto OutlineValueCollection. Los valores de la tabla asociada con este código de esquema.

**Returns:**
[OutlineValueCollection](../../com.aspose.tasks/outlinevaluecollection) - OutlineValueCollection object.
### setAlias(String value) {#setAlias-java.lang.String-}
```
public final void setAlias(String value)
```


Establece el alias de un código de esquema personalizado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el alias de un código de esquema personalizado. |

### setAllLevelsRequired(boolean value) {#setAllLevelsRequired-boolean-}
```
public final void setAllLevelsRequired(boolean value)
```


Establece un valor que indica si los códigos nuevos deben tener todos los niveles. No disponible para códigos empresariales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si los códigos nuevos deben tener todos los niveles. |

### setEnterprise(boolean value) {#setEnterprise-boolean-}
```
public final void setEnterprise(boolean value)
```


Establece un valor que indica si un código de esquema personalizado es un código de esquema personalizado empresarial.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si un código de esquema personalizado es un código de esquema personalizado empresarial. |

### setEnterpriseOutlineCodeAlias(int value) {#setEnterpriseOutlineCodeAlias-int-}
```
public final void setEnterpriseOutlineCodeAlias(int value)
```


Establece una referencia a otro campo personalizado para el cual esta definición de código de esquema es un alias.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | una referencia a otro campo personalizado para el cual esta definición de código de esquema es un alias. |

### setFieldId(String value) {#setFieldId-java.lang.String-}
```
public final void setFieldId(String value)
```


Establece el número de campo de un código de esquema.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el número de campo de un código de esquema. |

### setFieldName(String value) {#setFieldName-java.lang.String-}
```
public final void setFieldName(String value)
```


Establece el nombre de un código de esquema personalizado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el nombre de un código de esquema personalizado. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Establece el GUID de un código de esquema.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el GUID de un código de esquema. |

### setLeafOnly(boolean value) {#setLeafOnly-boolean-}
```
public final void setLeafOnly(boolean value)
```


Establece un valor que indica si los valores especificados en este campo de código de esquema deben ser valores hoja.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si los valores especificados en este campo de código de esquema deben ser valores hoja. |

### setOnlyTableValuesAllowed(boolean value) {#setOnlyTableValuesAllowed-boolean-}
```
public final void setOnlyTableValuesAllowed(boolean value)
```


Establece un valor que indica si los valores especificados deben provenir de la tabla de valores.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si los valores especificados deben provenir de la tabla de valores. |

### setPhoneticAlias(String value) {#setPhoneticAlias-java.lang.String-}
```
public final void setPhoneticAlias(String value)
```


Establece la pronunciación fonética del alias del código de esquema personalizado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | la pronunciación fonética del alias del código de esquema personalizado. |

### setResourceSubstitutionEnabled(boolean value) {#setResourceSubstitutionEnabled-boolean-}
```
public final void setResourceSubstitutionEnabled(boolean value)
```


Establece un valor que indica si el código de esquema personalizado puede ser usado por el Asistente de sustitución de recursos en Microsoft Project.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si el código de esquema personalizado puede ser usado por el Asistente de sustitución de recursos en Microsoft Project. |

### setShowIndent(boolean value) {#setShowIndent-boolean-}
```
public final void setShowIndent(boolean value)
```


Establece un valor que indica si los sangrados de este código de esquema deben mostrarse.

--------------------

Esta es una nueva propiedad para MS Project 2010.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si los sangrados de este código de esquema deben mostrarse. |

