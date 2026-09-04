---
title: "OutlineValue"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示大纲值。"
type: docs
weight: 173
url: /zh/java/com.aspose.tasks/outlinevalue/
---

**Inheritance:**
java.lang.Object
```
public class OutlineValue
```

表示大纲值。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [OutlineValue()](#OutlineValue--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getDescription()](#getDescription--) | 获取大纲值的描述。 |
| [getDurationValue()](#getDurationValue--) | 如果类型为 Duration，则获取持续时间。 |
| [getParentValueId()](#getParentValueId--) | 获取大纲代码的父节点 Id。 |
| [getType()](#getType--) | 获取大纲代码类型。 |
| [getValue()](#getValue--) | 获取实际值。 |
| [getValueGuid()](#getValueGuid--) | 获取在整个项目中标识此值的 GUID。 |
| [getValueId()](#getValueId--) | 获取项目中大纲代码值的唯一 Id。 |
| [isCollapsed()](#isCollapsed--) | 获取指示大纲值是否折叠的值。 |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | 设置指示大纲值是否折叠的值。 |
| [setDescription(String value)](#setDescription-java.lang.String-) | 设置大纲值的描述。 |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | 如果类型为 Duration，则设置持续时间。 |
| [setParentValueId(int value)](#setParentValueId-int-) | 设置大纲代码的父节点 Id。 |
| [setType(int value)](#setType-int-) | 设置大纲代码类型。 |
| [setValue(String value)](#setValue-java.lang.String-) | 设置实际值。 |
| [setValueId(int value)](#setValueId-int-) | 设置项目中大纲代码值的唯一 Id。 |
### OutlineValue() {#OutlineValue--}
```
public OutlineValue()
```


### getDescription() {#getDescription--}
```
public final String getDescription()
```


获取大纲值的描述。

**Returns:**
java.lang.String - 大纲值的描述。
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


如果类型为 Duration，则获取持续时间。

--------------------

在需要为 Duration 类型的 OutlineValues 设置值时，优先使用此属性而不是 `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-))。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration if Type is Duration.
### getParentValueId() {#getParentValueId--}
```
public final int getParentValueId()
```


获取大纲代码的父节点 Id。

**Returns:**
int - 大纲代码的父节点 Id。
### getType() {#getType--}
```
public final int getType()
```


获取大纲代码类型。

**Returns:**
int - 大纲代码类型。
### getValue() {#getValue--}
```
public final String getValue()
```


获取实际值。

**Returns:**
java.lang.String - 实际值。
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


获取在整个项目中标识此值的 GUID。

**Returns:**
java.util.UUID - 在整个项目中标识此值的 GUID。
### getValueId() {#getValueId--}
```
public final int getValueId()
```


获取项目中大纲代码值的唯一 Id。

**Returns:**
int - 项目中大纲代码值的唯一 Id。
### isCollapsed() {#isCollapsed--}
```
public final boolean isCollapsed()
```


获取指示大纲值是否折叠的值。

--------------------

这是 MS Project 2010 的新属性。

**Returns:**
boolean - 指示大纲值是否折叠的值。
### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public final void setCollapsed(boolean value)
```


设置指示大纲值是否折叠的值。

--------------------

这是 MS Project 2010 的新属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示大纲值是否折叠的值。 |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


设置大纲值的描述。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 大纲值的描述。 |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


如果类型为 Duration，则设置持续时间。

--------------------

在需要为 Duration 类型的 OutlineValues 设置值时，优先使用此属性而不是 `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-))。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | 如果类型为 Duration，则持续时间。 |

### setParentValueId(int value) {#setParentValueId-int-}
```
public final void setParentValueId(int value)
```


设置大纲代码的父节点 Id。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 大纲代码的父节点 Id。 |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


设置大纲代码类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 大纲代码类型。 |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


设置实际值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 实际值。 |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


设置项目中大纲代码值的唯一 Id。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 项目中大纲代码值的唯一 Id。 |

