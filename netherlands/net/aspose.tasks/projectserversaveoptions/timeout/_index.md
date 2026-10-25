---
title: "ProjectServerSaveOptions.Timeout"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectServerSaveOptions-eigenschap. Haalt op of stelt de time-out in die wordt gebruikt bij het wachten op de verwerking van een opslaan-projectverzoek door de wachtrijverwerkingsservice van Project Servers. De standaardwaarde voor deze eigenschap is 1 minuut"
type: docs
weight: 50
url: /nl/net/aspose.tasks/projectserversaveoptions/timeout/
---
## ProjectServerSaveOptions.Timeout property

Haalt op of stelt de time-out in die wordt gebruikt bij het wachten op de verwerking van een opslaan‑projectverzoek door de wachtrijverwerkingsservice van Project Server. De standaardwaarde voor deze eigenschap is 1 minuut.

```csharp
public TimeSpan Timeout { get; set; }
```

## Opmerkingen

De verwerkingstijd kan langer zijn voor grote projecten of wanneer de Project Server-instantie te druk is met het beantwoorden van andere verzoeken.

## Voorbeelden

Toont hoe een project bij te werken op Microsoft Project Online en de time-outwaarde voor opslaan te regelen.

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

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


