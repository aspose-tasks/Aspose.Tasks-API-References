---
title: "AndAllCondition"
second_title: "Aspose.Tasks for Java API Reference"
description: "모든 조건에 논리 AND를 적용합니다."
type: docs
weight: 11
url: /ko/java/com.aspose.tasks/andallcondition/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class AndAllCondition<T> implements ICondition<T>
```

모든 조건에 논리 AND를 적용합니다. 예: cond1 AND cond2 AND cond3...

T : 메서드 인터페이스를 적용할 객체 유형.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions)](#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---) | AndAllCondition&lt;T&gt; 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [check(T el)](#check-T-) | 지정된 객체가 조건을 만족하면 true를 반환합니다. |
### AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions) {#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---}
```
public AndAllCondition(List<ICondition<T>> conditions)
```


AndAllCondition&lt;T&gt; 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 조건 | java.util.List&lt;com.aspose.tasks.ICondition&lt;T&gt;&gt; | 조건 목록입니다. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


지정된 객체가 조건을 만족하면 true를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | T | 확인할 객체. |

**Returns:**
boolean - 객체가 조건을 만족하면 True.
