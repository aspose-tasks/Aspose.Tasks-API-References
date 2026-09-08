---
title: "Tsk.WorkVariance"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업의 기준 작업량과 현재 예정된 작업량 사이의 차이를 나타냅니다."
type: docs
weight: 1160
url: /ko/net/aspose.tasks/tsk/workvariance/
---
## Tsk.WorkVariance field

작업의 기준 작업과 현재 예정된 작업 사이의 차이.

```csharp
public static readonly Key<Duration, TaskKey> WorkVariance;
```

## 예제

Tsk.WorkVariance 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.WorkVariance, project.GetDuration(1));

Console.WriteLine("Work Variance: " + task.Get(Tsk.WorkVariance));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


