---
title: "Classe ProjectOnlineException"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.ProjectOnlineException. Rappresenta un'eccezione che viene sollevata quando si riscontrano errori durante l'interazione con un'istanza di Project Online o Project Server"
type: docs
weight: 1480
url: /it/net/aspose.tasks/projectonlineexception/
---
## ProjectOnlineException class

Rappresenta un'eccezione che viene lanciata quando vengono trovati errori durante l'interazione con l'istanza di Project Online o Project Server.

```csharp
public class ProjectOnlineException : TasksException
```

## Esempi

Mostra come catturare l'eccezione durante la lettura di un progetto da MS Project Online.

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

### Vedi anche

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


