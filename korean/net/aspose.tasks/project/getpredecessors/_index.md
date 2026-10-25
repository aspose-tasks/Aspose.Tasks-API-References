---
title: "Project.GetPredecessors"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 메서드. 지정된 작업의 선행 작업인 작업 링크 컬렉션을 반환합니다"
type: docs
weight: 1120
url: /ko/net/aspose.tasks/project/getpredecessors/
---
## Project.GetPredecessors method

지정된 작업의 선행 작업인 작업 링크 컬렉션을 반환합니다.

```csharp
public TaskLinkCollection GetPredecessors(Task task)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 작업 | 작업 | 선행 작업을 가져올 작업입니다. |

### 반환 값

선행 작업 [`TaskLink`](../../tasklink/) 목록.

## 예제

특정 작업에 대한 선행 작업을 가져오는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");
var task = project.RootTask.Children.GetById(10);

var predecessors = project.GetPredecessors(task);

// 선행 작업 및 후속 작업의 이름을 표시합니다.
foreach (var predecessor in predecessors)
{
    Console.WriteLine("Predecessor " + predecessor.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor " + predecessor.SuccTask.Get(Tsk.Name));
}
```

### 또 보기

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


