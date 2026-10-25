---
title: "OutlineValueCollection"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示对象的集合。"
type: docs
weight: 174
url: /zh/java/com.aspose.tasks/outlinevaluecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class OutlineValueCollection extends AbstractList<OutlineValue>
```

表示一组 [OutlineValue](../../com.aspose.tasks/outlinevalue) 对象的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(OutlineValue item)](#add-com.aspose.tasks.OutlineValue-) | 将指定的项添加到此集合中。 |
| [get(int index)](#get-int-) | 返回此集合中指定位置的元素。 |
| [iterator()](#iterator--) | 返回此集合中元素的迭代器。 |
| [remove(int index)](#remove-int-) | 移除此集合中指定位置的元素，并返回被移除的元素。 |
| [size()](#size--) | 获取此集合中包含的元素数量。 |
### add(OutlineValue item) {#add-com.aspose.tasks.OutlineValue-}
```
public final boolean add(OutlineValue item)
```


将指定的项添加到此集合中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [OutlineValue](../../com.aspose.tasks/outlinevalue) | 要添加到此集合的指定项。 |

**Returns:**
布尔值 - 如果成功添加了指定项则为 true；否则为 false。
### get(int index) {#get-int-}
```
public final OutlineValue get(int index)
```


返回此集合中指定位置的元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 获取内部元素的指定位置。 |

**Returns:**
[OutlineValue](../../com.aspose.tasks/outlinevalue) - the element at the specified position in this collection.
### iterator() {#iterator--}
```
public Iterator<OutlineValue> iterator()
```


返回此集合中元素的迭代器。

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.OutlineValue&gt; - 此集合中元素的迭代器。
### remove(int index) {#remove-int-}
```
public final OutlineValue remove(int index)
```


移除此集合中指定位置的元素，并返回被移除的元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要移除元素的指定位置。 |

**Returns:**
[OutlineValue](../../com.aspose.tasks/outlinevalue) - the element that was removed from the collection.
### size() {#size--}
```
public final int size()
```


获取此集合中包含的元素数量。

**Returns:**
int - 此集合中包含的元素数量。
