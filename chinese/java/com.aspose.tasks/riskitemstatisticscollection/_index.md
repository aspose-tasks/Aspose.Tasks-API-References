---
title: "RiskItemStatisticsCollection"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示一个包含该类实例的集合。"
type: docs
weight: 266
url: /zh/java/com.aspose.tasks/riskitemstatisticscollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.util.Map, java.lang.Iterable
```
public class RiskItemStatisticsCollection implements Map<Task,RiskItemStatistics>, Iterable<RiskItemStatistics>
```

表示一个集合，包含 [RiskItemStatistics](../../com.aspose/tasks/riskitemstatistics) 类的实例。
## 方法

| 方法 | 描述 |
| --- | --- |
| [clear()](#clear--) | 从集合中移除所有项。 |
| [containsKey(Object key)](#containsKey-java.lang.Object-) | 如果此映射包含指定键的映射，则返回 true。 |
| [containsValue(Object value)](#containsValue-java.lang.Object-) | 如果此映射将一个或多个键映射到指定值，则返回 true。 |
| [entrySet()](#entrySet--) | 返回此映射中包含的映射的 Set 视图。 |
| [get(Object task)](#get-java.lang.Object-) | 返回此集合中与指定 Task 对象关联的 `RiskItemStatistics` 类的实例；如果未找到该项，则返回 null。 |
| [isEmpty()](#isEmpty--) | 如果此映射不包含键值映射，则返回 true |
| [iterator()](#iterator--) | 返回此集合的枚举器。 |
| [keySet()](#keySet--) | 返回此映射中包含的键的 Set 视图。 |
| [put(Task key, RiskItemStatistics value)](#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-) | 在此映射中将指定值与指定键关联。 |
| [putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m)](#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--) | 将指定映射中的所有映射复制到此映射中。 |
| [remove(Object key)](#remove-java.lang.Object-) | 如果存在，则从此映射中移除键的映射（如果存在）。 |
| [size()](#size--) | 返回此集合中的元素数量。 |
| [values()](#values--) | 返回此映射中包含的值的 Collection 视图。 |
### clear() {#clear--}
```
public void clear()
```


从集合中移除所有项。

### containsKey(Object key) {#containsKey-java.lang.Object-}
```
public boolean containsKey(Object key)
```


如果此映射包含指定键的映射，则返回 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - 如果此映射包含指定键的映射，则为 true。
### containsValue(Object value) {#containsValue-java.lang.Object-}
```
public boolean containsValue(Object value)
```


如果此映射将一个或多个键映射到指定值，则返回 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - 如果此映射将一个或多个键映射到指定值，则为 true。
### entrySet() {#entrySet--}
```
public Set<Map.Entry<Task,RiskItemStatistics>> entrySet()
```


返回此映射中包含的映射的 Set 视图。

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;com.aspose.tasks.Task,com.aspose.tasks.RiskItemStatistics&gt;&gt; - \{@inheritDoc\}
### get(Object task) {#get-java.lang.Object-}
```
public RiskItemStatistics get(Object task)
```


返回此集合中与指定 Task 对象关联的 `RiskItemStatistics` 类的实例；如果未找到该项，则返回 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 任务 | java.lang.Object | 指定的 `Task` 类实例。 |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - risk item which is associated with the specified task object if found; null otherwise.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


如果此映射不包含键值映射，则返回 true

**Returns:**
boolean - 如果此映射不包含键值映射，则为 true
### iterator() {#iterator--}
```
public Iterator<RiskItemStatistics> iterator()
```


返回此集合的枚举器。

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.RiskItemStatistics&gt; - 此集合的枚举器。
### keySet() {#keySet--}
```
public Set<Task> keySet()
```


返回此映射中包含的键的 Set 视图。

**Returns:**
java.util.Set&lt;com.aspose.tasks.Task&gt; - 此映射中包含的键的集合视图。
### put(Task key, RiskItemStatistics value) {#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-}
```
public RiskItemStatistics put(Task key, RiskItemStatistics value)
```


在此映射中将指定值与指定键关联。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| key | [Task](../../com.aspose.tasks/task) | \{@inheritDoc\} |
| value | [RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m) {#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--}
```
public void putAll(Map<? extends Task,? extends RiskItemStatistics> m)
```


将指定映射中的所有映射复制到此映射中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| m | java.util.Map&lt;? extends com.aspose.tasks.Task,? extends com.aspose.tasks.RiskItemStatistics&gt; | \{@inheritDoc\} |

### remove(Object key) {#remove-java.lang.Object-}
```
public RiskItemStatistics remove(Object key)
```


如果存在，则从此映射中移除键的映射（如果存在）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### size() {#size--}
```
public int size()
```


返回此集合中的元素数量。

**Returns:**
int - 此集合中的元素数量。
### values() {#values--}
```
public Collection<RiskItemStatistics> values()
```


返回此映射中包含的值的 Collection 视图。

**Returns:**
java.util.Collection&lt;com.aspose.tasks.RiskItemStatistics&gt; - 此映射中包含的值的集合视图。
