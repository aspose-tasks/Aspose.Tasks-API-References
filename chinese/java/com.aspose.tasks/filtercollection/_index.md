---
title: "FilterCollection"
second_title: "Aspose.Tasks for Java API 参考"
description: "包含一个对象列表。"
type: docs
weight: 92
url: /zh/java/com.aspose.tasks/filtercollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class FilterCollection extends AbstractCollection<Filter>
```

包含一个 [Filter](../../com.aspose.tasks/filter) 对象列表。实现 ICollection&lt;Filter&gt; 接口。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(Filter item)](#add-com.aspose.tasks.Filter-) |  |
| [clear()](#clear--) | 从此集合中移除所有元素（可选操作）。 |
| [contains(Filter item)](#contains-com.aspose.tasks.Filter-) | 如果此集合包含指定的项，则返回 true。 |
| [copyTo(Filter[] array, int arrayIndex)](#copyTo-com.aspose.tasks.Filter---int-) | 从指定数组复制元素到此集合，起始于指定索引。 |
| [iterator()](#iterator--) | 返回此集合中包含的元素的迭代器。 |
| [remove(Filter item)](#remove-com.aspose.tasks.Filter-) | 从此集合中移除指定项。 |
| [size()](#size--) | 获取此集合中包含的元素数量。 |
| [toList()](#toList--) | 将过滤器集合转换为 `Filter` 对象列表。 |
### add(Filter item) {#add-com.aspose.tasks.Filter-}
```
public boolean add(Filter item)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) |  |

**Returns:**
boolean
### clear() {#clear--}
```
public void clear()
```


从此集合中移除所有元素（可选操作）。

### contains(Filter item) {#contains-com.aspose.tasks.Filter-}
```
public final boolean contains(Filter item)
```


如果此集合包含指定的项，则返回 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | 指定的项。 |

**Returns:**
boolean - 如果集合包含指定的项，则为 true。
### copyTo(Filter[] array, int arrayIndex) {#copyTo-com.aspose.tasks.Filter---int-}
```
public final void copyTo(Filter[] array, int arrayIndex)
```


从指定数组复制元素到此集合，起始于指定索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| array | [Filter\[\]](../../com.aspose.tasks/filter) | 要复制元素到的指定一维数组 |
| arrayIndex | int | 指定数组中开始复制的零基索引。 |

### iterator() {#iterator--}
```
public Iterator<Filter> iterator()
```


返回此集合中包含的元素的迭代器。

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Filter&gt; - 集合迭代器。
### remove(Filter item) {#remove-com.aspose.tasks.Filter-}
```
public final boolean remove(Filter item)
```


从此集合中移除指定项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | 指定的项。 |

**Returns:**
boolean - 如果操作成功则为 true。
### size() {#size--}
```
public final int size()
```


获取此集合中包含的元素数量。

**Returns:**
int - 此集合中包含的元素数量。
### toList() {#toList--}
```
public List<Filter> toList()
```


将过滤器集合转换为 `Filter` 对象列表。

**Returns:**
java.util.List&lt;com.aspose.tasks.Filter&gt; - `Filter` 对象的通用列表。
