---
title: "Tsk.ACWP"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 프로젝트 상태 날짜 또는 오늘 날짜까지 작업에 이미 수행된 작업에 대해 발생한 비용"
type: docs
weight: 110
url: /ko/net/aspose.tasks/tsk/acwp/
---
## Tsk.ACWP field

작업에 이미 수행된 작업에 대해 발생한 비용으로, 프로젝트 상태 날짜 또는 오늘 날짜까지 적용됩니다.

```csharp
public static readonly Key<double, TaskKey> ACWP;
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


