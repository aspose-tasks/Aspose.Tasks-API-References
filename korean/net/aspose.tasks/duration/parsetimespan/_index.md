---
title: "Duration.ParseTimeSpan"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Duration 메서드. PTHMS 형식의 기간 문자열을 구문 분석합니다."
type: docs
weight: 130
url: /ko/net/aspose.tasks/duration/parsetimespan/
---
## Duration.ParseTimeSpan method

"PT--H--M--S--" 형식의 기간 문자열을 구문 분석합니다.

```csharp
public static TimeSpan ParseTimeSpan(string value)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | 문자열 | 구문 분석할 지정된 문자열. |

### 반환 값

구문 분석된 [`TimeSpan`](../timespan/) 구조체 인스턴스를 반환합니다.

## 예제

문자열을 시간 간격으로 변환하는 방법을 보여줍니다.

```csharp
var timeSpan = Duration.ParseTimeSpan("PT1H10M30S");
Console.WriteLine("The parsed time span: " + timeSpan);
```

### 또 보기

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


