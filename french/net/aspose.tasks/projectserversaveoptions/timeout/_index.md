---
title: "ProjectServerSaveOptions.Timeout"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ProjectServerSaveOptions. Obtient ou définit le délai d'attente utilisé lors de l'attente du traitement d'une requête de sauvegarde de projet par le service de traitement de la file d'attente de Project Servers. La valeur par défaut de cette propriété est de 1 minute."
type: docs
weight: 50
url: /fr/net/aspose.tasks/projectserversaveoptions/timeout/
---
## ProjectServerSaveOptions.Timeout property

Obtient ou définit le délai d'attente utilisé lors de l'attente du traitement de la demande d'enregistrement du projet par le service de traitement de la file d'attente de Project Server. La valeur par défaut de cette propriété est d'une minute.

```csharp
public TimeSpan Timeout { get; set; }
```

## Remarques

Le temps de traitement peut être plus long pour les grands projets ou dans le cas où l'instance Project Server est trop occupée à répondre à d'autres requêtes.

## Exemples

Montre comment mettre à jour un projet sur Microsoft Project Online et contrôler la valeur du délai d'attente de sauvegarde.

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

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


