---
title: "ProjectServerSaveOptions.Timeout"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ProjectServerSaveOptions. Ottiene o imposta il timeout utilizzato durante l'attesa dell'elaborazione della richiesta di salvataggio del progetto da parte del servizio di elaborazione della coda di Project Server. Il valore predefinito per questa proprietà è 1 minuto"
type: docs
weight: 50
url: /it/net/aspose.tasks/projectserversaveoptions/timeout/
---
## ProjectServerSaveOptions.Timeout property

Ottiene o imposta il timeout utilizzato durante l'attesa dell'elaborazione della richiesta di salvataggio del progetto da parte del servizio di elaborazione della coda di Project Server. Il valore predefinito per questa proprietà è 1 minuto.

```csharp
public TimeSpan Timeout { get; set; }
```

## Osservazioni

Il tempo di elaborazione può essere più lungo per progetti di grandi dimensioni o nel caso in cui l'istanza di Project Server sia troppo occupata a rispondere ad altre richieste.

## Esempi

Mostra come aggiornare un progetto su Microsoft Project Online e controllare il valore del timeout di salvataggio.

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

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


