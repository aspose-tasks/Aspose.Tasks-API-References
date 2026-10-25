---
title: "VbaModule"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un módulo VBA."
type: docs
weight: 334
url: /es/java/com.aspose.tasks/vbamodule/
---

**Inheritance:**
java.lang.Object
```
public final class VbaModule
```

Representa un módulo VBA.
## Métodos

| Método | Descripción |
| --- | --- |
| [createClassModule(String name)](#createClassModule-java.lang.String-) | Crea una instancia de [VbaModule](../../com.aspose.tasks/vbamodule) con el tipo VbaModuleType.ClassModule. |
| [createProceduralModule(String name)](#createProceduralModule-java.lang.String-) | Crea una instancia de [VbaModule](../../com.aspose.tasks/vbamodule) con el tipo VbaModuleType.ProceduralModule. |
| [getAttributes()](#getAttributes--) | Obtiene una colección de los atributos del módulo. |
| [getName()](#getName--) | Obtiene un nombre del módulo VBA |
| [getSourceCode()](#getSourceCode--) | Obtiene el código fuente del módulo VBA |
| [getType()](#getType--) | Obtiene el tipo del módulo. |
| [setName(String value)](#setName-java.lang.String-) | Un nombre del módulo VBA |
| [setSourceCode(String value)](#setSourceCode-java.lang.String-) | Establece el código fuente del módulo VBA |
### createClassModule(String name) {#createClassModule-java.lang.String-}
```
public static VbaModule createClassModule(String name)
```


Crea una instancia de [VbaModule](../../com.aspose.tasks/vbamodule) con el tipo VbaModuleType.ClassModule.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### createProceduralModule(String name) {#createProceduralModule-java.lang.String-}
```
public static VbaModule createProceduralModule(String name)
```


Crea una instancia de [VbaModule](../../com.aspose.tasks/vbamodule) con el tipo VbaModuleType.ProceduralModule.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### getAttributes() {#getAttributes--}
```
public final VbaModuleAttributeCollection getAttributes()
```


Obtiene una colección de los atributos del módulo.

**Returns:**
[VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection) - a collection of the module's attributes.
### getName() {#getName--}
```
public final String getName()
```


Obtiene un nombre del módulo VBA

**Returns:**
java.lang.String - un nombre del módulo VBA
### getSourceCode() {#getSourceCode--}
```
public final String getSourceCode()
```


Obtiene el código fuente del módulo VBA

**Returns:**
java.lang.String - el código fuente del módulo VBA
### getType() {#getType--}
```
public final int getType()
```


Obtiene el tipo del módulo.

**Returns:**
int - el tipo del módulo.
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Un nombre del módulo VBA

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | un nombre del módulo VBA |

### setSourceCode(String value) {#setSourceCode-java.lang.String-}
```
public final void setSourceCode(String value)
```


Establece el código fuente del módulo VBA

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el código fuente del módulo VBA |

