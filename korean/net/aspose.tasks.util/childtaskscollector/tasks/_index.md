---
title: "ChildTasksCollector.Tasks"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ChildTasksCollector 속성. 수집된 하위 객체 작업 목록을 가져옵니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.util/childtaskscollector/tasks/
---
## ChildTasksCollector.Tasks property

수집된 하위 객체(작업) 목록을 가져옵니다.

```csharp
public List<Task> Tasks { get; }
```

## 예제

프로젝트의 모든 작업을 평범한 목록으로 반복하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 수집된 모든 작업을 파싱합니다
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### 또 보기

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


