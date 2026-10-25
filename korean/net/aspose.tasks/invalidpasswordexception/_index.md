---
title: "클래스 InvalidPasswordException"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.InvalidPasswordException 클래스. 잘못된 비밀번호로 암호 보호된 파일을 열 때 발생하는 예외 유형을 나타냅니다."
type: docs
weight: 910
url: /ko/net/aspose.tasks/invalidpasswordexception/
---
## InvalidPasswordException class

잘못된 비밀번호로 암호 보호 파일을 열 때 발생하는 예외 유형을 나타냅니다.

```csharp
public class InvalidPasswordException : TasksException
```

## 예제

암호 보호된 프로젝트 파일을 읽는 동안 &lt;see cref="InvalidPasswordException"/&gt;을 처리하는 방법을 보여줍니다.

```csharp
try
{
    var project = new Project(DataDir + "PasswordProtected.mpp");

    // 프로젝트 작업 중 ...
    Console.WriteLine("Project Name: " + project.Get(Prj.Name));
}
catch (TasksReadingException e)
{
    // 메시지는 "프로젝트가 암호로 보호되어 있습니다. 비밀번호가 제공되지 않았거나 올바르지 않습니다." 입니다.
    Console.WriteLine(e.Message);
}
```

### 또 보기

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


