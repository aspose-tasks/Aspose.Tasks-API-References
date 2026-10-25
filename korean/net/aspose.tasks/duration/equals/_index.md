---
title: "Duration.Equals"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Duration 메서드. 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다."
type: docs
weight: 80
url: /ko/net/aspose.tasks/duration/equals/
---
## Equals(Duration) {#equals}

이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

```csharp
public bool Equals(Duration other)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 다른 | Duration | 이 인스턴스와 비교할 객체. |

### 반환 값

다른 Duration 인스턴스가 이 인스턴스와 동일한 TimeSpan 및 TimeUnit 값을 가지고 있으면 **True**를 반환하고, 그렇지 않으면 **false**를 반환합니다.

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

---

## Equals(object) {#equals_1}

이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

```csharp
public override bool Equals(object obj)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | Object | 이 인스턴스와 비교할 객체. |

### 반환 값

**True** if the specified object is a Duration that has the same TimeSpan and TimeUnit values as this instance; otherwise, **false**.

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


