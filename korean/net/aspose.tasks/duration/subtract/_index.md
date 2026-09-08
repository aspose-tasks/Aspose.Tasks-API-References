---
title: "Duration.Subtract"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Duration 메서드. 지정된 기간을 이 기간 인스턴스에서 빼습니다."
type: docs
weight: 100
url: /ko/net/aspose.tasks/duration/subtract/
---
## Subtract(Duration) {#subtract}

지정된 기간을 이 기간 인스턴스에서 빼습니다.

```csharp
public Duration Subtract(Duration d)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| d | Duration | 이 인스턴스에서 빼기 위한 지정된 [`Duration`](../) 인스턴스. |

### 반환 값

이 인스턴스의 값에서 지정된 기간 값을 뺀 값을 나타내는 새로운 기간 객체.

## 예제

작업의 기간을 변경하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// 작업을 가져옵니다
var task1 = project.RootTask.Children.GetById(1);

// 작업 기간을 업데이트합니다
var duration1 = task1.Get(Tsk.Duration);

// 작업 1에서 하루를 빼기
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// 작업에 새 기간을 설정합니다
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// 다른 작업을 가져옵니다
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// 실제 시간 단위 유형을 사용하여 기간을 변경합니다
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// 작업에 새 기간을 설정합니다
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### 또 보기

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Subtract(double) {#subtract_1}

지정된 double 값을 이 기간 인스턴스에서 빼습니다.

```csharp
public Duration Subtract(double val)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | Double | 이 인스턴스에서 빼기 위한 지정된 Double 값. |

### 반환 값

이 인스턴스의 값에서 지정된 기간 값을 뺀 값을 나타내는 새로운 기간 객체.

## 예제

작업의 기간을 변경하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// 작업을 가져옵니다
var task1 = project.RootTask.Children.GetById(1);

// 작업 기간을 업데이트합니다
var duration1 = task1.Get(Tsk.Duration);

// 작업 1에서 하루를 빼기
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// 작업에 새 기간을 설정합니다
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// 다른 작업을 가져옵니다
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// 실제 시간 단위 유형을 사용하여 기간을 변경합니다
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// 작업에 새 기간을 설정합니다
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### 또 보기

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


