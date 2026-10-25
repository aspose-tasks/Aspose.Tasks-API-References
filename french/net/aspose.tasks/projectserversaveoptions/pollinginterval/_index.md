---
title: "ProjectServerSaveOptions.PollingInterval"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ProjectServerSaveOptions. Obtient ou définit l'intervalle entre les requêtes d'état des travaux de la file d'attente. La valeur par défaut est de 2 secondes"
type: docs
weight: 20
url: /fr/net/aspose.tasks/projectserversaveoptions/pollinginterval/
---
## ProjectServerSaveOptions.PollingInterval property

Obtient ou définit l'intervalle entre les requêtes d'état des travaux de la file d'attente. La valeur par défaut est de 2 secondes.

```csharp
public TimeSpan PollingInterval { get; set; }
```

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

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


