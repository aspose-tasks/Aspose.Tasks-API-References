---
title: "ProjectServerSaveOptions.PollingInterval"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ProjectServerSaveOptions. Obtiene o establece el intervalo entre solicitudes de estado de trabajos en cola. El valor predeterminado es 2 segundos."
type: docs
weight: 20
url: /es/net/aspose.tasks/projectserversaveoptions/pollinginterval/
---
## ProjectServerSaveOptions.PollingInterval property

Obtiene o establece el intervalo entre solicitudes de estado de trabajos en cola. El valor predeterminado es 2 segundos.

```csharp
public TimeSpan PollingInterval { get; set; }
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


