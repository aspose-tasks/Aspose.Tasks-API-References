---
title: "ProjectServerManager.UpdateProject"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectServerManager-methode. Werkt een bestaand project bij in een Project Server/Project Online‑instantie met de standaard opslaan‑opties. Het bestaande project wordt overschreven."
type: docs
weight: 70
url: /nl/net/aspose.tasks/projectservermanager/updateproject/
---
## UpdateProject(Project) {#updateproject}

Werk een bestaand project bij in Project Server\Project Online‑instantie met de standaard opslagopties. Het bestaande project wordt overschreven.

```csharp
public void UpdateProject(Project project)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| project | Project | Het project om op te slaan naar de Project Server\Project Online‑instantie. |

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | In geval van een communicatiefout of een fout die door een server wordt geretourneerd. |

## Opmerkingen

De eigenschap 'project.Get(Prj.Guid)' van het project moet een geldige GUID zijn van een project dat bestaat in een Project Server‑account \ Project Online‑instantie.

## Voorbeelden

In dit voorbeeld wordt het project geladen vanuit een Project Online‑account, aangepast en terug opgeslagen naar het Project Online‑account.

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

Toont hoe een project bij te werken op Microsoft Project Online.

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

### Zie ook

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## UpdateProject(Project, ProjectServerSaveOptions) {#updateproject_1}

Werk een bestaand project bij in Project Server\Project Online‑instantie met de opgegeven opslagopties. Het bestaande project wordt overschreven.

```csharp
public void UpdateProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| project | Project | Het project om op te slaan naar de Project Server\Project Online‑instantie. |
| saveOptions | ProjectServerSaveOptions | Instantie van de [`ProjectServerSaveOptions`](../../projectserversaveoptions/)‑klasse. |

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | In geval van een communicatiefout of een fout die door een server wordt geretourneerd. |

## Opmerkingen

saveOptions.ProjectGuid moet worden ingesteld op een GUID van een project dat bestaat op een Project Server\ Project Online‑instantie.

## Voorbeelden

In dit voorbeeld wordt het project geladen vanuit een Project Online‑account, aangepast en terug opgeslagen naar het Project Online‑account.

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

Toont hoe een project bij te werken op Microsoft Project Online met gebruik van Project Server‑opslaan‑opties.

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

### Zie ook

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


