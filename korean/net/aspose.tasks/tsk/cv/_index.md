---
title: "Tsk.CV"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업에 대한 기준 비용과 총 비용의 차이. 비용 편차  비용  기준 비용"
type: docs
weight: 260
url: /ko/net/aspose.tasks/tsk/cv/
---
## Tsk.CV field

작업에 대한 기준 비용과 총 비용 간의 차이. 비용 차이 = 비용 - 기준 비용

```csharp
public static readonly Key<double, TaskKey> CV;
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


