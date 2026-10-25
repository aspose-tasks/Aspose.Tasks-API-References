---
title: "Klasse ProjectServerManager"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ProjectServerManager klasse. De klasse die de methoden biedt om projecten te lezen en bewerkingen uit te voeren in het opgegeven Project Online‑account of in de opgegeven on‑premise Project Server‑instantie. Versies 2016 en 2019 van Project Server worden ondersteund."
type: docs
weight: 1500
url: /nl/net/aspose.tasks/projectservermanager/
---
## ProjectServerManager class

De klasse die de methoden biedt om projecten te lezen en bewerkingen uit te voeren in het opgegeven Project Online‑account of in de opgegeven on‑premise Project Server‑instance (versies 2016 en 2019 van Project Server worden ondersteund).

```csharp
public sealed class ProjectServerManager
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [ProjectServerManager](projectservermanager/)(ProjectServerCredentials) | Initialiseert een nieuwe instantie van de `ProjectServerManager`-klasse. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject)(Project) | Maakt een nieuw project aan in een Project Server\Project Online‑instantie met behulp van de standaard opslagopties. |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject_1)(Project, ProjectServerSaveOptions) | Maakt een nieuw project aan in Project Server\Project Online‑instantie met de opgegeven opslagopties. |
| [GetProject](../../aspose.tasks/projectservermanager/getproject/)(Guid) | Haalt het project met de opgegeven guid op uit het Project Online‑account \ Project Server‑instantie. |
| [GetProjectList](../../aspose.tasks/projectservermanager/getprojectlist/)() | Haalt de lijst met projecten op uit de 'Working'-opslag van het huidige Project Online‑account \ Project Server‑instantie. |
| [GetProjectRawData](../../aspose.tasks/projectservermanager/getprojectrawdata/)(Guid) | Haalt de binaire gegevens van het project op voor probleemoplossingsdoeleinden. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject)(Project) | Werk een bestaand project bij in Project Server\Project Online‑instantie met de standaard opslagopties. Het bestaande project wordt overschreven. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject_1)(Project, ProjectServerSaveOptions) | Werk een bestaand project bij in Project Server\Project Online‑instantie met de opgegeven opslagopties. Het bestaande project wordt overschreven. |

## Gebeurtenissen

| Naam | Beschrijving |
| --- | --- |
| event [ExecutingWebRequest](../../aspose.tasks/projectservermanager/executingwebrequest/) | Een gebeurtenis die wordt opgehaald wanneer het webverzoek naar de web‑API van Project Server wordt verzonden. |

## Voorbeelden

Toont hoe de Project Server‑manager te gebruiken om een nieuw project te maken met vooraf gedefinieerde opslagopties op Microsoft Project Online.

```csharp
try
{
    const string sharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(sharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    var options = new ProjectServerSaveOptions
    {
        Timeout = TimeSpan.FromSeconds(10)
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


