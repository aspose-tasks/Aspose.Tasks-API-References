---
title: "ProjectServerSaveOptions.Timeout"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ProjectServerSaveOptions. Obtiene o establece el tiempo de espera utilizado al esperar el procesamiento de la solicitud de guardado de proyecto por el servicio de procesamiento de colas de Project Servers. El valor predeterminado para esta propiedad es 1 minuto."
type: docs
weight: 50
url: /es/net/aspose.tasks/projectserversaveoptions/timeout/
---
## ProjectServerSaveOptions.Timeout property

Obtiene o establece el tiempo de espera utilizado al esperar el procesamiento de la solicitud de guardado de proyecto por el servicio de procesamiento de colas de Project Server. El valor predeterminado de esta propiedad es 1 minuto.

```csharp
public TimeSpan Timeout { get; set; }
```

## Observaciones

El tiempo de procesamiento puede ser mayor para proyectos grandes o en caso de que la instancia de Project Server esté demasiado ocupada respondiendo a otras solicitudes.

## Ejemplos

Muestra cómo actualizar un proyecto en Microsoft Project Online y controlar el valor del tiempo de espera de guardado.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
try
{
    var manager = new ProjectServerManager(credentials);

    ProjectInfo projectInfo = null;
    foreach (var info in manager.GetProjectList())
    {
        if (info.Name == "My project")
        {
            projectInfo = info;
        }
    }

    if (projectInfo == null)
    {
        Console.WriteLine("Project 'My project' not found in working store of Project Online account.");
        return;
    }

    var project = manager.GetProject(projectInfo.Id);
    project.Set(Prj.FinishDate, new DateTime(2020, 03, 01));

    var task = project.RootTask.Children.Add("New task");
    task.Set(Tsk.Start, new DateTime(2020, 02, 26));
    task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));

    var options = new ProjectServerSaveOptions { Timeout = TimeSpan.FromMinutes(5) };

    manager.UpdateProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine("Failed to update the project. Error: " + ex);
}
```

### Ver también

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


