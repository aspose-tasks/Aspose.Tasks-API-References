---
title: "클래스 TasksException"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TasksException 클래스. 표준 내부 예외 유형을 나타냅니다."
type: docs
weight: 2520
url: /ko/net/aspose.tasks/tasksexception/
---
## TasksException class

표준 내부 예외 유형을 나타냅니다.

```csharp
public class TasksException : ApplicationException
```

## 예제

손상된 프로젝트 구조를 감지하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// 프로젝트 구조를 확인합니다.
// 프로젝트 구조가 올바르지 않을 경우 <see cref="TasksException">가 발생합니다.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


