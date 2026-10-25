---
title: "Clase ProjectOnlineException"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.ProjectOnlineException. Representa una excepción que se lanza cuando se encuentran errores durante la interacción con una instancia de Project Online o Project Server"
type: docs
weight: 1480
url: /es/net/aspose.tasks/projectonlineexception/
---
## ProjectOnlineException class

Representa una excepción que se lanza cuando se encuentran errores durante la interacción con una instancia de Project Online o Project Server.

```csharp
public class ProjectOnlineException : TasksException
```

## Ejemplos

Muestra cómo capturar la excepción al leer un proyecto desde MS Project Online.

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

### Ver también

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


