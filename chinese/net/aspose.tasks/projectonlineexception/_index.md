---
title: "类 ProjectOnlineException"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ProjectOnlineException 类。表示在与 Project Online 或 Project Server 实例交互时发现错误时抛出的异常"
type: docs
weight: 1480
url: /zh/net/aspose.tasks/projectonlineexception/
---
## ProjectOnlineException class

表示在与 Project Online 或 Project Server 实例交互时发现错误而抛出的异常。

```csharp
public class ProjectOnlineException : TasksException
```

## 示例

展示如何在从 MS Project Online 读取项目时捕获异常。

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

### 另见

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


