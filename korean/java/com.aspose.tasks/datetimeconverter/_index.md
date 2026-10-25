---
title: "DateTimeConverter"
second_title: "Aspose.Tasks for Java API Reference"
description: "보기 시간축 계층에서 날짜를 문자열로 변환하는 변환기를 나타냅니다."
type: docs
weight: 70
url: /ko/java/com.aspose.tasks/datetimeconverter/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class DateTimeConverter extends System.MulticastDelegate
```

보기 시간축 계층에서 날짜를 문자열로 변환하는 변환기를 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [DateTimeConverter()](#DateTimeConverter--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [invoke(Date date)](#invoke-java.util.Date-) | 보기 시간축 단계에서 날짜를 문자열로 변환하는 변환 메서드를 나타냅니다. |
### DateTimeConverter() {#DateTimeConverter--}
```
public DateTimeConverter()
```


### invoke(Date date) {#invoke-java.util.Date-}
```
public abstract String invoke(Date date)
```


보기 시간축 단계에서 날짜를 문자열로 변환하는 변환 메서드를 나타냅니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 날짜 | java.util.Date | `java.util.Date` 클래스의 인스턴스를 문자열로 변환합니다. |

**Returns:**
java.lang.String - 지정된 날짜의 문자열 표현.
