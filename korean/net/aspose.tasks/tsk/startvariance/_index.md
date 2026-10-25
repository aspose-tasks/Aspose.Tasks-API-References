---
title: "Tsk.StartVariance"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업 또는 할당의 기준 시작 날짜와 현재 예정된 시작 날짜 사이의 차이를 나타내는 시간입니다."
type: docs
weight: 1040
url: /ko/net/aspose.tasks/tsk/startvariance/
---
## Tsk.StartVariance field

작업 또는 할당의 기준 시작 날짜와 현재 예정된 시작 날짜 사이의 차이를 나타내는 시간.

```csharp
public static readonly Key<Duration, TaskKey> StartVariance;
```

## 예제

Tsk.StartVariance 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Start Variance: " + task.Get(Tsk.StartVariance));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


