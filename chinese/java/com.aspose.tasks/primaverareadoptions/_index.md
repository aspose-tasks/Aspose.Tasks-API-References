---
title: "PrimaveraReadOptions"
second_title: "Aspose.Tasks for Java API 参考"
description: "允许在读取 Primavera Xml 或 Primavera Xer 文件时指定附加选项。"
type: docs
weight: 206
url: /zh/java/com.aspose.tasks/primaverareadoptions/
---

**Inheritance:**
java.lang.Object
```
public class PrimaveraReadOptions
```

允许在读取 Primavera Xml 或 Primavera Xer 文件时指定附加选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PrimaveraReadOptions()](#PrimaveraReadOptions--) | 初始化一个新的 [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) 类的实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getPreserveUids()](#getPreserveUids--) | 获取一个标志，指定是否应保留实体的原始唯一标识符。 |
| [getProjectUid()](#getProjectUid--) | 获取要从包含多个项目的文件中读取的项目的 UID。 |
| [getReadBaselineProjects()](#getReadBaselineProjects--) | 获取一个标志，指定是否应加载基线项目。 |
| [getUndefinedConstraintHandlingBehavior()](#getUndefinedConstraintHandlingBehavior--) | 指定用于处理从 XER 格式读取的未定义约束任务的行为。 |
| [setPreserveUids(boolean value)](#setPreserveUids-boolean-) | 设置一个标志，指定是否应保留实体的原始唯一标识符。 |
| [setProjectUid(int value)](#setProjectUid-int-) | 设置要从包含多个项目的文件中读取的项目的 UID。 |
| [setReadBaselineProjects(boolean value)](#setReadBaselineProjects-boolean-) | 设置一个标志，指定是否应加载基线项目。 |
| [setUndefinedConstraintHandlingBehavior(int value)](#setUndefinedConstraintHandlingBehavior-int-) | 指定用于处理从 XER 格式读取的未定义约束任务的行为。 |
### PrimaveraReadOptions() {#PrimaveraReadOptions--}
```
public PrimaveraReadOptions()
```


初始化一个新的 [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) 类的实例。

### getPreserveUids() {#getPreserveUids--}
```
public final boolean getPreserveUids()
```


获取一个标志，指定是否应保留实体的原始唯一标识符。

**Returns:**
boolean - 指定是否应保留实体的原始唯一标识符的标志。
### getProjectUid() {#getProjectUid--}
```
public final int getProjectUid()
```


获取要从包含多个项目的文件中读取的项目的 UID。

**Returns:**
int - 要从包含多个项目的文件中读取的项目的 UID。
### getReadBaselineProjects() {#getReadBaselineProjects--}
```
public final boolean getReadBaselineProjects()
```


获取一个标志，指定是否应加载基线项目。默认值为 true。

--------------------

此标志适用于包含基线项目的 Primavera XML 文件（XER 格式不支持基线）。当不需要基线数据时，可以将该选项设置为 false，以加快加载带基线的大型项目的速度。

**Returns:**
boolean - 指定是否应加载基线项目的标志。
### getUndefinedConstraintHandlingBehavior() {#getUndefinedConstraintHandlingBehavior--}
```
public final int getUndefinedConstraintHandlingBehavior()
```


指定用于处理从 XER 格式读取的未定义约束任务的行为。

**Returns:**
int - 用于处理从 XER 格式读取的未定义约束任务的行为。
### setPreserveUids(boolean value) {#setPreserveUids-boolean-}
```
public final void setPreserveUids(boolean value)
```


设置一个标志，指定是否应保留实体的原始唯一标识符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指定是否应保留实体的原始唯一标识符的标志。 |

### setProjectUid(int value) {#setProjectUid-int-}
```
public final void setProjectUid(int value)
```


设置要从包含多个项目的文件中读取的项目的 UID。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 要从包含多个项目的文件中读取的项目的 UID。 |

### setReadBaselineProjects(boolean value) {#setReadBaselineProjects-boolean-}
```
public final void setReadBaselineProjects(boolean value)
```


设置一个标志，指定是否应加载基线项目。默认值为 true。

--------------------

此标志适用于包含基线项目的 Primavera XML 文件（XER 格式不支持基线）。当不需要基线数据时，可以将该选项设置为 false，以加快加载带基线的大型项目的速度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个标志，指定是否应加载基线项目。 |

### setUndefinedConstraintHandlingBehavior(int value) {#setUndefinedConstraintHandlingBehavior-int-}
```
public final void setUndefinedConstraintHandlingBehavior(int value)
```


指定用于处理从 XER 格式读取的未定义约束任务的行为。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 用于处理从 XER 格式读取的未定义约束任务的行为。 |

