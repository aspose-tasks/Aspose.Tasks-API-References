---
title: "Classe ProjectServerSaveOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.ProjectServerSaveOptions. Consente di specificare opzioni aggiuntive quando il progetto viene salvato su Project Server o Project Online"
type: docs
weight: 1510
url: /it/net/aspose.tasks/projectserversaveoptions/
---
## ProjectServerSaveOptions class

Consente di specificare opzioni aggiuntive quando il progetto viene salvato su Project Server o Project Online.

```csharp
public sealed class ProjectServerSaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ProjectServerSaveOptions](projectserversaveoptions/)() | Inizializza una nuova istanza della classe `ProjectServerSaveOptions`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [PollingInterval](../../aspose.tasks/projectserversaveoptions/pollinginterval/) { get; set; } | Ottiene o imposta l'intervallo tra le richieste di stato dei lavori in coda. Il valore predefinito è 2 secondi. |
| [ProjectGuid](../../aspose.tasks/projectserversaveoptions/projectguid/) { get; set; } | Ottiene o imposta l'identificatore univoco di un progetto. Deve essere univoco all'interno dell'istanza di Project Server \\ Project Online. |
| [ProjectName](../../aspose.tasks/projectserversaveoptions/projectname/) { get; set; } | Ottiene o imposta il nome di un progetto che viene visualizzato nell'elenco dei progetti di Project Server \\ Project Online. Deve essere univoco all'interno dell'istanza di Project Server \\ Project Online. Se il valore è omesso, verrà utilizzato il valore della proprietà Prj.Name. |
| [Timeout](../../aspose.tasks/projectserversaveoptions/timeout/) { get; set; } | Ottiene o imposta il timeout utilizzato durante l'attesa dell'elaborazione della richiesta di salvataggio del progetto da parte del servizio di elaborazione della coda di Project Server. Il valore predefinito per questa proprietà è 1 minuto. |

## Esempi

Mostra come utilizzare le opzioni &lt;see cref="Aspose.Tasks.ProjectServerSaveOptions" /&gt; per creare un nuovo progetto in un'istanza on-premise di Project Server.

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

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


