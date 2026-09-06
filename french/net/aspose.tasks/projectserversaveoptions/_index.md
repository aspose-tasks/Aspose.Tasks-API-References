---
title: "Classe ProjectServerSaveOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.ProjectServerSaveOptions. Permet de spécifier des options supplémentaires lorsque le projet est enregistré sur Project Server ou Project Online"
type: docs
weight: 1510
url: /fr/net/aspose.tasks/projectserversaveoptions/
---
## ProjectServerSaveOptions class

Permet de spécifier des options supplémentaires lorsque le projet est enregistré sur Project Server ou Project Online.

```csharp
public sealed class ProjectServerSaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ProjectServerSaveOptions](projectserversaveoptions/)() | Initialise une nouvelle instance de la classe `ProjectServerSaveOptions`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [PollingInterval](../../aspose.tasks/projectserversaveoptions/pollinginterval/) { get; set; } | Obtient ou définit l'intervalle entre les requêtes d'état des travaux de la file d'attente. La valeur par défaut est de 2 secondes. |
| [ProjectGuid](../../aspose.tasks/projectserversaveoptions/projectguid/) { get; set; } | Obtient ou définit l'identifiant unique d'un projet. Il doit être unique au sein de l'instance Project Server \ Project Online. |
| [ProjectName](../../aspose.tasks/projectserversaveoptions/projectname/) { get; set; } | Obtient ou définit le nom d'un projet qui est affiché dans la liste des projets Project Server \ Project Online. Il doit être unique au sein de l'instance Project Server \ Project Online. Si la valeur est omise, la valeur de la propriété Prj.Name sera utilisée à la place. |
| [Timeout](../../aspose.tasks/projectserversaveoptions/timeout/) { get; set; } | Obtient ou définit le délai d'attente utilisé lors de l'attente du traitement de la demande d'enregistrement du projet par le service de traitement de la file d'attente de Project Server. La valeur par défaut de cette propriété est d'une minute. |

## Exemples

Montre comment utiliser les options &lt;see cref="Aspose.Tasks.ProjectServerSaveOptions" /&gt; pour créer un nouveau projet dans une instance sur site de Project Server.

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

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


