---
title: "ExtendedAttributeDefinitionCollection"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示对象的集合。"
type: docs
weight: 84
url: /zh/java/com.aspose.tasks/extendedattributedefinitioncollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ExtendedAttributeDefinitionCollection extends AbstractList<ExtendedAttributeDefinition>
```

表示一个由 [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) 对象组成的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(ExtendedAttributeDefinition item)](#add-com.aspose.tasks.ExtendedAttributeDefinition-) | 将指定的项添加到此集合中。 |
| [clear()](#clear--) | 从此集合中移除所有项。 |
| [contains(ExtendedAttributeDefinition item)](#contains-com.aspose.tasks.ExtendedAttributeDefinition-) | 如果在此集合中找到指定项，则返回 true；否则返回 false。 |
| [copyTo(ExtendedAttributeDefinition[] array, int arrayIndex)](#copyTo-com.aspose.tasks.ExtendedAttributeDefinition---int-) | 将此集合的元素复制到指定数组中，从指定的数组索引开始。 |
| [get(int index)](#get-int-) | 返回此集合中指定位置的元素。 |
| [getById(int id)](#getById-int-) | 通过 id 返回扩展属性定义 |
| [getParentProject()](#getParentProject--) | 获取 [ExtendedAttributeDefinitionCollection](../../com.aspose.tasks/extendedattributedefinitioncollection) 实例的父项目。 |
| [insert(int index, ExtendedAttributeDefinition item)](#insert-int-com.aspose.tasks.ExtendedAttributeDefinition-) | 在指定索引处插入指定项。 |
| [iterator()](#iterator--) | 返回此集合中元素的迭代器。 |
| [remove(int index)](#remove-int-) | 移除此集合中指定位置的元素，并返回被移除的元素。 |
| [remove(Object item)](#remove-java.lang.Object-) | 从此集合中移除特定对象的第一次出现。 |
| [set(int index, ExtendedAttributeDefinition value)](#set-int-com.aspose.tasks.ExtendedAttributeDefinition-) | 在此集合中设置指定位置的元素。 |
| [size()](#size--) | 获取此集合中包含的元素数量。 |
| [toList()](#toList--) | 将此 ExtendedAttributeDefinitionCollection 对象转换为包含 [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) 类实例的列表。 |
### add(ExtendedAttributeDefinition item) {#add-com.aspose.tasks.ExtendedAttributeDefinition-}
```
public final boolean add(ExtendedAttributeDefinition item)
```


将指定的项添加到此集合中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) | 要添加到此集合的指定项。 |

**Returns:**
布尔值 - 如果成功添加了指定项则为 true；否则为 false。
### clear() {#clear--}
```
public final void clear()
```


从此集合中移除所有项。

### contains(ExtendedAttributeDefinition item) {#contains-com.aspose.tasks.ExtendedAttributeDefinition-}
```
public final boolean contains(ExtendedAttributeDefinition item)
```


如果在此集合中找到指定项，则返回 true；否则返回 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) | 要查找的指定项。 |

**Returns:**
布尔 - 如果在此集合中找到指定项，则为 true；否则为 false。
### copyTo(ExtendedAttributeDefinition[] array, int arrayIndex) {#copyTo-com.aspose.tasks.ExtendedAttributeDefinition---int-}
```
public final void copyTo(ExtendedAttributeDefinition[] array, int arrayIndex)
```


将此集合的元素复制到指定数组中，从指定的数组索引开始。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| array | [ExtendedAttributeDefinition\[\]](../../com.aspose.tasks/extendedattributedefinition) | 要复制元素到的指定一维数组 |
| arrayIndex | int | 指定数组中开始复制的零基索引。 |

### get(int index) {#get-int-}
```
public ExtendedAttributeDefinition get(int index)
```


返回此集合中指定位置的元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 获取内部元素的指定位置。 |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - the element at the specified position in this collection.
### getById(int id) {#getById-int-}
```
public final ExtendedAttributeDefinition getById(int id)
```


通过 id 返回扩展属性定义

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| id | int | 指定的 id |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - ExtendedAttributeDefinition with specified id.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


获取 [ExtendedAttributeDefinitionCollection](../../com.aspose.tasks/extendedattributedefinitioncollection) 实例的父项目。

**Returns:**
[Project](../../com.aspose.tasks/project) - returns a parent project for this collection.
### insert(int index, ExtendedAttributeDefinition item) {#insert-int-com.aspose.tasks.ExtendedAttributeDefinition-}
```
public final void insert(int index, ExtendedAttributeDefinition item)
```


在指定索引处插入指定项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 应插入项的指定零基索引。 |
| item | [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) | 要插入到此集合的指定项。 |

### iterator() {#iterator--}
```
public Iterator<ExtendedAttributeDefinition> iterator()
```


返回此集合中元素的迭代器。

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.ExtendedAttributeDefinition&gt; - 此集合中元素的迭代器。
### remove(int index) {#remove-int-}
```
public final ExtendedAttributeDefinition remove(int index)
```


移除此集合中指定位置的元素，并返回被移除的元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要移除元素的指定位置。 |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - the element that was removed from the collection.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


从此集合中移除特定对象的第一次出现。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 项 | java.lang.Object | 要移除的指定对象。 |

**Returns:**
boolean - 如果成功从此集合中移除指定对象则为 true；否则为 false。
### set(int index, ExtendedAttributeDefinition value) {#set-int-com.aspose.tasks.ExtendedAttributeDefinition-}
```
public final ExtendedAttributeDefinition set(int index, ExtendedAttributeDefinition value)
```


在此集合中设置指定位置的元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要设置元素的指定位置。 |
| value | [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) | 在此集合中指定位置要设置的元素。 |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - `ExtendedAttributeDefinition` value.
### size() {#size--}
```
public final int size()
```


获取此集合中包含的元素数量。

**Returns:**
int - 此集合中包含的元素数量。
### toList() {#toList--}
```
public final List<ExtendedAttributeDefinition> toList()
```


将此 ExtendedAttributeDefinitionCollection 对象转换为包含 [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) 类实例的列表。

**Returns:**
java.util.List&lt;com.aspose.tasks.ExtendedAttributeDefinition&gt; - 包含 [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) 类实例的列表。
