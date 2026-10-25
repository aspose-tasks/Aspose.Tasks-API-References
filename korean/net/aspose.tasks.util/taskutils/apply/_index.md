---
title: "TaskUtils.Apply"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskUtils 메서드. 트리의 각 작업에 지정된 알고리즘을 적용합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.util/taskutils/apply/
---
## TaskUtils.Apply method

지정된 알고리즘을 트리의 각 작업에 적용합니다.

```csharp
public static void Apply(Task root, ITreeAlgorithm<Task> alg, int level)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| root | 작업 | 트리의 루트 |
| alg | ITreeAlgorithm`1 | 적용된 알고리즘. |
| 레벨 | Int32 | 루트 작업의 레벨. |

## 예제

트리 알고리즘을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// 모든 프로젝트 작업을 수집합니다
var coll = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, coll, 0);

// 작업을 일반 목록처럼 다룹니다
foreach (var task in coll.Tasks)
{
    Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
}
```

### 또 보기

* class [Task](../../../aspose.tasks/task/)
* interface [ITreeAlgorithm&lt;T&gt;](../../itreealgorithm-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


