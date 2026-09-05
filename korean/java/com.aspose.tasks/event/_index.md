---
title: "이벤트"
second_title: "Aspose.Tasks for Java API Reference"
description: "이벤트."
type: docs
weight: 374
url: /ko/java/com.aspose.tasks/event/
---
```
public interface Event<TArgs>
```

이벤트.

`TArgs`: 이벤트 인수.

TArgs :
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | 이 메서드는 이벤트가 발생될 때 호출됩니다. |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


이 메서드는 이벤트가 발생될 때 호출됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 보내는 객체 | java.lang.Object | 이 이벤트를 시작하는 객체. |
| args | TArgs | 사용자 정의 인수. |

