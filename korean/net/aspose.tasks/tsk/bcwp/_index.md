---
title: "Tsk.BCWP"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업 완료 비율에 시간 단계별 기준 비용을 곱한 누적값"
type: docs
weight: 120
url: /ko/net/aspose.tasks/tsk/bcwp/
---
## Tsk.BCWP field

작업의 완료 비율에 시간 단계별 기준 비용을 곱한 누적 값.

```csharp
public static readonly Key<double, TaskKey> BCWP;
```

## 예제

Shows how to read task cost values.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

foreach (var task in collector.Tasks)
{
    Console.WriteLine("Cost: " + task.Get(Tsk.Cost));
    Console.WriteLine("ACWP: " + task.Get(Tsk.ACWP));
    Console.WriteLine("BCWP: " + task.Get(Tsk.BCWP));
    Console.WriteLine("BCWS: " + task.Get(Tsk.BCWS));

    // CV = BCWP - ACWP
    Console.WriteLine("CV: " + task.Get(Tsk.CV));
    Console.WriteLine();
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


