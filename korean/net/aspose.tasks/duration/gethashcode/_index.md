---
title: "Duration.GetHashCode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Duration 메서드. 이 객체에 대한 해시 코드 값을 반환합니다."
type: docs
weight: 90
url: /ko/net/aspose.tasks/duration/gethashcode/
---
## Duration.GetHashCode method

이 객체에 대한 해시 코드 값을 반환합니다.

```csharp
public override int GetHashCode()
```

### 반환 값

이 Duration 인스턴스에 대한 해시 코드 값을 반환합니다.

## 예제

Duration의 해시 코드를 얻는 방법을 보여줍니다.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// 캘린더의 해시 코드는 시간 단위 유형과 Duration의 초기 값을 기반으로 합니다.
// 따라서 다음 해시 코드는 동일합니다.
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 2 Hash Code: {0}", duration2.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration2.GetHashCode()));

// 하지만 Duration 1과 3의 해시 코드는 동일하지 않습니다.
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 3 Hash Code: {0}", duration3.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration3.GetHashCode()));
```

### 또 보기

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


