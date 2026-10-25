---
title: "Tsk.ActualCost"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 리소스가 작업에서 이미 수행한 작업에 발생한 비용과 작업과 관련된 기타 기록된 비용"
type: docs
weight: 20
url: /ko/net/aspose.tasks/tsk/actualcost/
---
## Tsk.ActualCost field

리소스가 자신의 작업에서 이미 수행한 작업에 대해 발생한 비용과 작업과 연관된 기타 기록된 비용을 포함합니다.

```csharp
public static readonly Key<decimal, TaskKey> ActualCost;
```

## 예제

작업의 실제 속성을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ActualTaskProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 수집된 모든 작업을 파싱합니다
foreach (var task in collector.Tasks)
{
    Console.WriteLine("Task Name : " + task.Get(Tsk.Name));
    Console.WriteLine("Actual Start: " + task.Get(Tsk.ActualStart).ToLongDateString());
    Console.WriteLine("Actual Finish: " + task.Get(Tsk.ActualFinish).ToLongDateString());
    Console.WriteLine("Actual Duration: " + task.Get(Tsk.ActualDuration).TimeSpan.Hours);
    Console.WriteLine("Actual Cost: " + task.Get(Tsk.ActualCost));
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


