---
title: "Tsk.OutlineLevel"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업의 개요 수준"
type: docs
weight: 840
url: /ko/net/aspose.tasks/tsk/outlinelevel/
---
## Tsk.OutlineLevel field

작업의 개요 수준.

```csharp
public static readonly Key<int, TaskKey> OutlineLevel;
```

## 예제

작업 개요 속성을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TaskOutlineProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 수집된 모든 작업을 파싱합니다
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Level : " + task.Get(Tsk.OutlineLevel));
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Number : " + task.Get(Tsk.OutlineNumber));
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


