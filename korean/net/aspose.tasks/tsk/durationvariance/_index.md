---
title: "Tsk.DurationVariance"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업의 기준 지속 시간과 현재 추정 총 지속 시간 사이의 차이입니다."
type: docs
weight: 320
url: /ko/net/aspose.tasks/tsk/durationvariance/
---
## Tsk.DurationVariance field

작업의 기준 기간과 총 기간(현재 추정치) 간의 차이.

```csharp
public static readonly Key<Duration, TaskKey> DurationVariance;
```

## 예제

Tsk.DurationVariance 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationVariance, project.GetWork(1));

Console.WriteLine("Duration Variance: " + task.Get(Tsk.DurationVariance));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


