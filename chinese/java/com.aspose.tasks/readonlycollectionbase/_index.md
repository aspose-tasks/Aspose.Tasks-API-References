---
title: "ReadOnlyCollectionBase"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示只读对象集合。"
type: docs
weight: 238
url: /zh/java/com.aspose.tasks/readonlycollectionbase/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class ReadOnlyCollectionBase<T> extends AbstractList<T>
```

表示只读对象集合。

T：集合项的类型。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(T item)](#add-T-) | 这是 ICollection 的 Add 方法的存根实现，只会抛出 UnsupportedOperationException。 |
| [add(int index, T element)](#add-int-T-) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | 返回指定索引处的元素。 |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | 确定集合是否为只读。 |
| [iterator()](#iterator--) | 返回此集合的枚举器。 |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [set(int index, T value)](#set-int-T-) | 返回指定索引处的元素。 |
| [size()](#size--) | 获取对象中包含的对象数量。 |
| [toList()](#toList--) | 将集合转换为对象列表。 |
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


这是 ICollection 的 Add 方法的存根实现，只会抛出 UnsupportedOperationException。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 项 | T | 要添加的项。 |

**Returns:**
boolean
### add(int index, T element) {#add-int-T-}
```
public final void add(int index, T element)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | \{@inheritDoc\} |
| 元素 | T | \{@inheritDoc\} |

### clear() {#clear--}
```
public final void clear()
```




### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
布尔 - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public final T get(int index)
```


返回指定索引处的元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要获取的元素的零基索引。 |

**Returns:**
T - 指定索引处的元素。
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


确定集合是否为只读。

**Returns:**
boolean - 如果集合只读则为 true；否则为 false。
### iterator() {#iterator--}
```
public final Iterator<T> iterator()
```


返回此集合的枚举器。

**Returns:**
java.util.Iterator<T> - 此集合的枚举器。
### remove(int index) {#remove-int-}
```
public final T remove(int index)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | \{@inheritDoc\} |

**Returns:**
T - {@inheritDoc}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
布尔 - \{@inheritDoc\}
### set(int index, T value) {#set-int-T-}
```
public final T set(int index, T value)
```


返回指定索引处的元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要获取的元素的零基索引。 |
| 值 | T |  |

**Returns:**
T - 指定索引处的元素。
### size() {#size--}
```
public final int size()
```


获取对象中包含的对象数量。

**Returns:**
int - 对象中包含的对象数量。
### toList() {#toList--}
```
public final List<T> toList()
```


将集合转换为对象列表。

**Returns:**
java.util.List<T> - 对象的通用列表。
