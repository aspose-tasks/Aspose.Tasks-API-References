---
title: "ProjectServerSaveOptions.ProjectServerSaveOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de ProjectServerSaveOptions. Inicializa una nueva instancia de la clase ProjectServerSaveOptions."
type: docs
weight: 10
url: /es/net/aspose.tasks/projectserversaveoptions/projectserversaveoptions/
---
## ProjectServerSaveOptions constructor

Inicializa una nueva instancia de la clase [`ProjectServerSaveOptions`](../).

```csharp
public ProjectServerSaveOptions()
```

## Ejemplos

Muestra cómo usar las opciones &lt;see cref="Aspose.Tasks.ProjectServerSaveOptions" /&gt; para crear un nuevo proyecto en una instancia local de Project Server.

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
    var options = new ProjectServerSaveOptions
                      {
                          ProjectGuid = Guid.NewGuid(),
                          ProjectName = "New project",
                          Timeout = TimeSpan.FromMinutes(5),
                          PollingInterval = TimeSpan.FromSeconds(3)
                      };

    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Ver también

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


