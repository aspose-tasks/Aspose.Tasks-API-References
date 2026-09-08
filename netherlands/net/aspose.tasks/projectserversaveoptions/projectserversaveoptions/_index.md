---
title: "ProjectServerSaveOptions.ProjectServerSaveOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectServerSaveOptions-constructeur. Initialiseert een nieuw exemplaar van de ProjectServerSaveOptions-klasse."
type: docs
weight: 10
url: /nl/net/aspose.tasks/projectserversaveoptions/projectserversaveoptions/
---
## ProjectServerSaveOptions constructor

Initialiseert een nieuw exemplaar van de [`ProjectServerSaveOptions`](../) klasse.

```csharp
public ProjectServerSaveOptions()
```

## Voorbeelden

Toont hoe de &lt;see cref="Aspose.Tasks.ProjectServerSaveOptions" /&gt;-opties te gebruiken om een nieuw project te maken in een on‑premise‑instantie van Project Server.

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

### Zie ook

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


