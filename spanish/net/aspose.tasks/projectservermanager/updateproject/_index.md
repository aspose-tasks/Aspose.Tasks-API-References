---
title: "ProjectServerManager.UpdateProject"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ProjectServerManager. Actualiza el proyecto existente en la instancia de Project Server/Project Online usando las opciones de guardado predeterminadas. El proyecto existente será sobrescrito."
type: docs
weight: 70
url: /es/net/aspose.tasks/projectservermanager/updateproject/
---
## UpdateProject(Project) {#updateproject}

Actualiza el proyecto existente en la instancia de Project Server\\Project Online usando las opciones de guardado predeterminadas. El proyecto existente será sobrescrito.

```csharp
public void UpdateProject(Project project)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| project | Project | El proyecto a guardar en la instancia de Project Server\\Project Online. |

### Excepciones

| excepción | condición |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | En caso de error de comunicación o error devuelto por un servidor. |

## Observaciones

La propiedad del proyecto 'project.Get(Prj.Guid)' debe ser un GUID válido de un proyecto que exista en la cuenta de Project Server \\ instancia de Project Online.

## Ejemplos

En este ejemplo el proyecto se carga desde la cuenta de Project Online, se modifica y se guarda nuevamente en la cuenta de Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project);
```

Muestra cómo actualizar un proyecto en Microsoft Project Online.

```csharp
const string URL = "https://contoso.sharepoint.com/sites/pwa";
const string Domain = "CONTOSO.COM";
const string UserName = "Administrator";
const string Password = "MyPassword";

var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
try
{
    var manager = new ProjectServerManager(projectServerCredentials);

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

    manager.UpdateProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine("Failed to update the project. Error: " + ex);
}
```

### Ver también

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## UpdateProject(Project, ProjectServerSaveOptions) {#updateproject_1}

Actualiza el proyecto existente en la instancia de Project Server\\Project Online usando las opciones de guardado especificadas. El proyecto existente será sobrescrito.

```csharp
public void UpdateProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| project | Project | El proyecto a guardar en la instancia de Project Server\\Project Online. |
| saveOptions | ProjectServerSaveOptions | Instancia de la clase [`ProjectServerSaveOptions`](../../projectserversaveoptions/). |

### Excepciones

| excepción | condición |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | En caso de error de comunicación o error devuelto por un servidor. |

## Observaciones

saveOptions.ProjectGuid debe establecerse con el GUID de un proyecto que exista en la instancia de Project Server\\ Project Online.

## Ejemplos

En este ejemplo el proyecto se carga desde la cuenta de Project Online, se modifica y se guarda nuevamente en la cuenta de Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project, new ProjectServerSaveOptions
{
    ProjectGuid = projectGuid
});
```

Muestra cómo actualizar un proyecto en Microsoft Project Online utilizando las opciones de guardado de Project Server.

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

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


