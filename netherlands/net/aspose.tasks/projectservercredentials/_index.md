---
title: "Klasse ProjectServerCredentials"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ProjectServerCredentials-klasse. Inloggegevens die worden gebruikt om verbinding te maken met Project Online of een on-premise instantie van Project Server"
type: docs
weight: 1490
url: /nl/net/aspose.tasks/projectservercredentials/
---
## ProjectServerCredentials class

Inloggegevens die worden gebruikt om verbinding te maken met Project Online of een on‑premise‑instance van Project Server.

```csharp
public sealed class ProjectServerCredentials
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [ProjectServerCredentials](projectservercredentials/#constructor)(string, NetworkCredential) | Initialiseert een nieuw exemplaar van de `ProjectServerCredentials`-klasse met de URL van het Project Web Access-eindpunt en netwerkinloggegevens. |
| [ProjectServerCredentials](projectservercredentials/#constructor_1)(string, string) | Initialiseert een nieuw exemplaar van de `ProjectServerCredentials`-klasse met de URL van de SharePoint-site en een geldig SPOIDCRL-autorisatietoken voor de PWA (Project Web Access)-site van SharePoint. |
| [ProjectServerCredentials](projectservercredentials/#constructor_2)(string, string, string) | Initialiseert een nieuw exemplaar van de `ProjectServerCredentials`-klasse met de URL van de SharePoint-site, gebruikersnaam en wachtwoord. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [AuthToken](../../aspose.tasks/projectservercredentials/authtoken/) { get; } | Haalt het autorisatietoken op voor de SharePoint‑instantie. |
| [SiteUrl](../../aspose.tasks/projectservercredentials/siteurl/) { get; } | Haalt de URL van PWA op bij de SharePoint-site of de URL van een on-premise Project Server op. Bijvoorbeeld, https://your_company_name.sharepoint.com/sites/pwa\"; |
| [UserName](../../aspose.tasks/projectservercredentials/username/) { get; } | Haalt de gebruikersnaam op voor de SharePoint-site. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [ToString](../../aspose.tasks/projectservercredentials/tostring/)() | Retourneert een tekenreeksrepresentatie van deze instantie. |

## Voorbeelden

Toont hoe projectserverreferenties te gebruiken om een lijst met projecten op te halen uit Microsoft Project Online.

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var newProject = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(newProject);

    IEnumerable<ProjectInfo> list = manager.GetProjectList();

    foreach (var info in list)
    {
        var project = manager.GetProject(info.Id);
        Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
        Console.WriteLine("Resources count: {0}", project.Resources.Count);
    }
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


