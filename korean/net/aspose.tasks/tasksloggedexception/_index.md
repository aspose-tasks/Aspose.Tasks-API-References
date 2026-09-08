---
title: "클래스 TasksLoggedException"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TasksLoggedException 클래스. 표준 내부 예외 유형을 나타냅니다."
type: docs
weight: 2530
url: /ko/net/aspose.tasks/tasksloggedexception/
---
## TasksLoggedException class

표준 내부 예외 유형을 나타냅니다.

```csharp
public class TasksLoggedException : ApplicationException
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | 예외 로그 정보를 가져옵니다. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | 예외 작업 정보를 가져옵니다. |

## 예제

MPP 내보내기와 관련된 문제를 확인하기 위해 로그 텍스트와 예외 유형을 읽는 방법을 보여줍니다.

```csharp
try
{
    var project = new Project(DataDir + "PrintTaskWritingException.mpp");

    // 프로젝트를 MPP 파일로 내보냅니다.
    project.Save(OutDir + "PrintTaskWritingException_out.MPP", SaveFileFormat.Mpp);
}
catch (TasksWritingException ex)
{
    Console.WriteLine("Exception Operation: " + ex.Operation);
    Console.WriteLine("Exception Log Text: ");
    Console.WriteLine(ex.LogText);
}
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


