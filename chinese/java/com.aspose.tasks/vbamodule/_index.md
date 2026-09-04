---
title: "VbaModule"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示一个 VBA 模块。"
type: docs
weight: 334
url: /zh/java/com.aspose.tasks/vbamodule/
---

**Inheritance:**
java.lang.Object
```
public final class VbaModule
```

表示一个 VBA 模块。
## 方法

| 方法 | 描述 |
| --- | --- |
| [createClassModule(String name)](#createClassModule-java.lang.String-) | 创建一个 [VbaModule](../../com.aspose/tasks/vbamodule) 实例，类型为 VbaModuleType.ClassModule。 |
| [createProceduralModule(String name)](#createProceduralModule-java.lang.String-) | 创建一个 [VbaModule](../../com.aspose/tasks/vbamodule) 实例，类型为 VbaModuleType.ProceduralModule。 |
| [getAttributes()](#getAttributes--) | 获取模块属性的集合。 |
| [getName()](#getName--) | 获取 VBA 模块的名称 |
| [getSourceCode()](#getSourceCode--) | 获取 VBA 模块的源代码 |
| [getType()](#getType--) | 获取模块的类型。 |
| [setName(String value)](#setName-java.lang.String-) | VBA 模块的名称 |
| [setSourceCode(String value)](#setSourceCode-java.lang.String-) | 设置 VBA 模块的源代码 |
### createClassModule(String name) {#createClassModule-java.lang.String-}
```
public static VbaModule createClassModule(String name)
```


创建一个 [VbaModule](../../com.aspose/tasks/vbamodule) 实例，类型为 VbaModuleType.ClassModule。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### createProceduralModule(String name) {#createProceduralModule-java.lang.String-}
```
public static VbaModule createProceduralModule(String name)
```


创建一个 [VbaModule](../../com.aspose/tasks/vbamodule) 实例，类型为 VbaModuleType.ProceduralModule。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### getAttributes() {#getAttributes--}
```
public final VbaModuleAttributeCollection getAttributes()
```


获取模块属性的集合。

**Returns:**
[VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection) - a collection of the module's attributes.
### getName() {#getName--}
```
public final String getName()
```


获取 VBA 模块的名称

**Returns:**
java.lang.String - VBA 模块的名称
### getSourceCode() {#getSourceCode--}
```
public final String getSourceCode()
```


获取 VBA 模块的源代码

**Returns:**
java.lang.String - VBA 模块的源代码
### getType() {#getType--}
```
public final int getType()
```


获取模块的类型。

**Returns:**
int - 模块的类型。
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


VBA 模块的名称

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | VBA 模块的名称 |

### setSourceCode(String value) {#setSourceCode-java.lang.String-}
```
public final void setSourceCode(String value)
```


设置 VBA 模块的源代码

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | VBA 模块的源代码 |

