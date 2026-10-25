---
title: "Tsk.Priority"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업에 부여된 중요도 수준으로, 이는 리소스 레벨링 중 작업이나 할당이 얼마나 쉽게 지연되거나 분할될 수 있는지를 나타냅니다."
type: docs
weight: 930
url: /ko/net/aspose.tasks/tsk/priority/
---
## Tsk.Priority field

작업에 부여된 중요도 수준으로, 이는 리소스 레벨링 중 작업이나 할당이 얼마나 쉽게 지연되거나 분할될 수 있는지를 나타냅니다.

```csharp
public static readonly Key<int, TaskKey> Priority;
```

## 예제

작업 우선순위를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TaskPriority.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 모든 작업에 대한 우선순위 표시
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Priority : " + task.Get(Tsk.Priority));
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


