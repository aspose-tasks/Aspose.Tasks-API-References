---
title: "ListUtils"
second_title: "Aspose.Tasks for Java API Reference"
description: "목록 처리를 위한 유틸리티 클래스."
type: docs
weight: 147
url: /ko/java/com.aspose.tasks/listutils/
---

**Inheritance:**
java.lang.Object
```
public class ListUtils
```

목록 처리를 위한 유틸리티 클래스.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [&lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex)](#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-) | 지정된 위치부터 시작하여 각 리스트 요소에 알고리즘을 적용합니다. |
| [&lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond)](#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--) | 지정된 조건에 따라 리스트 요소를 필터링합니다. |
| [&lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz)](#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-) | 지정된 조건을 만족하는 리스트 요소의 첫 번째 발생을 찾습니다. |
### &lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex) {#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-}
```
public static void <T>apply(List<T> list, IAlgorithm<T> algorithm, int startIndex)
```


지정된 위치부터 시작하여 각 리스트 요소에 알고리즘을 적용합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| list | java.util.List&lt;T&gt; | 처리할 리스트. |
| algorithm | [IAlgorithm](../../com.aspose.tasks/ialgorithm) | 적용된 알고리즘. |
| 시작인덱스 | int | 시작 요소 위치. |

### &lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond) {#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--}
```
public static List<T> <T>filter(List<T> list, ICondition<T> cond)
```


지정된 조건에 따라 리스트 요소를 필터링합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| list | java.util.List&lt;T&gt; | 처리할 리스트. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | 지정된 리스트를 필터링하는 데 사용되는 조건. |

**Returns:**
java.util.List&lt;T&gt; - 필터링된 리스트.
### &lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz) {#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-}
```
public static T <T>find(List<T> list, ICondition<T> cond, Class clazz)
```


지정된 조건을 만족하는 리스트 요소의 첫 번째 발생을 찾습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| list | java.util.List&lt;T&gt; | 처리할 리스트. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | 지정된 리스트에서 요소를 찾는 데 사용되는 조건. |
| clazz | java.lang.Class | 요소 T의 클래스 유형. |

**Returns:**
T - 리스트 요소 또는 null.
