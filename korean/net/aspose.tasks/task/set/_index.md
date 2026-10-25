---
title: "Task.Set"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 메서드. 지정된 속성을 이 컨테이너의 지정된 값에 매핑합니다."
type: docs
weight: 1410
url: /ko/net/aspose.tasks/task/set/
---
## Task.Set&lt;T&gt; method

이 컨테이너에서 지정된 속성을 지정된 값에 매핑합니다.

```csharp
public void Set<T>(Key<T, TaskKey> key, T val)
```

| 매개변수 | 설명 |
| --- | --- |
| T | 매핑된 값의 유형. |
| key | 지정된 속성 키. [`Tsk`](../../tsk/)는 속성 키를 가져오기 위해 사용됩니다. |
| 값 | 값입니다. |

## 예제

작업 속성을 가져오고/설정하는 방법을 보여줍니다.

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
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


