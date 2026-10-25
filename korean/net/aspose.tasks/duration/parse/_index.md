---
title: "Duration.Parse"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Duration 메서드. 지정된 문자열을 Duration 구조체의 인스턴스로 변환합니다"
type: docs
weight: 10
url: /ko/net/aspose.tasks/duration/parse/
---
## Duration.Parse method

지정된 문자열을 [`Duration`](../) 구조체의 인스턴스로 변환합니다.

```csharp
public static Duration Parse(Project p, string value)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| p | Project | 지정된 [`Project`](../../project/) 클래스 인스턴스를 대상으로 기간을 변환합니다. |
| value | 문자열 | 변환할 지정된 문자열. |

### 반환 값

변환된 [`Duration`](../) 구조체 인스턴스를 반환합니다.

## 예제

특수 형식 문자열에서 문자열을 구문 분석하는 방법을 보여줍니다.

```csharp
var project = new Project();

// 기간 예시:
// "1d", "1dy", "1d?", "1day", "1 dy", "1 edy? ", "8hr", "8 hour", "8hours", "0.2w?", "0.2wk", "0.2 eweek", "0.2ew?"
// 여기서 1 - 항목 수(일, 주 등), d - 일, h - 시간, w - 주, ? - 추정 플래그, e - 경과 플래그

// 추정 기간을 구문 분석해 보세요
var duration1 = Duration.Parse(project, "1d?");
Console.WriteLine("The parsed time span: " + duration1.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration1.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration1.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration1.IsElapsed);
Console.WriteLine();

// 추정 기간을 구문 분석해 보세요
var duration2 = Duration.Parse(project, "0.2 eweek");
Console.WriteLine("The parsed time span: " + duration2.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration2.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration2.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration2.IsElapsed);
```

### 또 보기

* class [Project](../../project/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


