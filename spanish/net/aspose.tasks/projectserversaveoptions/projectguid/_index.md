---
title: "ProjectServerSaveOptions.ProjectGuid"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ProjectServerSaveOptions. Obtiene o establece el identificador único de un proyecto. Debe ser único dentro de la instancia de Project Server Project Online."
type: docs
weight: 30
url: /es/net/aspose.tasks/projectserversaveoptions/projectguid/
---
## ProjectServerSaveOptions.ProjectGuid property

Obtiene o establece el identificador único de un proyecto. Debe ser único dentro de la instancia de Project Server \ Project Online.

```csharp
public Guid ProjectGuid { get; set; }
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


