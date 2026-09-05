---
title: "RiskItemStatisticsCollection"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "クラスのインスタンスを含むコレクションを表します。"
type: docs
weight: 266
url: /ja/java/com.aspose.tasks/riskitemstatisticscollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.util.Map, java.lang.Iterable
```
public class RiskItemStatisticsCollection implements Map<Task,RiskItemStatistics>, Iterable<RiskItemStatistics>
```

[RiskItemStatistics](../../com.aspose/tasks/riskitemstatistics) クラスのインスタンスを含むコレクションを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [clear()](#clear--) | コレクションからすべての項目を削除します。 |
| [containsKey(Object key)](#containsKey-java.lang.Object-) | 指定されたキーに対するマッピングがこのマップに含まれている場合、true を返します。 |
| [containsValue(Object value)](#containsValue-java.lang.Object-) | 指定された値に対して1つ以上のキーがこのマップにマッピングされている場合、true を返します。 |
| [entrySet()](#entrySet--) | このマップに含まれるマッピングの Set ビューを返します。 |
| [get(Object task)](#get-java.lang.Object-) | `RiskItemStatistics` クラスのインスタンスを返します。このコレクションに含まれ、指定された Task オブジェクトに関連付けられているものです。見つからない場合は null を返します。 |
| [isEmpty()](#isEmpty--) | このマップにキーと値のマッピングが存在しない場合、true を返します |
| [iterator()](#iterator--) | このコレクションの列挙子を返します。 |
| [keySet()](#keySet--) | このマップに含まれるキーの Set ビューを返します。 |
| [put(Task key, RiskItemStatistics value)](#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-) | 指定されたキーに指定された値をこのマップに関連付けます。 |
| [putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m)](#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--) | 指定されたマップからすべてのマッピングをこのマップにコピーします。 |
| [remove(Object key)](#remove-java.lang.Object-) | キーに対するマッピングが存在する場合、このマップからそれを削除します。 |
| [size()](#size--) | このコレクションの要素数を返します。 |
| [values()](#values--) | このマップに含まれる値の Collection ビューを返します。 |
### clear() {#clear--}
```
public void clear()
```


コレクションからすべての項目を削除します。

### containsKey(Object key) {#containsKey-java.lang.Object-}
```
public boolean containsKey(Object key)
```


指定されたキーに対するマッピングがこのマップに含まれている場合、true を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - 指定されたキーに対するマッピングがこのマップに含まれている場合は true。
### containsValue(Object value) {#containsValue-java.lang.Object-}
```
public boolean containsValue(Object value)
```


指定された値に対して1つ以上のキーがこのマップにマッピングされている場合、true を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - 指定された値に対して1つ以上のキーがこのマップにマッピングされている場合は true。
### entrySet() {#entrySet--}
```
public Set<Map.Entry<Task,RiskItemStatistics>> entrySet()
```


このマップに含まれるマッピングの Set ビューを返します。

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;com.aspose.tasks.Task,com.aspose.tasks.RiskItemStatistics&gt;&gt; - \\{@inheritDoc\\}
### get(Object task) {#get-java.lang.Object-}
```
public RiskItemStatistics get(Object task)
```


`RiskItemStatistics` クラスのインスタンスを返します。このコレクションに含まれ、指定された Task オブジェクトに関連付けられているものです。見つからない場合は null を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| タスク | java.lang.Object | `Task` クラスの指定されたインスタンス。 |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - risk item which is associated with the specified task object if found; null otherwise.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


このマップにキーと値のマッピングが存在しない場合、true を返します

**Returns:**
boolean - このマップにキーと値のマッピングが存在しない場合は true
### iterator() {#iterator--}
```
public Iterator<RiskItemStatistics> iterator()
```


このコレクションの列挙子を返します。

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.RiskItemStatistics&gt; - このコレクションの列挙子です。
### keySet() {#keySet--}
```
public Set<Task> keySet()
```


このマップに含まれるキーの Set ビューを返します。

**Returns:**
java.util.Set&lt;com.aspose.tasks.Task&gt; - このマップに含まれるキーの集合ビューです。
### put(Task key, RiskItemStatistics value) {#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-}
```
public RiskItemStatistics put(Task key, RiskItemStatistics value)
```


指定されたキーに指定された値をこのマップに関連付けます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| key | [Task](../../com.aspose.tasks/task) | \{@inheritDoc\} |
| value | [RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m) {#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--}
```
public void putAll(Map<? extends Task,? extends RiskItemStatistics> m)
```


指定されたマップからすべてのマッピングをこのマップにコピーします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| m | java.util.Map&lt;? extends com.aspose.tasks.Task,? extends com.aspose.tasks.RiskItemStatistics&gt; | \{@inheritDoc\} |

### remove(Object key) {#remove-java.lang.Object-}
```
public RiskItemStatistics remove(Object key)
```


キーに対するマッピングが存在する場合、このマップからそれを削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### size() {#size--}
```
public int size()
```


このコレクションの要素数を返します。

**Returns:**
int - このコレクションの要素数です。
### values() {#values--}
```
public Collection<RiskItemStatistics> values()
```


このマップに含まれる値の Collection ビューを返します。

**Returns:**
java.util.Collection&lt;com.aspose.tasks.RiskItemStatistics&gt; - このマップに含まれる値のコレクションビューです。
