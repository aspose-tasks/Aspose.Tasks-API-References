---
title: "从指定位置开始，对每个 List 元素应用算法。"
second_title: "Aspose.Tasks for Java API 参考"
description: "用于 ArrayList 处理的实用类。"
type: docs
weight: 14
url: /zh/java/com.aspose.tasks/arrayutils/
---

**Inheritance:**
java.lang.Object
```
public class ArrayUtils
```

用于 ArrayList 处理的实用类。
## 方法

| 方法 | 描述 |
| --- | --- |
| [&lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays)](#-T-concat-java.lang.Class-T--T--...-) |  |
| [apply(List array, IAlgorithm algorithm, int startIndex)](#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-) | 根据指定条件过滤 ArrayList 元素。 |
| [filter(List array, ICondition cond)](#filter-java.util.List-com.aspose.tasks.ICondition-) | 根据指定条件过滤 ArrayList 元素。 |
| [find(List array, ICondition cond)](#find-java.util.List-com.aspose.tasks.ICondition-) | 查找满足指定条件的 ArrayList 元素的第一次出现。 |
### &lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays) {#-T-concat-java.lang.Class-T--T--...-}
```
public static T[] <T>concat(Class<T> typeOfT, T[][] arrays)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| typeOfT | java.lang.Class&lt;T&gt; |  |
| 数组 | T[][] |  |

**Returns:**
T[]
### apply(List array, IAlgorithm algorithm, int startIndex) {#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-}
```
public static void apply(List array, IAlgorithm algorithm, int startIndex)
```


根据指定条件过滤 ArrayList 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 数组 | java.util.List | 要处理的 ArrayList。 |
| 算法 | com.aspose.tasks.IAlgorithm | 已应用的算法。 |
| 起始索引 | int | 起始元素位置。 |

### filter(List array, ICondition cond) {#filter-java.util.List-com.aspose.tasks.ICondition-}
```
public static List filter(List array, ICondition cond)
```


根据指定条件过滤 ArrayList 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 数组 | java.util.List | 要处理的列表。 |
| cond | com.aspose.tasks.ICondition | 用于过滤 List 的条件。 |

**Returns:**
java.util.List - 已过滤的 List。
### find(List array, ICondition cond) {#find-java.util.List-com.aspose.tasks.ICondition-}
```
public static Object find(List array, ICondition cond)
```


查找满足指定条件的 ArrayList 元素的第一次出现。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 数组 | java.util.List | 要处理的 ArrayList。 |
| cond | com.aspose.tasks.ICondition | 用于查找 ArrayList 元素的条件。 |

**Returns:**
java.lang.Object - List 元素或 null。
