---
title: "ProjectServerManager.UpdateProject"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ProjectServerManager. Met à jour le projet existant dans l'instance Project Server/Project Online en utilisant les options d’enregistrement par défaut. Le projet existant sera écrasé"
type: docs
weight: 70
url: /fr/net/aspose.tasks/projectservermanager/updateproject/
---
## UpdateProject(Project) {#updateproject}

Met à jour le projet existant dans une instance de Project Server\Project Online en utilisant les options d’enregistrement par défaut. Le projet existant sera écrasé.

```csharp
public void UpdateProject(Project project)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| project | Project | Le projet à enregistrer dans l'instance Project Server\Project Online. |

### Exceptions

| exception | condition |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | En cas d'erreur de communication ou d'erreur renvoyée par le serveur. |

## Remarques

La propriété du projet 'project.Get(Prj.Guid)' doit être un guid valide d'un projet qui existe dans le compte Project Server \ Project Online.

## Exemples

Dans cet exemple, le projet est chargé depuis le compte Project Online, modifié et enregistré à nouveau dans le compte Project Online.

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

Montre comment mettre à jour un projet sur Microsoft Project Online.

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

### Voir aussi

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## UpdateProject(Project, ProjectServerSaveOptions) {#updateproject_1}

Met à jour le projet existant dans une instance de Project Server\Project Online en utilisant les options d’enregistrement spécifiées. Le projet existant sera écrasé.

```csharp
public void UpdateProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| project | Project | Le projet à enregistrer dans l'instance Project Server\Project Online. |
| saveOptions | ProjectServerSaveOptions | Instance de la classe [`ProjectServerSaveOptions`](../../projectserversaveoptions/). |

### Exceptions

| exception | condition |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | En cas d'erreur de communication ou d'erreur renvoyée par le serveur. |

## Remarques

saveOptions.ProjectGuid doit être défini sur un guid d'un projet qui existe sur l'instance Project Server\ Project Online.

## Exemples

Dans cet exemple, le projet est chargé depuis le compte Project Online, modifié et enregistré à nouveau dans le compte Project Online.

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

Montre comment mettre à jour un projet sur Microsoft Project Online en utilisant les options d'enregistrement du Project Server.

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

### Voir aussi

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


