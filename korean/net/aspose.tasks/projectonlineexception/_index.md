---
title: "클래스 ProjectOnlineException"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ProjectOnlineException 클래스. Project Online 또는 Project Server 인스턴스와 상호 작용 중에 오류가 발견될 때 발생하는 예외를 나타냅니다."
type: docs
weight: 1480
url: /ko/net/aspose.tasks/projectonlineexception/
---
## ProjectOnlineException class

Project Online 또는 Project Server 인스턴스와 상호 작용 중 오류가 발견될 때 발생하는 예외를 나타냅니다.

```csharp
public class ProjectOnlineException : TasksException
```

## 예제

MS Project Online에서 프로젝트를 읽는 동안 예외를 잡는 방법을 보여줍니다.

```csharp
try
{
    const string URL = "https://project_server.local/sites/pwa";
    const string Domain = "CONTOSO.COM";
    const string UserName = "Administrator";
    const string Password = "MyPassword";

    var project = new Project(DataDir + @"Project1.mpp");

    var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
    var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
    var manager = new ProjectServerManager(projectServerCredentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 또 보기

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


