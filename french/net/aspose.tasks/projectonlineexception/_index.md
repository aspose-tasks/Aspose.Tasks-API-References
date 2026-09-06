---
title: "Classe ProjectOnlineException"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.ProjectOnlineException classe. Représente une exception qui est levée lorsque des erreurs sont détectées lors de l'interaction avec une instance de Project Online ou de Project Server."
type: docs
weight: 1480
url: /fr/net/aspose.tasks/projectonlineexception/
---
## ProjectOnlineException class

Représente une exception qui est levée lorsque des erreurs sont détectées lors de l'interaction avec une instance de Project Online ou de Project Server.

```csharp
public class ProjectOnlineException : TasksException
```

## Exemples

Montre comment attraper l'exception lors de la lecture d'un projet depuis MS Project Online.

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

### Voir aussi

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


