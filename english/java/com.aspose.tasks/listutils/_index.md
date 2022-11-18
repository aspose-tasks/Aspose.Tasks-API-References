---
title: ListUtils
second_title: Aspose.Tasks for Java API Reference
description: Utility class for list processing.
type: docs
weight: 136
url: /java/com.aspose.tasks/listutils/
---

**Inheritance:**
java.lang.Object
```
public class ListUtils
```

Utility class for list processing.
## Methods

| Method | Description |
| --- | --- |
| [&lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex)](#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-) | Apply algorithm for each list element starting from specified position. |
| [&lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond)](#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--) | Filter list elements by specified condition. |
| [&lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz)](#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-) | Find first occurrence of an list element which satisfy specified condition. |
### &lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex) {#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-}
```
public static void <T>apply(List<T> list, IAlgorithm<T> algorithm, int startIndex)
```


Apply algorithm for each list element starting from specified position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| list | java.util.List&lt;T&gt; | List to process. |
| algorithm | [IAlgorithm](../../com.aspose.tasks/ialgorithm) | Applied algorithm. |
| startIndex | int | Start element position. |

### &lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond) {#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--}
```
public static List<T> <T>filter(List<T> list, ICondition<T> cond)
```


Filter list elements by specified condition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| list | java.util.List&lt;T&gt; | A list to process. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Condition used to filter the specified list. |

**Returns:**
java.util.List&lt;T&gt; - Filtered list.
### &lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz) {#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-}
```
public static T <T>find(List<T> list, ICondition<T> cond, Class clazz)
```


Find first occurrence of an list element which satisfy specified condition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| list | java.util.List&lt;T&gt; | A list to process. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Condition used to find an element in the specified list. |
| clazz | java.lang.Class | Class type of element T. |

**Returns:**
T - List element or null.
