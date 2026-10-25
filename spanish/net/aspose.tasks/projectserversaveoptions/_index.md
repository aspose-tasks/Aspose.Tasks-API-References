---
title: "Clase ProjectServerSaveOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.ProjectServerSaveOptions. Permite especificar opciones adicionales cuando el proyecto se guarda en Project Server o Project Online."
type: docs
weight: 1510
url: /es/net/aspose.tasks/projectserversaveoptions/
---
## ProjectServerSaveOptions class

Permite especificar opciones adicionales cuando el proyecto se guarda en Project Server o Project Online.

```csharp
public sealed class ProjectServerSaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ProjectServerSaveOptions](projectserversaveoptions/)() | Inicializa una nueva instancia de la clase `ProjectServerSaveOptions`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [PollingInterval](../../aspose.tasks/projectserversaveoptions/pollinginterval/) { get; set; } | Obtiene o establece el intervalo entre solicitudes de estado de trabajos en cola. El valor predeterminado es 2 segundos. |
| [ProjectGuid](../../aspose.tasks/projectserversaveoptions/projectguid/) { get; set; } | Obtiene o establece el identificador único de un proyecto. Debe ser único dentro de la instancia de Project Server \ Project Online. |
| [ProjectName](../../aspose.tasks/projectserversaveoptions/projectname/) { get; set; } | Obtiene o establece el nombre de un proyecto que se muestra en la lista de proyectos de Project Server \ Project Online. Debe ser único dentro de la instancia de Project Server \ Project Online. Si el valor se omite, se utilizará el valor de la propiedad Prj.Name. |
| [Timeout](../../aspose.tasks/projectserversaveoptions/timeout/) { get; set; } | Obtiene o establece el tiempo de espera utilizado al esperar el procesamiento de la solicitud de guardado de proyecto por el servicio de procesamiento de colas de Project Server. El valor predeterminado de esta propiedad es 1 minuto. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


