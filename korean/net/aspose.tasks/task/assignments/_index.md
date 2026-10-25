---
title: "Task.Assignments"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 속성. 이 객체에 대한 리소스 할당 컬렉션을 가져옵니다."
type: docs
weight: 120
url: /ko/net/aspose.tasks/task/assignments/
---
## Task.Assignments property

이 객체에 대한 리소스 할당 컬렉션을 가져옵니다.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## 예제

작업 할당을 반복하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // 작업 할당을 표시합니다.
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### 또 보기

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


