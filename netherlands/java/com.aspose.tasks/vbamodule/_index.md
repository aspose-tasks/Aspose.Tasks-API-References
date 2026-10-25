---
title: "VbaModule"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een VBA-module voor."
type: docs
weight: 334
url: /nl/java/com.aspose.tasks/vbamodule/
---

**Inheritance:**
java.lang.Object
```
public final class VbaModule
```

Stelt een VBA-module voor.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [createClassModule(String name)](#createClassModule-java.lang.String-) | Maakt een instantie van [VbaModule](../../com.aspose/tasks/vbamodule) met type VbaModuleType.ClassModule. |
| [createProceduralModule(String name)](#createProceduralModule-java.lang.String-) | Maakt een instantie van [VbaModule](../../com.aspose/tasks/vbamodule) met type VbaModuleType.ProceduralModule. |
| [getAttributes()](#getAttributes--) | Haalt een verzameling van de attributen van de module op. |
| [getName()](#getName--) | Haalt een naam van de VBA-module op |
| [getSourceCode()](#getSourceCode--) | Haalt de broncode van de VBA-module op |
| [getType()](#getType--) | Haalt het type van de module op. |
| [setName(String value)](#setName-java.lang.String-) | Een naam van de VBA-module |
| [setSourceCode(String value)](#setSourceCode-java.lang.String-) | Stelt de broncode van de VBA-module in |
### createClassModule(String name) {#createClassModule-java.lang.String-}
```
public static VbaModule createClassModule(String name)
```


Maakt een instantie van [VbaModule](../../com.aspose/tasks/vbamodule) met type VbaModuleType.ClassModule.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### createProceduralModule(String name) {#createProceduralModule-java.lang.String-}
```
public static VbaModule createProceduralModule(String name)
```


Maakt een instantie van [VbaModule](../../com.aspose/tasks/vbamodule) met type VbaModuleType.ProceduralModule.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### getAttributes() {#getAttributes--}
```
public final VbaModuleAttributeCollection getAttributes()
```


Haalt een verzameling van de attributen van de module op.

**Returns:**
[VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection) - a collection of the module's attributes.
### getName() {#getName--}
```
public final String getName()
```


Haalt een naam van de VBA-module op

**Returns:**
java.lang.String - een naam van de VBA-module
### getSourceCode() {#getSourceCode--}
```
public final String getSourceCode()
```


Haalt de broncode van de VBA-module op

**Returns:**
java.lang.String - een broncode van de VBA-module
### getType() {#getType--}
```
public final int getType()
```


Haalt het type van de module op.

**Returns:**
int - het type van de module.
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Een naam van de VBA-module

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een naam van de VBA-module |

### setSourceCode(String value) {#setSourceCode-java.lang.String-}
```
public final void setSourceCode(String value)
```


Stelt de broncode van de VBA-module in

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een broncode van de VBA-module |

