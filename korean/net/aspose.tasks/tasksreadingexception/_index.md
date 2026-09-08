---
title: "클래스 TasksReadingException"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TasksReadingException 클래스. 표준 내부 읽기 예외 유형을 나타냅니다"
type: docs
weight: 2540
url: /ko/net/aspose.tasks/tasksreadingexception/
---
## TasksReadingException class

표준 내부 읽기 예외 유형을 나타냅니다.

```csharp
public class TasksReadingException : TasksLoggedException
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | 예외 로그 정보를 가져옵니다. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | 예외 작업 정보를 가져옵니다. |

## 예제

프로젝트의 읽기/쓰기 예외를 처리하는 방법을 보여줍니다.

```csharp
try
{
    var project = new Project(DataDir + "project.mpp");
    project.Save(OutDir + "HandleExceptions_out.mpp", SaveFileFormat.Mpp);
}
catch (TasksReadingException ex)
{
    Console.WriteLine("Message: ");
    Console.WriteLine(ex.Message);
    Console.WriteLine("Log: ");
    Console.WriteLine(ex.LogText);
    if (ex.InnerException != null)
    {
        Console.WriteLine("Inner exception message: ");
        Console.WriteLine(ex.InnerException.Message);
    }
}
```

### 또 보기

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


