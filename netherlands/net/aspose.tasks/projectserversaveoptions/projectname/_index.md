---
title: "ProjectServerSaveOptions.ProjectName"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectServerSaveOptions-eigenschap. Haalt op of stelt de naam van een project in dat wordt weergegeven in de Project Server Project Online-projectenlijst. Moet uniek zijn binnen de Project Server Project Online-instantie. Als de waarde wordt weggelaten, wordt de waarde van de Prj.Name-eigenschap gebruikt."
type: docs
weight: 40
url: /nl/net/aspose.tasks/projectserversaveoptions/projectname/
---
## ProjectServerSaveOptions.ProjectName property

Haalt op of stelt de naam van een project in die wordt weergegeven in de Project Server \ Project Online‑projectenlijst. Moet uniek zijn binnen de Project Server \ Project Online‑instantie. Als de waarde wordt weggelaten, wordt de waarde van de Prj.Name‑eigenschap gebruikt.

```csharp
public string ProjectName { get; set; }
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


