---
title: "Tsk.IsMilestone"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업이 마일스톤인지 여부를 결정합니다"
type: docs
weight: 630
url: /ko/net/aspose.tasks/tsk/ismilestone/
---
## Tsk.IsMilestone field

작업이 마일스톤인지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, TaskKey> IsMilestone;
```

## 예제

예상 작업 및/또는 마일스톤 작업을 찾는 방법을 보여줍니다.

```csharp
var prj = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(prj.RootTask, collector, 0);

// 수집된 작업을 반복합니다
foreach (var task in collector.Tasks)
{
    var estimated = task.Get(Tsk.IsEstimated).Value ? "Estimated" : "Non-Estimated";
    var milestone = task.Get(Tsk.IsMilestone).Value ? "Milestone" : "Non-Milestone";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + estimated);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + milestone);
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


