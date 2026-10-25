---
title: "Duration.Convert"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Duration 메서드. Duration 객체를 지정된 시간 단위로 다른 기간으로 변환합니다"
type: docs
weight: 70
url: /ko/net/aspose.tasks/duration/convert/
---
## Duration.Convert method

Duration 객체를 지정된 시간 단위로 다른 기간으로 변환합니다.

```csharp
public Duration Convert(TimeUnitType timeUnitType)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| timeUnitType | TimeUnitType | 지정된 시간 단위 유형입니다. |

### 반환 값

지정된 단위 유형으로 새로운 기간을 반환합니다.

## 예제

기간을 다양한 시간 단위 유형으로 변환하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// 작업을 가져와 다양한 형식으로 기간을 계산합니다.
var task = project.RootTask.Children.GetById(1);

// 분, 일, 시간, 주 및 월 단위의 기간을 가져옵니다.
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### 또 보기

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


