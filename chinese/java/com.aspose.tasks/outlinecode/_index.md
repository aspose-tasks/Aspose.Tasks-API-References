---
title: "OutlineCode"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示大纲代码的值。"
type: docs
weight: 167
url: /zh/java/com.aspose.tasks/outlinecode/
---

**Inheritance:**
java.lang.Object
```
public class OutlineCode
```

表示大纲代码的值。

--------------------

需要两条数据——由 FieldId 指定的纲要代码表指针，以及由 ValueId 或 ValueGuid 指向值列表的值。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [OutlineCode()](#OutlineCode--) | 初始化一个新的 [OutlineCode](../../com.aspose.tasks/outlinecode) 类的实例。 |
| [OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)](#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-) | 使用指定的 Outline Code 及其其中一个值，初始化一个新的 [OutlineCode](../../com.aspose.tasks/outlinecode) 类的实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getFieldId()](#getFieldId--) | 获取项目 Id 自定义字段的数值。 |
| [getValueGuid()](#getValueGuid--) | 获取值列表中值的 GUID。 |
| [getValueId()](#getValueId--) | 获取值列表中与纲要代码集合中的定义关联的 Id。 |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | 设置项目 Id 自定义字段的数值。 |
| [setValueGuid(String value)](#setValueGuid-java.lang.String-) | 设置值列表中值的 GUID。 |
| [setValueId(int value)](#setValueId-int-) | 设置值列表中与纲要代码集合中的定义关联的 Id。 |
### OutlineCode() {#OutlineCode--}
```
public OutlineCode()
```


初始化一个新的 [OutlineCode](../../com.aspose.tasks/outlinecode) 类的实例。

### OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue) {#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-}
```
public OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)
```


使用指定的 Outline Code 及其其中一个值，初始化一个新的 [OutlineCode](../../com.aspose.tasks/outlinecode) 类的实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| codeDefinition | [OutlineCodeDefinition](../../com.aspose.tasks/outlinecodedefinition) | 纲要代码定义。 |
| outlineValue | [OutlineValue](../../com.aspose.tasks/outlinevalue) | 纲要代码定义值之一。 |

### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


获取项目 Id 自定义字段的数值。

**Returns:**
java.lang.String - 项目 Id 自定义字段的数值。
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


获取值列表中值的 GUID。ValueGuid 与值列表中的 FieldGuid 相匹配。

**Returns:**
java.lang.String - 值列表中值的 GUID。
### getValueId() {#getValueId--}
```
public final int getValueId()
```


获取值列表中与纲要代码集合中的定义关联的 Id。

**Returns:**
int - 与纲要代码集合中的定义关联的值列表中的 Id。
### setFieldId(String value) {#setFieldId-java.lang.String-}
```
public final void setFieldId(String value)
```


设置项目 Id 自定义字段的数值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 项目 Id 自定义字段的数值。 |

### setValueGuid(String value) {#setValueGuid-java.lang.String-}
```
public final void setValueGuid(String value)
```


设置值列表中值的 GUID。ValueGuid 与值列表中的 FieldGuid 相匹配。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 值列表中值的 GUID。 |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


设置值列表中与纲要代码集合中的定义关联的 Id。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 在大纲代码集合中与定义关联的值列表中的 Id。 |

