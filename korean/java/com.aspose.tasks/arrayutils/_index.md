---
title: "ArrayUtils"
second_title: "Aspose.Tasks for Java API Reference"
description: "ArrayList 처리를 위한 유틸리티 클래스."
type: docs
weight: 14
url: /ko/java/com.aspose.tasks/arrayutils/
---

**Inheritance:**
java.lang.Object
```
public class ArrayUtils
```

ArrayList 처리를 위한 유틸리티 클래스.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [&lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays)](#-T-concat-java.lang.Class-T--T--...-) |  |
| [apply(List array, IAlgorithm algorithm, int startIndex)](#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-) | 지정된 위치부터 시작하여 각 List 요소에 알고리즘을 적용합니다. |
| [filter(List array, ICondition cond)](#filter-java.util.List-com.aspose.tasks.ICondition-) | 지정된 조건에 따라 ArrayList 요소를 필터링합니다. |
| [find(List array, ICondition cond)](#find-java.util.List-com.aspose.tasks.ICondition-) | 지정된 조건을 만족하는 ArrayList 요소의 첫 번째 발생을 찾습니다. |
### &lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays) {#-T-concat-java.lang.Class-T--T--...-}
```
public static T[] <T>concat(Class<T> typeOfT, T[][] arrays)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| typeOfT | java.lang.Class&lt;T&gt; |  |
| 배열 | T[][] |  |

**Returns:**
T[]
### apply(List array, IAlgorithm algorithm, int startIndex) {#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-}
```
public static void apply(List array, IAlgorithm algorithm, int startIndex)
```


지정된 위치부터 시작하여 각 List 요소에 알고리즘을 적용합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 배열 | java.util.List | 처리할 ArrayList. |
| 알고리즘 | com.aspose.tasks.IAlgorithm | 적용된 알고리즘. |
| 시작인덱스 | int | 시작 요소 위치. |

### filter(List array, ICondition cond) {#filter-java.util.List-com.aspose.tasks.ICondition-}
```
public static List filter(List array, ICondition cond)
```


지정된 조건에 따라 ArrayList 요소를 필터링합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 배열 | java.util.List | 처리할 리스트. |
| 조건 | com.aspose.tasks.ICondition | List를 필터링하는 데 사용되는 조건. |

**Returns:**
java.util.List - 필터링된 List.
### find(List array, ICondition cond) {#find-java.util.List-com.aspose.tasks.ICondition-}
```
public static Object find(List array, ICondition cond)
```


지정된 조건을 만족하는 ArrayList 요소의 첫 번째 발생을 찾습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 배열 | java.util.List | 처리할 ArrayList. |
| 조건 | com.aspose.tasks.ICondition | ArrayList 요소를 찾는 데 사용되는 조건. |

**Returns:**
java.lang.Object - List 요소 또는 null.
