---
title: VbaModule
second_title: Aspose.Tasks for Java API Reference
description: Represents a VBA module.
type: docs
weight: 333
url: /java/com.aspose.tasks/vbamodule/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.tasks.IVbaModule](../../com.aspose.tasks/ivbamodule)
```
public final class VbaModule implements IVbaModule
```

Represents a VBA module.
## Methods

| Method | Description |
| --- | --- |
| [createClassModule(String name)](#createClassModule-java.lang.String-) | Creates an instance of [VbaModule](../../com.aspose.tasks/vbamodule) with VbaModuleType.ClassModule type. |
| [createProceduralModule(String name)](#createProceduralModule-java.lang.String-) | Creates an instance of [VbaModule](../../com.aspose.tasks/vbamodule) with VbaModuleType.ProceduralModule type. |
| [getAttributes()](#getAttributes--) | Gets a collection of the module's attributes. |
| [getName()](#getName--) | Gets a name of the VBA module |
| [getSourceCode()](#getSourceCode--) | Gets a source code of the VBA module |
| [getType()](#getType--) | Gets the type of the module. |
| [setName(String value)](#setName-java.lang.String-) | A name of the VBA module |
| [setSourceCode(String value)](#setSourceCode-java.lang.String-) | Sets a source code of the VBA module |
### createClassModule(String name) {#createClassModule-java.lang.String-}
```
public static VbaModule createClassModule(String name)
```


Creates an instance of [VbaModule](../../com.aspose.tasks/vbamodule) with VbaModuleType.ClassModule type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### createProceduralModule(String name) {#createProceduralModule-java.lang.String-}
```
public static VbaModule createProceduralModule(String name)
```


Creates an instance of [VbaModule](../../com.aspose.tasks/vbamodule) with VbaModuleType.ProceduralModule type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### getAttributes() {#getAttributes--}
```
public final VbaModuleAttributeCollection getAttributes()
```


Gets a collection of the module's attributes.

**Returns:**
[VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection) - a collection of the module's attributes.
### getName() {#getName--}
```
public final String getName()
```


Gets a name of the VBA module

**Returns:**
java.lang.String - a name of the VBA module
### getSourceCode() {#getSourceCode--}
```
public final String getSourceCode()
```


Gets a source code of the VBA module

**Returns:**
java.lang.String - a source code of the VBA module
### getType() {#getType--}
```
public final int getType()
```


Gets the type of the module.

**Returns:**
int - the type of the module.
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


A name of the VBA module

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a name of the VBA module |

### setSourceCode(String value) {#setSourceCode-java.lang.String-}
```
public final void setSourceCode(String value)
```


Sets a source code of the VBA module

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a source code of the VBA module |

