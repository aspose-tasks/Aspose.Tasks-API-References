---
title: "RateCollection"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示一个包含对象的集合。"
type: docs
weight: 234
url: /zh/java/com.aspose.tasks/ratecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractMap

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RateCollection extends AbstractMap<Integer,RateByDateCollection> implements Iterable<Map.Entry<Integer,RateByDateCollection>>
```

表示一个包含 [Rate](../../com.aspose.tasks/rate) 对象的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(Date ratesFrom)](#add-java.util.Date-) | 向此集合添加一个新的 [Rate](../../com.aspose.tasks/rate) 实例。 |
| [add(Date ratesFrom, int type)](#add-java.util.Date-int-) | 向此集合添加一个新的 [Rate](../../com.aspose.tasks/rate) 实例。 |
| [clear()](#clear--) | \{@inheritDoc\} |
| [entrySet()](#entrySet--) | (@inheritDoc\} |
| [get(Object key)](#get-java.lang.Object-) | (@inheritDoc\} |
| [getByRateType(int key)](#getByRateType-int-) | 返回指定索引处的元素。 |
| [getParentResource()](#getParentResource--) | 获取此集合的父级 [Resource](../../com.aspose.tasks/resource) 对象。 |
| [isReadOnly()](#isReadOnly--) | 获取指示此集合是否只读的值。 |
| [iterator()](#iterator--) | 返回此集合的枚举器。 |
| [put(Integer key, RateByDateCollection value)](#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-) | (@inheritDoc\} |
| [remove(Rate item)](#remove-com.aspose.tasks.Rate-) | 从此集合中移除 Rate 实例。 |
| [setByRateType(int key, RateByDateCollection value)](#setByRateType-int-com.aspose.tasks.RateByDateCollection-) | 设置指定索引处的元素。 |
| [size()](#size--) | 获取 RateCollection 中包含的元素数量。 |
| [toList()](#toList--) | 将 [RateCollection](../../com.aspose.tasks/ratecollection) 对象转换为 [Rate](../../com.aspose.tasks/rate) 对象的列表。 |
| [toList(int type)](#toList-int-) | 将 [RateCollection](../../com.aspose.tasks/ratecollection) 对象转换为按指定 [RateType](../../com.aspose.tasks/ratetype) 类型过滤的 [Rate](../../com.aspose.tasks/rate) 对象列表。 |
### add(Date ratesFrom) {#add-java.util.Date-}
```
public final Rate add(Date ratesFrom)
```


向此集合添加一个新的 [Rate](../../com.aspose.tasks/rate) 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ratesFrom | java.util.Date | 新费率生效的日期。 |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### add(Date ratesFrom, int type) {#add-java.util.Date-int-}
```
public final Rate add(Date ratesFrom, int type)
```


向此集合添加一个新的 [Rate](../../com.aspose.tasks/rate) 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ratesFrom | java.util.Date | 新费率生效的日期。 |
| type | int | 要添加到的费率表。 |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### clear() {#clear--}
```
public final void clear()
```




### entrySet() {#entrySet--}
```
public Set<Map.Entry<Integer,RateByDateCollection>> entrySet()
```


(@inheritDoc\}

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;java.lang.Integer,com.aspose.tasks.RateByDateCollection&gt;&gt; - \{@inheritDoc\}
### get(Object key) {#get-java.lang.Object-}
```
public final RateByDateCollection get(Object key)
```


(@inheritDoc\}

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### getByRateType(int key) {#getByRateType-int-}
```
public final RateByDateCollection getByRateType(int key)
```


返回指定索引处的元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| key | int | 要获取的元素的零基索引。 |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - the element at the specified index.
### getParentResource() {#getParentResource--}
```
public final Resource getParentResource()
```


获取此集合的父级 [Resource](../../com.aspose.tasks/resource) 对象。

**Returns:**
[Resource](../../com.aspose.tasks/resource) - the parent [Resource](../../com.aspose.tasks/resource) object for this collection.
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


获取指示此集合是否只读的值。

**Returns:**
boolean - 指示此集合是否只读的值。
### iterator() {#iterator--}
```
public final Iterator iterator()
```


返回此集合的枚举器。

**Returns:**
java.util.Iterator - 此集合的枚举器。
### put(Integer key, RateByDateCollection value) {#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-}
```
public final RateByDateCollection put(Integer key, RateByDateCollection value)
```


(@inheritDoc\}

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| key | java.lang.Integer | \{@inheritDoc\} |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### remove(Rate item) {#remove-com.aspose.tasks.Rate-}
```
public final boolean remove(Rate item)
```


从此集合中移除 Rate 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [Rate](../../com.aspose.tasks/rate) | 要删除的项目。 |

**Returns:**
boolean - 如果成功删除指定的 Rate，则为 true；否则为 false。
### setByRateType(int key, RateByDateCollection value) {#setByRateType-int-com.aspose.tasks.RateByDateCollection-}
```
public final void setByRateType(int key, RateByDateCollection value)
```


设置指定索引处的元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| key | int | 要设置的元素的零基索引。 |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | 要在指定索引处设置的元素。 |

### size() {#size--}
```
public final int size()
```


获取 RateCollection 中包含的元素数量。

**Returns:**
int - RateCollection 中包含的元素数量。
### toList() {#toList--}
```
public final List<Rate> toList()
```


将 [RateCollection](../../com.aspose.tasks/ratecollection) 对象转换为 [Rate](../../com.aspose.tasks/rate) 对象的列表。

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - [Rate](../../com.aspose.tasks/rate) 对象的列表。
### toList(int type) {#toList-int-}
```
public final List<Rate> toList(int type)
```


将 [RateCollection](../../com.aspose.tasks/ratecollection) 对象转换为按指定 [RateType](../../com.aspose.tasks/ratetype) 类型过滤的 [Rate](../../com.aspose.tasks/rate) 对象列表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | 要过滤的类型。 |

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - [Rate](../../com.aspose.tasks/rate) 对象的列表。
