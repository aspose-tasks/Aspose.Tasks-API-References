---
title: "Tsk.Finish"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업의 예정 완료 날짜"
type: docs
weight: 390
url: /ko/net/aspose.tasks/tsk/finish/
---
## Tsk.Finish field

작업의 예정 종료 날짜.

```csharp
public static readonly Key<DateTime, TaskKey> Finish;
```

## 예제

작업 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

// 작업을 추가하고 작업 속성을 설정합니다
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 수집된 모든 작업을 파싱합니다
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


