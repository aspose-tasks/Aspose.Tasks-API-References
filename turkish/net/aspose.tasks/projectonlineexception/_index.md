---
title: "Sınıf ProjectOnlineException"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ProjectOnlineException sınıfı. Project Online veya Project Server örneğiyle etkileşim sırasında hatalar bulunduğunda atılan bir istisnayı temsil eder."
type: docs
weight: 1480
url: /tr/net/aspose.tasks/projectonlineexception/
---
## ProjectOnlineException class

Project Online veya Project Server örneğiyle etkileşim sırasında hatalar bulunduğunda atılan bir istisna temsil eder.

```csharp
public class ProjectOnlineException : TasksException
```

## Örnekler

MS Project Online'dan bir proje okunurken istisnanın nasıl yakalanacağını gösterir.

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

### Ayrıca Bakınız

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


