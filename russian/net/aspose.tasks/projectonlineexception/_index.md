---
title: "Класс ProjectOnlineException"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ProjectOnlineException. Представляет исключение, которое выбрасывается, когда обнаруживаются ошибки при взаимодействии с экземпляром Project Online или Project Server."
type: docs
weight: 1480
url: /ru/net/aspose.tasks/projectonlineexception/
---
## ProjectOnlineException class

Представляет исключение, которое выбрасывается, когда обнаруживаются ошибки при взаимодействии с экземпляром Project Online или Project Server.

```csharp
public class ProjectOnlineException : TasksException
```

## Примеры

Показывает, как перехватывать исключение при чтении проекта из MS Project Online.

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

### См. также

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


