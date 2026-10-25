---
title: "Duration.IsElapsed"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Duration 속성. 시간 단위가 경과했는지 여부를 나타내는 값을 가져옵니다. 이 Duration 인스턴스가 경과했는지 결정하는 플래그입니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/duration/iselapsed/
---
## Duration.IsElapsed property

시간 단위가 경과했는지 여부를 나타내는 값을 가져옵니다. 이 Duration 인스턴스가 경과했는지 결정하는 플래그입니다.

```csharp
public bool IsElapsed { get; }
```

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

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


