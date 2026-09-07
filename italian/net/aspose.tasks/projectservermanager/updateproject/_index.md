---
title: "ProjectServerManager.UpdateProject"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ProjectServerManager. Aggiorna il progetto esistente nell'istanza Project Server/Project Online usando le opzioni di salvataggio predefinite. Il progetto esistente verrà sovrascritto"
type: docs
weight: 70
url: /it/net/aspose.tasks/projectservermanager/updateproject/
---
## UpdateProject(Project) {#updateproject}

Aggiorna il progetto esistente nell'istanza di Project Server\Project Online utilizzando le opzioni di salvataggio predefinite. Il progetto esistente verrà sovrascritto.

```csharp
public void UpdateProject(Project project)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| progetto | Project | Il progetto da salvare nell'istanza Project Server\Project Online. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | In caso di errore di comunicazione o di errore restituito da un server. |

## Osservazioni

La proprietà 'project.Get(Prj.Guid)' del progetto dovrebbe essere un GUID valido di un progetto che esiste nell'account Project Server \ Project Online.

## Esempi

In questo esempio il progetto viene caricato dall'account Project Online, modificato e salvato nuovamente nell'account Project Online.

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

Mostra come aggiornare un progetto su Microsoft Project Online.

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

### Vedi anche

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## UpdateProject(Project, ProjectServerSaveOptions) {#updateproject_1}

Aggiorna il progetto esistente nell'istanza di Project Server\Project Online utilizzando le opzioni di salvataggio specificate. Il progetto esistente verrà sovrascritto.

```csharp
public void UpdateProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| progetto | Project | Il progetto da salvare nell'istanza Project Server\Project Online. |
| saveOptions | ProjectServerSaveOptions | Istanza della classe [`ProjectServerSaveOptions`](../../projectserversaveoptions/). |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | In caso di errore di comunicazione o di errore restituito da un server. |

## Osservazioni

saveOptions.ProjectGuid dovrebbe essere impostato su un GUID di un progetto che esiste nell'istanza Project Server\ Project Online.

## Esempi

In questo esempio il progetto viene caricato dall'account Project Online, modificato e salvato nuovamente nell'account Project Online.

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

Mostra come aggiornare un progetto su Microsoft Project Online utilizzando le opzioni di salvataggio di Project Server.

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

### Vedi anche

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


