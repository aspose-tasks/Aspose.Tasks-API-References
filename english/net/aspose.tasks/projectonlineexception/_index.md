---
title: Class ProjectOnlineException
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ProjectOnlineException class. Represents an exception which is thrown when errors are found during interaction with Project Online or Project Server instance
type: docs
weight: 1460
url: /net/aspose.tasks/projectonlineexception/
---
## ProjectOnlineException class

Represents an exception which is thrown when errors are found during interaction with Project Online or Project Server instance.

```csharp
public class ProjectOnlineException : TasksException
```

## Examples

Shows how to catch exception while reading a project from MS Project Online.

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

### See Also

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


