---
title: "Class ProjectOnlineException"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ProjectOnlineException class. Vertegenwoordigt een uitzondering die wordt gegooid wanneer er fouten worden gevonden tijdens interactie met een Project Online- of Project Server‑instantie."
type: docs
weight: 1480
url: /nl/net/aspose.tasks/projectonlineexception/
---
## ProjectOnlineException class

Stelt een uitzondering voor die wordt gegooid wanneer er fouten worden gevonden tijdens interactie met een Project Online- of Project Server‑instance.

```csharp
public class ProjectOnlineException : TasksException
```

## Voorbeelden

Toont hoe een uitzondering op te vangen tijdens het lezen van een project vanuit MS Project Online.

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

### Zie ook

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


