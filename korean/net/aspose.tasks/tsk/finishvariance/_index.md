---
title: "Tsk.FinishVariance"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk field. 작업 또는 할당의 기준선 완료 날짜와 현재 완료 날짜 사이의 차이를 나타내는 시간"
type: docs
weight: 420
url: /ko/net/aspose.tasks/tsk/finishvariance/
---
## Tsk.FinishVariance field

작업 또는 할당의 기준 종료 날짜와 현재 종료 날짜 간의 차이를 나타내는 시간.

```csharp
public static readonly Key<Duration, TaskKey> FinishVariance;
```

## 예제

Tsk.FinishVariance 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Finish Variance: " + task.Get(Tsk.FinishVariance));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


