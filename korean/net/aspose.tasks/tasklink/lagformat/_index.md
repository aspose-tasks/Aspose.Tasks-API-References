---
title: "TaskLink.LagFormat"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskLink 속성. 지연 형식을 표현하는 형식을 가져오거나 설정합니다"
type: docs
weight: 30
url: /ko/net/aspose.tasks/tasklink/lagformat/
---
## TaskLink.LagFormat property

지연 형식을 표현하는 포맷을 가져오거나 설정합니다.

```csharp
public TimeUnitType LagFormat { get; set; }
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

* enum [TimeUnitType](../../timeunittype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


