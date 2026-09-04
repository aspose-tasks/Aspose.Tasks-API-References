---
title: "ListUtils"
second_title: "Aspose.Tasks for Java API 参考"
description: "用于列表处理的实用类。"
type: docs
weight: 147
url: /zh/java/com.aspose.tasks/listutils/
---

**Inheritance:**
java.lang.Object
```
public class ListUtils
```

用于列表处理的实用类。
## 方法

| 方法 | 描述 |
| --- | --- |
| [&lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex)](#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-) | 从指定位置开始，对每个列表元素应用算法。 |
| [&lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond)](#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--) | 根据指定条件过滤列表元素。 |
| [&lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz)](#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-) | 查找满足指定条件的列表元素的首次出现。 |
### &lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex) {#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-}
```
public static void <T>apply(List<T> list, IAlgorithm<T> algorithm, int startIndex)
```


从指定位置开始，对每个列表元素应用算法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| list | java.util.List&lt;T&gt; | 要处理的列表。 |
| algorithm | [IAlgorithm](../../com.aspose.tasks/ialgorithm) | 已应用的算法。 |
| 起始索引 | int | 起始元素位置。 |

### &lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond) {#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--}
```
public static List<T> <T>filter(List<T> list, ICondition<T> cond)
```


根据指定条件过滤列表元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| list | java.util.List&lt;T&gt; | 要处理的列表。 |
| cond | [ICondition](../../com.aspose.tasks/icondition) | 用于过滤指定列表的条件。 |

**Returns:**
java.util.List&lt;T&gt; - 已过滤的列表。
### &lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz) {#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-}
```
public static T <T>find(List<T> list, ICondition<T> cond, Class clazz)
```


查找满足指定条件的列表元素的首次出现。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| list | java.util.List&lt;T&gt; | 要处理的列表。 |
| cond | [ICondition](../../com.aspose.tasks/icondition) | 用于在指定列表中查找元素的条件。 |
| clazz | java.lang.Class | 元素 T 的类类型。 |

**Returns:**
T - 列表元素或 null。
