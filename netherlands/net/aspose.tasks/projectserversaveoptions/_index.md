---
title: "Klasse ProjectServerSaveOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ProjectServerSaveOptions klasse. Stelt toe extra opties op te geven wanneer een project wordt opgeslagen naar Project Server of Project Online."
type: docs
weight: 1510
url: /nl/net/aspose.tasks/projectserversaveoptions/
---
## ProjectServerSaveOptions class

Staat toe extra opties op te geven wanneer een project wordt opgeslagen naar Project Server of Project Online.

```csharp
public sealed class ProjectServerSaveOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [ProjectServerSaveOptions](projectserversaveoptions/)() | Initialiseert een nieuw exemplaar van de `ProjectServerSaveOptions` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [PollingInterval](../../aspose.tasks/projectserversaveoptions/pollinginterval/) { get; set; } | Haalt op of stelt het interval tussen wachtrijtaakstatusverzoeken in. De standaardwaarde is 2 seconden. |
| [ProjectGuid](../../aspose.tasks/projectserversaveoptions/projectguid/) { get; set; } | Haalt op of stelt de unieke identifier van een project in. Moet uniek zijn binnen de Project Server \ Project Online‑instantie. |
| [ProjectName](../../aspose.tasks/projectserversaveoptions/projectname/) { get; set; } | Haalt op of stelt de naam van een project in die wordt weergegeven in de Project Server \ Project Online‑projectenlijst. Moet uniek zijn binnen de Project Server \ Project Online‑instantie. Als de waarde wordt weggelaten, wordt de waarde van de Prj.Name‑eigenschap gebruikt. |
| [Timeout](../../aspose.tasks/projectserversaveoptions/timeout/) { get; set; } | Haalt op of stelt de time-out in die wordt gebruikt bij het wachten op de verwerking van een opslaan‑projectverzoek door de wachtrijverwerkingsservice van Project Server. De standaardwaarde voor deze eigenschap is 1 minuut. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


