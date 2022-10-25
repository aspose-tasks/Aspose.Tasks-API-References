---
title: ArrayUtils
second_title: Aspose.Tasks for Java API Reference
description: Utility class for ArrayList processing.
type: docs
weight: 14
url: /java/com.aspose.tasks/arrayutils/
---

**Inheritance:**
java.lang.Object
```
public class ArrayUtils
```

Utility class for ArrayList processing.
## Methods

| Method | Description |
| --- | --- |
| [&lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[]... arrays)](#-T-concat-java.lang.Class-T--T--...-) |  |
| [apply(List array, IAlgorithm algorithm, int startIndex)](#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-) | Apply algorithm for each List element starting from specified position. |
| [filter(List array, ICondition cond)](#filter-java.util.List-com.aspose.tasks.ICondition-) | Filter ArrayList elements by specified condition. |
| [find(List array, ICondition cond)](#find-java.util.List-com.aspose.tasks.ICondition-) | Find first occurrence of an ArrayList element which satisfy specified condition. |
### &lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[]... arrays) {#-T-concat-java.lang.Class-T--T--...-}
```
public static T[] <T>concat(Class<T> typeOfT, T[]... arrays)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| typeOfT | java.lang.Class&lt;T&gt; |  |
| arrays | T[]... |  |

**Returns:**
T[]
### apply(List array, IAlgorithm algorithm, int startIndex) {#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-}
```
public static void apply(List array, IAlgorithm algorithm, int startIndex)
```


Apply algorithm for each List element starting from specified position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| array | java.util.List | ArrayList to process. |
| algorithm | com.aspose.tasks.IAlgorithm | Applied algorithm. |
| startIndex | int | Start element position. |

### filter(List array, ICondition cond) {#filter-java.util.List-com.aspose.tasks.ICondition-}
```
public static List filter(List array, ICondition cond)
```


Filter ArrayList elements by specified condition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| array | java.util.List | List to process. |
| cond | com.aspose.tasks.ICondition | Condition used to filter List. |

**Returns:**
java.util.List - Filtered List.
### find(List array, ICondition cond) {#find-java.util.List-com.aspose.tasks.ICondition-}
```
public static Object find(List array, ICondition cond)
```


Find first occurrence of an ArrayList element which satisfy specified condition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| array | java.util.List | ArrayList to process. |
| cond | com.aspose.tasks.ICondition | Condition used to find ArrayList element. |

**Returns:**
java.lang.Object - List element or null.
