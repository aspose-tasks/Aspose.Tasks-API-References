---
title: "VbaModule"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en VBA-modul."
type: docs
weight: 334
url: /sv/java/com.aspose.tasks/vbamodule/
---

**Inheritance:**
java.lang.Object
```
public final class VbaModule
```

Representerar en VBA-modul.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [createClassModule(String name)](#createClassModule-java.lang.String-) | Skapar en instans av [VbaModule](../../com.aspose.tasks/vbamodule) med typen VbaModuleType.ClassModule. |
| [createProceduralModule(String name)](#createProceduralModule-java.lang.String-) | Skapar en instans av [VbaModule](../../com.aspose.tasks/vbamodule) med typen VbaModuleType.ProceduralModule. |
| [getAttributes()](#getAttributes--) | Hämtar en samling av modulens attribut. |
| [getName()](#getName--) | Hämtar ett namn på VBA-modulen. |
| [getSourceCode()](#getSourceCode--) | Hämtar källkoden för VBA-modulen. |
| [getType()](#getType--) | Hämtar modulens typ. |
| [setName(String value)](#setName-java.lang.String-) | Ett namn på VBA-modulen. |
| [setSourceCode(String value)](#setSourceCode-java.lang.String-) | Ställer in källkoden för VBA-modulen. |
### createClassModule(String name) {#createClassModule-java.lang.String-}
```
public static VbaModule createClassModule(String name)
```


Skapar en instans av [VbaModule](../../com.aspose.tasks/vbamodule) med typen VbaModuleType.ClassModule.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### createProceduralModule(String name) {#createProceduralModule-java.lang.String-}
```
public static VbaModule createProceduralModule(String name)
```


Skapar en instans av [VbaModule](../../com.aspose.tasks/vbamodule) med typen VbaModuleType.ProceduralModule.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### getAttributes() {#getAttributes--}
```
public final VbaModuleAttributeCollection getAttributes()
```


Hämtar en samling av modulens attribut.

**Returns:**
[VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection) - a collection of the module's attributes.
### getName() {#getName--}
```
public final String getName()
```


Hämtar ett namn på VBA-modulen.

**Returns:**
java.lang.String – ett namn på VBA-modulen.
### getSourceCode() {#getSourceCode--}
```
public final String getSourceCode()
```


Hämtar källkoden för VBA-modulen.

**Returns:**
java.lang.String - en källkod för VBA-modulen
### getType() {#getType--}
```
public final int getType()
```


Hämtar modulens typ.

**Returns:**
int - modulens typ.
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Ett namn på VBA-modulen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett namn på VBA-modulen |

### setSourceCode(String value) {#setSourceCode-java.lang.String-}
```
public final void setSourceCode(String value)
```


Ställer in källkoden för VBA-modulen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | en källkod för VBA-modulen |

