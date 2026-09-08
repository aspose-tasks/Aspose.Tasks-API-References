---
title: "Task.Status"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 속성. 작업 상태를 가져옵니다."
type: docs
weight: 1160
url: /ko/net/aspose.tasks/task/status/
---
## Task.Status property

작업 상태를 가져옵니다.

```csharp
public TaskStatus Status { get; }
```

## 예제

작업 상태를 가져오는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TaskPercentageCompletion.mpp");

// 상태 계산에 상태 날짜가 사용되므로 Project의 상태 날짜를 설정해야 합니다.
project.StatusDate = new DateTime(2010, 7, 9, 15, 0, 0);
foreach (var task in project.EnumerateAllChildTasks())
{
    Console.WriteLine("{0} - {1}", task.Name, task.Status);
}
```

### 또 보기

* enum [TaskStatus](../../taskstatus/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


