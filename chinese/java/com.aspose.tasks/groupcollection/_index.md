---
title: "GroupCollection"
second_title: "Aspose.Tasks for Java API 参考"
description: "包含一个对象列表。"
type: docs
weight: 123
url: /zh/java/com.aspose.tasks/groupcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class GroupCollection extends AbstractCollection<Group>
```

包含一系列 [Group](../../com.aspose.tasks/group) 对象。实现了 ICollection&lt;Group&gt; 接口。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(Group item)](#add-com.aspose.tasks.Group-) |  |
| [clear()](#clear--) |  |
| [contains(Group item)](#contains-com.aspose.tasks.Group-) | 如果此集合包含指定的项，则返回 true。 |
| [copyTo(Group[] array, int arrayIndex)](#copyTo-com.aspose.tasks.Group---int-) | 将此集合的元素复制到指定数组中，从指定的数组索引开始。 |
| [isReadOnly()](#isReadOnly--) | 获取一个值，指示此集合是否为只读。 |
| [iterator()](#iterator--) |  |
| [remove(Group item)](#remove-com.aspose.tasks.Group-) | 从此集合中移除特定对象的第一次出现。 |
| [size()](#size--) | 获取此集合中包含的元素数量。 |
| [toList()](#toList--) | 将组集合转换为 [Group](../../com.aspose.tasks/group) 对象的列表。 |
### add(Group item) {#add-com.aspose.tasks.Group-}
```
public final boolean add(Group item)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [Group](../../com.aspose.tasks/group) |  |

**Returns:**
boolean
### clear() {#clear--}
```
public final void clear()
```




### contains(Group item) {#contains-com.aspose.tasks.Group-}
```
public final boolean contains(Group item)
```


如果此集合包含指定的项，则返回 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [Group](../../com.aspose.tasks/group) | 指定的项。 |

**Returns:**
boolean - 如果集合包含指定的项，则为 true。
### copyTo(Group[] array, int arrayIndex) {#copyTo-com.aspose.tasks.Group---int-}
```
public final void copyTo(Group[] array, int arrayIndex)
```


将此集合的元素复制到指定数组中，从指定的数组索引开始。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| array | [Group\[\]](../../com.aspose.tasks/group) | 要复制元素到的指定一维数组 |
| arrayIndex | int | 指定数组中开始复制的零基索引。 |

### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


获取一个值，指示此集合是否为只读。

**Returns:**
boolean - 表示此集合是否为只读的值。
### iterator() {#iterator--}
```
public Iterator<Group> iterator()
```




**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Group&gt;
### remove(Group item) {#remove-com.aspose.tasks.Group-}
```
public final boolean remove(Group item)
```


从此集合中移除特定对象的第一次出现。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [Group](../../com.aspose.tasks/group) | 要移除的指定对象。 |

**Returns:**
boolean - 如果成功从此集合中移除指定对象则为 true；否则为 false。
### size() {#size--}
```
public final int size()
```


获取此集合中包含的元素数量。

**Returns:**
int - 此集合中包含的元素数量。
### toList() {#toList--}
```
public final List<Group> toList()
```


将组集合转换为 [Group](../../com.aspose.tasks/group) 对象的列表。

**Returns:**
java.util.List&lt;com.aspose.tasks.Group&gt; - [Group](../../com.aspose.tasks/group) 对象的通用列表。
