---
title: Duration
second_title: .NET API 참조용 Aspose.Tasks
description: 프로젝트의 기간을 나타냅니다.
type: docs
weight: 470
url: /ko/net/aspose.tasks/duration/
---
## Duration structure

프로젝트의 기간을 나타냅니다.

```csharp
public struct Duration : IEquatable<Duration>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [IsElapsed](../../aspose.tasks/duration/iselapsed/) { get; } | 시간 단위 경과 여부를 나타내는 값을 가져옵니다. 이 Duration 인스턴스가 경과되었는지 여부를 결정하는 플래그입니다. |
| [IsEstimated](../../aspose.tasks/duration/isestimated/) { get; } | 시간 단위의 추정 여부를 나타내는 값을 가져옵니다. 이 Duration 인스턴스가 예상되는지 여부를 결정하는 플래그입니다. |
| [TimeSpan](../../aspose.tasks/duration/timespan/) { get; } | 가져오기[`TimeSpan`](./timespan/) 이 Duration 객체의 인스턴스. 이 Duration 개체의 TimeSpan 인스턴스입니다. |
| [TimeUnit](../../aspose.tasks/duration/timeunit/) { get; } | 이 개체의 시간 단위 유형을 가져옵니다. 이 Duration 인스턴스의 시간 단위 유형입니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| static [Parse](../../aspose.tasks/duration/parse/)(Project, string) | 지정된 문자열을 인스턴스로 변환합니다.`Duration` 구조체. |
| [Add](../../aspose.tasks/duration/add/#add_1)(double) | 지정된 double 값을 이 기간에 추가합니다. |
| [Add](../../aspose.tasks/duration/add/#add)(Duration) | 지정된 기간을 이 기간에 추가합니다. |
| [Convert](../../aspose.tasks/duration/convert/)(TimeUnitType) | Duration 개체를 지정된 시간 단위의 다른 기간으로 변환합니다. |
| [Equals](../../aspose.tasks/duration/equals/#equals)(Duration) | 이 인스턴스가 지정된 개체와 같은지 여부를 나타내는 값을 반환합니다. |
| override [Equals](../../aspose.tasks/duration/equals/#equals_1)(object) | 이 인스턴스가 지정된 개체와 같은지 여부를 나타내는 값을 반환합니다. |
| override [GetHashCode](../../aspose.tasks/duration/gethashcode/)() | 이 개체의 해시 코드 값을 반환합니다. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract_1)(double) | 이 기간 인스턴스에서 지정된 double 값을 뺍니다. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract)(Duration) | 이 기간 인스턴스에서 지정된 기간을 뺍니다. |
| [ToDouble](../../aspose.tasks/duration/todouble/)() | 기간 개체를 다음으로 변환합니다.Double 값. |
| override [ToString](../../aspose.tasks/duration/tostring/)() | 이 인스턴스의 문자열 표현을 반환합니다. |
| static [ParseTimeSpan](../../aspose.tasks/duration/parsetimespan/)(string) | "PT--H--M--S--" 형식의 기간 문자열을 구문 분석합니다. |
| [operator ==](../../aspose.tasks/duration/op_equality/) | 이 인스턴스가 지정된 개체와 같은지 여부를 나타내는 값을 반환합니다. |
| [operator !=](../../aspose.tasks/duration/op_inequality/) | 이 인스턴스가 지정된 개체와 같지 않은지 여부를 나타내는 값을 반환합니다. |

### 또한보십시오

* 네임스페이스 [Aspose.Tasks](../../aspose.tasks/)
* 집회 [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
