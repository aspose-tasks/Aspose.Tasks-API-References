---
title: "Tsk.ActualDuration"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 예정된 지속 시간과 현재 남은 작업량 또는 완료 비율을 기반으로 한 작업의 실제 작업 시간 범위입니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/tsk/actualduration/
---
## Tsk.ActualDuration field

작업에 대한 실제 작업 시간의 범위로, 예정된 기간과 현재 남은 작업량 또는 완료 비율을 기반으로 합니다.

```csharp
public static readonly Key<Duration, TaskKey> ActualDuration;
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
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


