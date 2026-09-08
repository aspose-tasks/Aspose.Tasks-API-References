---
title: "Tsk.BCWS"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk field. 상태 날짜 또는 오늘 날짜까지 누적된 단계별 기준선 비용"
type: docs
weight: 130
url: /ko/net/aspose.tasks/tsk/bcws/
---
## Tsk.BCWS field

상태 날짜 또는 오늘 날짜까지의 누적 시간 단계별 기준 비용.

```csharp
public static readonly Key<double, TaskKey> BCWS;
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


