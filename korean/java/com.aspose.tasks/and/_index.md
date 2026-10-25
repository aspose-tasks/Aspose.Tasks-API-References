---
title: "그리고"
second_title: "Aspose.Tasks for Java API Reference"
description: "지정된 조건에 논리 AND를 적용합니다."
type: docs
weight: 10
url: /ko/java/com.aspose.tasks/and/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class And<T> implements ICondition<T>
```

지정된 조건에 논리 AND를 적용합니다.

T : 메서드 인터페이스를 적용할 객체 유형.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2)](#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--) | And&lt;T&gt; 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [check(T el)](#check-T-) | 지정된 객체가 조건을 만족하면 true를 반환합니다. |
### And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2) {#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--}
```
public And(ICondition<T> cond1, ICondition<T> cond2)
```


And&lt;T&gt; 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| cond1 | [ICondition](../../com.aspose.tasks/icondition) | 첫 번째 조건. |
| cond2 | [ICondition](../../com.aspose.tasks/icondition) | 두 번째 조건. |

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
