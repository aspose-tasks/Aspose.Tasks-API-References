---
title: "ICondition"
second_title: "Aspose.Tasks for Java API Reference"
description: "필터 또는 검색 메서드에서 사용할 수 있는 조건을 나타냅니다."
type: docs
weight: 377
url: /ko/java/com.aspose.tasks/icondition/
---
```
public interface ICondition<T>
```

필터 또는 검색 메서드에서 사용할 수 있는 조건을 나타냅니다.

T : 메서드 인터페이스를 적용할 객체 유형.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [check(T el)](#check-T-) | 지정된 객체가 조건을 만족하면 true를 반환합니다. |
### check(T el) {#check-T-}
```
public abstract boolean check(T el)
```


지정된 객체가 조건을 만족하면 true를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | T | 확인할 객체. |

**Returns:**
boolean - 객체가 조건을 만족하면 True.
