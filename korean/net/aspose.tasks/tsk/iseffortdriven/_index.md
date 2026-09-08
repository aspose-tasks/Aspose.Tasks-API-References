---
title: "Tsk.IsEffortDriven"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업에 대한 일정이 노력 기반인지 여부를 결정합니다."
type: docs
weight: 570
url: /ko/net/aspose.tasks/tsk/iseffortdriven/
---
## Tsk.IsEffortDriven field

작업 일정이 노력 기반 일정인지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, TaskKey> IsEffortDriven;
```

## 예제

중요 및/또는 노력 기반 작업을 찾는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CriticalEffortDrivenTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 수집된 모든 작업을 파싱합니다
foreach (var task in collector.Tasks)
{
    var effortDriven = task.Get(Tsk.IsEffortDriven).Value ? "EffortDriven" : "Non-EffortDriven";
    var nonCritical = task.Get(Tsk.IsCritical).Value ? "Critical" : "Non-Critical";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + effortDriven);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + nonCritical);
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


