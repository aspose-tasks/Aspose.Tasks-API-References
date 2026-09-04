---
title: "CustomProjectPropertyCollection"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示自定义项目属性的集合。"
type: docs
weight: 61
url: /zh/java/com.aspose.tasks/customprojectpropertycollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection, com.aspose.tasks.PropertyKeyedCollection
```
public final class CustomProjectPropertyCollection extends PropertyKeyedCollection<CustomProjectProperty>
```

表示自定义项目属性的集合。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [CustomProjectPropertyCollection()](#CustomProjectPropertyCollection--) | 初始化一个新的 [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) 类实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | 创建一个新的自定义属性。 |
| [add(String name, double value)](#add-java.lang.String-double-) | 创建一个新的自定义属性。 |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | 创建一个新的自定义属性。 |
| [add(String name, Date value)](#add-java.lang.String-java.util.Date-) | 创建一个新的自定义属性。 |
| [clear()](#clear--) | 清除 PropertyCollection。 |
| [isReadOnly()](#isReadOnly--) | 获取一个值，指示此集合是否为只读；否则为 false。 |
| [remove(String name)](#remove-java.lang.String-) | 从集合中移除具有指定名称的属性。 |
### CustomProjectPropertyCollection() {#CustomProjectPropertyCollection--}
```
public CustomProjectPropertyCollection()
```


初始化一个新的 [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) 类实例。

### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public final CustomProjectProperty add(String name, boolean value)
```


创建一个新的自定义属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | java.lang.String | 属性的名称。 |
| 值 | boolean | 新创建的属性对象值。 |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public final CustomProjectProperty add(String name, double value)
```


创建一个新的自定义属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | java.lang.String | 属性的名称。 |
| 值 | double | 新创建的属性对象值。 |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public final CustomProjectProperty add(String name, String value)
```


创建一个新的自定义属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | java.lang.String | 属性的名称。 |
| 值 | java.lang.String | 新创建的属性对象值。 |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, Date value) {#add-java.lang.String-java.util.Date-}
```
public final CustomProjectProperty add(String name, Date value)
```


创建一个新的自定义属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | java.lang.String | 属性的名称。 |
| 值 | java.util.Date | 新创建的属性对象值。 |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### clear() {#clear--}
```
public final void clear()
```


清除 PropertyCollection。

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


获取一个值，指示此集合是否为只读；否则为 false。

**Returns:**
boolean - 一个值，指示此集合是否为只读；否则为 false。
### remove(String name) {#remove-java.lang.String-}
```
public final boolean remove(String name)
```


从集合中移除具有指定名称的属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | java.lang.String | 属性的不区分大小写的名称。 |

**Returns:**
布尔值 - 如果成功找到并移除元素则为 True；否则为 false。
