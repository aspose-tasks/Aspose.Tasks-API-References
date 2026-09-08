---
title: "Duration.op_Inequality"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Duration 메서드. 이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값을 반환합니다"
type: docs
weight: 150
url: /ko/net/aspose.tasks/duration/op_inequality/
---
## Duration Inequality operator

이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값을 반환합니다.

```csharp
public static bool operator !=(Duration a, Duration b)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | Duration | 첫 번째 기간입니다. |
| b | Duration | 두 번째 기간입니다. |

### 반환 값

이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값

## 예제

기간 동등성을 확인하는 방법을 보여줍니다.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// 기간의 동등성은 기본 Timespan에 대해 확인됩니다
Console.WriteLine("Duration 1: " + duration1.TimeSpan);
Console.WriteLine("Duration 2: " + duration2.TimeSpan);
Console.WriteLine("Duration 3: " + duration3.TimeSpan);
Console.WriteLine("Are durations 1 and 2 equal: " + duration1.Equals(duration2));
Console.WriteLine("Are durations 1 and 3 equal: " + duration1.Equals(duration3));
```

### 또 보기

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


