---
title: "Not"
second_title: "Aspose.Tasks for Java API Reference"
description: "지정된 조건에 논리 NOT을 적용합니다."
type: docs
weight: 162
url: /ko/java/com.aspose.tasks/not/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class Not<T> implements ICondition<T>
```

지정된 조건에 논리 NOT을 적용합니다.

T : 메서드 인터페이스를 적용할 객체 유형.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Not(ICondition&lt;T&gt; condition)](#Not-com.aspose.tasks.ICondition-T--) | Not&lt;T&gt; 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [check(T el)](#check-T-) | 지정된 객체가 조건을 만족하면 true를 반환합니다. |
### Not(ICondition&lt;T&gt; condition) {#Not-com.aspose.tasks.ICondition-T--}
```
public Not(ICondition<T> condition)
```


Not&lt;T&gt; 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| condition | [ICondition](../../com.aspose.tasks/icondition) | 지정된 조건. |

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
boolean - 객체가 조건을 만족하면 true.
