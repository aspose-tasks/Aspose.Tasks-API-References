---
title: "ProjectServerSaveOptions.ProjectGuid"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ProjectServerSaveOptions. Ottiene o imposta l'identificatore univoco di un progetto. Deve essere univoco all'interno dell'istanza di Project Server Project Online"
type: docs
weight: 30
url: /it/net/aspose.tasks/projectserversaveoptions/projectguid/
---
## ProjectServerSaveOptions.ProjectGuid property

Ottiene o imposta l'identificatore univoco di un progetto. Deve essere univoco all'interno dell'istanza di Project Server \\ Project Online.

```csharp
public Guid ProjectGuid { get; set; }
```

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

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


