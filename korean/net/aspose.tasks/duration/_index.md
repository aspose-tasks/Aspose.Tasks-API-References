---
title: "구조체 Duration"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Duration 구조체. 프로젝트의 기간을 나타냅니다."
type: docs
weight: 470
url: /ko/net/aspose.tasks/duration/
---
## Duration structure

프로젝트에서 기간을 나타냅니다.

```csharp
public struct Duration : IEquatable<Duration>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [IsElapsed](../../aspose.tasks/duration/iselapsed/) { get; } | 시간 단위가 경과했는지 여부를 나타내는 값을 가져옵니다. 이 Duration 인스턴스가 경과했는지 결정하는 플래그입니다. |
| [IsEstimated](../../aspose.tasks/duration/isestimated/) { get; } | 시간 단위가 추정되었는지 여부를 나타내는 값을 가져옵니다. 이 Duration 인스턴스가 추정되었는지 결정하는 플래그입니다. |
| [TimeSpan](../../aspose.tasks/duration/timespan/) { get; } | 이 Duration 객체의 [`TimeSpan`](./timespan/) 인스턴스를 가져옵니다. 이 Duration 객체의 TimeSpan 인스턴스. |
| [TimeUnit](../../aspose.tasks/duration/timeunit/) { get; } | 이 객체의 시간 단위 유형을 가져옵니다. 이 Duration 인스턴스의 시간 단위 유형. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| static [Parse](../../aspose.tasks/duration/parse/)(Project, string) | 지정된 문자열을 `Duration` 구조체의 인스턴스로 변환합니다. |
| [Add](../../aspose.tasks/duration/add/#add_1)(double) | 지정된 double 값을 이 기간에 추가합니다. |
| [Add](../../aspose.tasks/duration/add/#add)(Duration) | 지정된 기간을 이 기간에 추가합니다. |
| [Convert](../../aspose.tasks/duration/convert/)(TimeUnitType) | Duration 객체를 지정된 시간 단위로 다른 기간으로 변환합니다. |
| [Equals](../../aspose.tasks/duration/equals/#equals)(Duration) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| override [Equals](../../aspose.tasks/duration/equals/#equals_1)(object) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| override [GetHashCode](../../aspose.tasks/duration/gethashcode/)() | 이 객체에 대한 해시 코드 값을 반환합니다. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract_1)(double) | 지정된 double 값을 이 기간 인스턴스에서 빼습니다. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract)(Duration) | 지정된 기간을 이 기간 인스턴스에서 빼습니다. |
| [ToDouble](../../aspose.tasks/duration/todouble/)() | Duration 객체를 Double 값으로 변환합니다. |
| override [ToString](../../aspose.tasks/duration/tostring/)() | 이 인스턴스의 문자열 표현을 반환합니다. |
| static [ParseTimeSpan](../../aspose.tasks/duration/parsetimespan/)(string) | "PT--H--M--S--" 형식의 기간 문자열을 구문 분석합니다. |
| [operator ==](../../aspose.tasks/duration/op_equality/) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [operator !=](../../aspose.tasks/duration/op_inequality/) | 이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값을 반환합니다. |

## 예제

작업의 기간을 업데이트하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// 작업을 가져옵니다
var task1 = project.RootTask.Children.GetById(1);

// 작업 기간을 업데이트합니다
var duration1 = task1.Get(Tsk.Duration);

// 작업 1에 하루를 추가합니다
duration1 = duration1.Add(project.GetDuration(1, TimeUnitType.Day));

// 작업에 새 기간을 설정합니다
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// 다른 작업을 가져옵니다
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// 실제 시간 단위 유형을 사용하여 기간을 변경합니다
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Add(1d /* the time unit type of duration2 will be used */);

// 작업에 새 기간을 설정합니다
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task1.Get(Tsk.Duration));
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


