---
title: "VbaModule"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un modulo VBA."
type: docs
weight: 334
url: /it/java/com.aspose.tasks/vbamodule/
---

**Inheritance:**
java.lang.Object
```
public final class VbaModule
```

Rappresenta un modulo VBA.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [createClassModule(String name)](#createClassModule-java.lang.String-) | Crea un'istanza di [VbaModule](../../com.aspose/tasks/vbamodule) con tipo VbaModuleType.ClassModule. |
| [createProceduralModule(String name)](#createProceduralModule-java.lang.String-) | Crea un'istanza di [VbaModule](../../com.aspose/tasks/vbamodule) con tipo VbaModuleType.ProceduralModule. |
| [getAttributes()](#getAttributes--) | Ottiene una collezione degli attributi del modulo. |
| [getName()](#getName--) | Ottiene un nome del modulo VBA |
| [getSourceCode()](#getSourceCode--) | Ottiene il codice sorgente del modulo VBA |
| [getType()](#getType--) | Ottiene il tipo del modulo. |
| [setName(String value)](#setName-java.lang.String-) | Un nome del modulo VBA |
| [setSourceCode(String value)](#setSourceCode-java.lang.String-) | Imposta il codice sorgente del modulo VBA |
### createClassModule(String name) {#createClassModule-java.lang.String-}
```
public static VbaModule createClassModule(String name)
```


Crea un'istanza di [VbaModule](../../com.aspose/tasks/vbamodule) con tipo VbaModuleType.ClassModule.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### createProceduralModule(String name) {#createProceduralModule-java.lang.String-}
```
public static VbaModule createProceduralModule(String name)
```


Crea un'istanza di [VbaModule](../../com.aspose/tasks/vbamodule) con tipo VbaModuleType.ProceduralModule.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### getAttributes() {#getAttributes--}
```
public final VbaModuleAttributeCollection getAttributes()
```


Ottiene una collezione degli attributi del modulo.

**Returns:**
[VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection) - a collection of the module's attributes.
### getName() {#getName--}
```
public final String getName()
```


Ottiene un nome del modulo VBA

**Returns:**
java.lang.String - un nome del modulo VBA
### getSourceCode() {#getSourceCode--}
```
public final String getSourceCode()
```


Ottiene il codice sorgente del modulo VBA

**Returns:**
java.lang.String - il codice sorgente del modulo VBA
### getType() {#getType--}
```
public final int getType()
```


Ottiene il tipo del modulo.

**Returns:**
int - il tipo del modulo.
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Un nome del modulo VBA

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un nome del modulo VBA |

### setSourceCode(String value) {#setSourceCode-java.lang.String-}
```
public final void setSourceCode(String value)
```


Imposta il codice sorgente del modulo VBA

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | il codice sorgente del modulo VBA |

