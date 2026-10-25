---
title: "TasksLoggedException.Operation"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TasksLoggedException 속성. 예외 작업 정보를 가져옵니다"
type: docs
weight: 20
url: /ko/net/aspose.tasks/tasksloggedexception/operation/
---
## TasksLoggedException.Operation property

예외 작업 정보를 가져옵니다.

```csharp
public string Operation { get; }
```

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

* class [TasksLoggedException](../)
* namespace [Aspose.Tasks](../../tasksloggedexception/)
* assembly [Aspose.Tasks](../../../)


