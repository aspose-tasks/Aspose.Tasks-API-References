---
title: "RiskItemStatisticsCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "인스턴스를 포함하는 컬렉션을 나타냅니다."
type: docs
weight: 266
url: /ko/java/com.aspose.tasks/riskitemstatisticscollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.util.Map, java.lang.Iterable
```
public class RiskItemStatisticsCollection implements Map<Task,RiskItemStatistics>, Iterable<RiskItemStatistics>
```

컬렉션은 [RiskItemStatistics](../../com.aspose/tasks/riskitemstatistics) 클래스의 인스턴스를 포함합니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [clear()](#clear--) | 컬렉션에서 모든 항목을 제거합니다. |
| [containsKey(Object key)](#containsKey-java.lang.Object-) | 지정된 키에 대한 매핑이 이 맵에 존재하면 true를 반환합니다. |
| [containsValue(Object value)](#containsValue-java.lang.Object-) | 지정된 값에 하나 이상의 키가 매핑되어 있으면 true를 반환합니다. |
| [entrySet()](#entrySet--) | 이 맵에 포함된 매핑의 Set 뷰를 반환합니다. |
| [get(Object task)](#get-java.lang.Object-) | 지정된 Task 객체와 연결된 이 컬렉션에 포함된 `RiskItemStatistics` 클래스의 인스턴스를 반환합니다; 찾지 못하면 null을 반환합니다. |
| [isEmpty()](#isEmpty--) | 이 맵에 키-값 매핑이 없으면 true를 반환합니다. |
| [iterator()](#iterator--) | 이 컬렉션에 대한 열거자를 반환합니다. |
| [keySet()](#keySet--) | 이 맵에 포함된 키의 Set 뷰를 반환합니다. |
| [put(Task key, RiskItemStatistics value)](#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-) | 지정된 값을 이 맵의 지정된 키와 연결합니다. |
| [putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m)](#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--) | 지정된 맵의 모든 매핑을 이 맵으로 복사합니다. |
| [remove(Object key)](#remove-java.lang.Object-) | 키에 대한 매핑이 존재하면 이 맵에서 해당 매핑을 제거합니다. |
| [size()](#size--) | 이 컬렉션의 요소 수를 반환합니다. |
| [values()](#values--) | 이 맵에 포함된 값들의 Collection 뷰를 반환합니다. |
### clear() {#clear--}
```
public void clear()
```


컬렉션에서 모든 항목을 제거합니다.

### containsKey(Object key) {#containsKey-java.lang.Object-}
```
public boolean containsKey(Object key)
```


지정된 키에 대한 매핑이 이 맵에 존재하면 true를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - 지정된 키에 대한 매핑이 이 맵에 존재하면 true.
### containsValue(Object value) {#containsValue-java.lang.Object-}
```
public boolean containsValue(Object value)
```


지정된 값에 하나 이상의 키가 매핑되어 있으면 true를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - 지정된 값에 하나 이상의 키가 매핑되어 있으면 true.
### entrySet() {#entrySet--}
```
public Set<Map.Entry<Task,RiskItemStatistics>> entrySet()
```


이 맵에 포함된 매핑의 Set 뷰를 반환합니다.

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;com.aspose.tasks.Task,com.aspose.tasks.RiskItemStatistics&gt;&gt; - \{@inheritDoc\}
### get(Object task) {#get-java.lang.Object-}
```
public RiskItemStatistics get(Object task)
```


지정된 Task 객체와 연결된 이 컬렉션에 포함된 `RiskItemStatistics` 클래스의 인스턴스를 반환합니다; 찾지 못하면 null을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 작업 | java.lang.Object | 지정된 `Task` 클래스의 인스턴스. |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - risk item which is associated with the specified task object if found; null otherwise.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


이 맵에 키-값 매핑이 없으면 true를 반환합니다.

**Returns:**
boolean - 이 맵에 키-값 매핑이 없을 경우 true
### iterator() {#iterator--}
```
public Iterator<RiskItemStatistics> iterator()
```


이 컬렉션에 대한 열거자를 반환합니다.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.RiskItemStatistics&gt; - 이 컬렉션에 대한 열거자.
### keySet() {#keySet--}
```
public Set<Task> keySet()
```


이 맵에 포함된 키의 Set 뷰를 반환합니다.

**Returns:**
java.util.Set&lt;com.aspose.tasks.Task&gt; - 이 맵에 포함된 키들의 집합 뷰.
### put(Task key, RiskItemStatistics value) {#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-}
```
public RiskItemStatistics put(Task key, RiskItemStatistics value)
```


지정된 값을 이 맵의 지정된 키와 연결합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| key | [Task](../../com.aspose.tasks/task) | \{@inheritDoc\} |
| value | [RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m) {#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--}
```
public void putAll(Map<? extends Task,? extends RiskItemStatistics> m)
```


지정된 맵의 모든 매핑을 이 맵으로 복사합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| m | java.util.Map&lt;? extends com.aspose.tasks.Task,? extends com.aspose.tasks.RiskItemStatistics&gt; | \{@inheritDoc\} |

### remove(Object key) {#remove-java.lang.Object-}
```
public RiskItemStatistics remove(Object key)
```


키에 대한 매핑이 존재하면 이 맵에서 해당 매핑을 제거합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### size() {#size--}
```
public int size()
```


이 컬렉션의 요소 수를 반환합니다.

**Returns:**
int - 이 컬렉션의 요소 수.
### values() {#values--}
```
public Collection<RiskItemStatistics> values()
```


이 맵에 포함된 값들의 Collection 뷰를 반환합니다.

**Returns:**
java.util.Collection&lt;com.aspose.tasks.RiskItemStatistics&gt; - 이 맵에 포함된 값들의 컬렉션 뷰.
