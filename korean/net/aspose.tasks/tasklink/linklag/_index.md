---
title: "TaskLink.LinkLag"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskLink 속성. 분의 10분의 1 단위 또는 백분율로 지연을 가져오거나 설정합니다"
type: docs
weight: 40
url: /ko/net/aspose.tasks/tasklink/linklag/
---
## TaskLink.LinkLag property

분의 10분의 1 또는 백분율로 지연을 가져오거나 설정합니다.

```csharp
public int LinkLag { get; set; }
```

## 예제

프로젝트 작업 링크를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

// 선행 작업 및 후속 작업의 이름을 표시합니다.
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Predecessor: " + taskLink.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor: " + taskLink.SuccTask.Get(Tsk.Name));
    Console.WriteLine("Lag Format: " + taskLink.LagFormat);
    Console.WriteLine("Link Lag: " + taskLink.LinkLag);
    Console.WriteLine();
}
```

### 또 보기

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


