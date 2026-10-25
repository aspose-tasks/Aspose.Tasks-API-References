---
title: "TimephasedDataCollection"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示对象的集合。"
type: docs
weight: 321
url: /zh/java/com.aspose.tasks/timephaseddatacollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class TimephasedDataCollection extends AbstractList<TimephasedData>
```

表示一个由 [TimephasedData](../../com.aspose.tasks/timephaseddata) 对象组成的集合。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [TimephasedDataCollection()](#TimephasedDataCollection--) | 初始化 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(TimephasedData item)](#add-com.aspose.tasks.TimephasedData-) | 向此集合对象添加 [TimephasedData](../../com.aspose.tasks/timephaseddata) 实例。 |
| [addRange(Iterable&lt;TimephasedData&gt; timephasedCollection)](#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--) | 向此集合对象添加一组 [TimephasedData](../../com.aspose.tasks/timephaseddata) 实例。 |
| [clear()](#clear--) | 从 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 中移除所有项。 |
| [containsItem(TimephasedData item)](#containsItem-com.aspose.tasks.TimephasedData-) | 确定 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 是否包含特定值。 |
| [copyToTArray(TimephasedData[] array, int arrayIndex)](#copyToTArray-com.aspose.tasks.TimephasedData---int-) | 将 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 的元素复制到数组中，从特定的数组索引开始。 |
| [get(int index)](#get-int-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | 获取一个值，指示 System.Collections.Generic.ICollection&lt;T&gt; 是否为只读。 |
| [iterator()](#iterator--) | 返回此集合的迭代器。 |
| [remove(TimephasedData item)](#remove-com.aspose.tasks.TimephasedData-) | 从此集合对象中移除 [TimephasedData](../../com.aspose.tasks/timephaseddata) 实例。 |
| [selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)](#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-) | 选择 `startTime` 与 `finishTime` 之间的所有时间阶段。 |
| [set_Item(int index, TimephasedData value)](#set-Item-int-com.aspose.tasks.TimephasedData-) | 设置指定索引处的元素。 |
| [size()](#size--) | 获取此 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 对象中包含的对象数量。 |
| [toList()](#toList--) | 将 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 对象转换为 [TimephasedData](../../com.aspose.tasks/timephaseddata) 对象的列表。 |
### TimephasedDataCollection() {#TimephasedDataCollection--}
```
public TimephasedDataCollection()
```


初始化 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 类的新实例。

### add(TimephasedData item) {#add-com.aspose.tasks.TimephasedData-}
```
public final boolean add(TimephasedData item)
```


向此集合对象添加 [TimephasedData](../../com.aspose.tasks/timephaseddata) 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | 要添加的项。 |

**Returns:**
boolean - 如果已添加项则为 true；否则为 false。
### addRange(Iterable&lt;TimephasedData&gt; timephasedCollection) {#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--}
```
public final void addRange(Iterable<TimephasedData> timephasedCollection)
```


向此集合对象添加一组 [TimephasedData](../../com.aspose.tasks/timephaseddata) 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| timephasedCollection | java.lang.Iterable&lt;com.aspose.tasks.TimephasedData&gt; | 要添加的 [TimephasedData](../../com.aspose.tasks/timephaseddata) 对象集合。 |

### clear() {#clear--}
```
public final void clear()
```


从 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 中移除所有项。

### containsItem(TimephasedData item) {#containsItem-com.aspose.tasks.TimephasedData-}
```
public final boolean containsItem(TimephasedData item)
```


确定 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 是否包含特定值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | 要在集合中定位的对象。 |

**Returns:**
boolean - 如果在集合中找到 `item` 则为 true；否则为 false。
### copyToTArray(TimephasedData[] array, int arrayIndex) {#copyToTArray-com.aspose.tasks.TimephasedData---int-}
```
public final void copyToTArray(TimephasedData[] array, int arrayIndex)
```


将 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 的元素复制到数组中，从特定的数组索引开始。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| array | [TimephasedData\[\]](../../com.aspose.tasks/timephaseddata) | 从 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 复制的元素的目标一维数组。该数组必须使用零基索引。 |
| arrayIndex | int | `array` 中开始复制的零基索引。 |

### get(int index) {#get-int-}
```
public TimephasedData get(int index)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | \{@inheritDoc\} |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


获取一个值，指示 System.Collections.Generic.ICollection&lt;T&gt; 是否为只读。

**Returns:**
boolean - 如果 System.Collections.Generic.ICollection&lt;T&gt; 为只读则为 true；否则为 false。
### iterator() {#iterator--}
```
public final Iterator<TimephasedData> iterator()
```


返回此集合的迭代器。

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.TimephasedData&gt; - 此集合的迭代器。
### remove(TimephasedData item) {#remove-com.aspose.tasks.TimephasedData-}
```
public final boolean remove(TimephasedData item)
```


从此集合对象中移除 [TimephasedData](../../com.aspose.tasks/timephaseddata) 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | 要删除的项目。 |

**Returns:**
boolean - 如果 `item` 已成功从 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 中移除则为 true；否则为 false。如果在 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 中未找到 `item`，此方法也返回 false。
### selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime) {#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-}
```
public final List<TimephasedData> selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)
```


选择 `startTime` 与 `finishTime` 之间的所有时间阶段。平均情况下具有 O(log n) 的复杂度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| timephasedDataType | 字节 | 要选择的时间阶段类型。 |
| startTime | java.util.Date | 区间的开始。 |
| finishTime | java.util.Date | 区间的结束。 |

**Returns:**
java.util.List&lt;com.aspose.tasks.TimephasedData&gt; - 返回新的列表实例，包含按 Start 属性排序的 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 数据。
### set_Item(int index, TimephasedData value) {#set-Item-int-com.aspose.tasks.TimephasedData-}
```
public final void set_Item(int index, TimephasedData value)
```


设置指定索引处的元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要设置的元素的零基索引。 |
| value | [TimephasedData](../../com.aspose.tasks/timephaseddata) | 要设置的元素。 |

### size() {#size--}
```
public final int size()
```


获取此 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 对象中包含的对象数量。

**Returns:**
int - 此 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 对象中包含的对象数量。
### toList() {#toList--}
```
public final List<TimephasedData> toList()
```


将 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 对象转换为 [TimephasedData](../../com.aspose.tasks/timephaseddata) 对象的列表。

**Returns:**
java.util.List&lt;com.aspose.tasks.TimephasedData&gt; - [TimephasedData](../../com.aspose.tasks/timephaseddata) 对象的列表。
