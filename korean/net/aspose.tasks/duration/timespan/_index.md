---
title: "Duration.TimeSpan"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Duration 속성. 이 Duration 객체의 TimeSpan 인스턴스를 가져옵니다. 이 Duration 객체의 TimeSpan 인스턴스"
type: docs
weight: 40
url: /ko/net/aspose.tasks/duration/timespan/
---
## Duration.TimeSpan property

`TimeSpan` 인스턴스를 이 Duration 객체에서 가져옵니다. 이 Duration 객체의 TimeSpan 인스턴스.

```csharp
public TimeSpan TimeSpan { get; }
```

## 예제

기간을 시간 간격(TimeSpan)으로 변환하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// 작업 기간을 가져옵니다
var duration = task.Get(Tsk.Duration);
Console.WriteLine("Time span of duration: " + duration.TimeSpan);
```

### 또 보기

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


