---
title: "Klasse ProjectInfo"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ProjectInfo klasse. Korte informatie over het gepubliceerde project beschikbaar op Project Online"
type: docs
weight: 1470
url: /nl/net/aspose.tasks/projectinfo/
---
## ProjectInfo class

Korte info over het gepubliceerde project dat beschikbaar is op Project Online.

```csharp
public sealed class ProjectInfo
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [ProjectInfo](projectinfo/)() | Initialiseert een nieuw exemplaar van de `ProjectInfo` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CreatedDate](../../aspose.tasks/projectinfo/createddate/) { get; } | Haalt de datum en tijd op waarop het project is aangemaakt. |
| [Description](../../aspose.tasks/projectinfo/description/) { get; } | Haalt de beschrijving van het project op. |
| [Id](../../aspose.tasks/projectinfo/id/) { get; } | Haalt de unieke identifier van het project op. |
| [IsCheckedOut](../../aspose.tasks/projectinfo/ischeckedout/) { get; } | Haalt een waarde op die aangeeft of het project is uitgecheckt. |
| [LastPublishedDate](../../aspose.tasks/projectinfo/lastpublisheddate/) { get; } | Haalt de meest recente datum op waarop het project is gepubliceerd. |
| [LastSavedDate](../../aspose.tasks/projectinfo/lastsaveddate/) { get; } | Haalt de meest recente datum op waarop het project is opgeslagen. |
| [Name](../../aspose.tasks/projectinfo/name/) { get; } | Haalt de naam van het project op. |

## Voorbeelden

Toont hoe informatie over projecten te lezen is vanuit Project Online.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

var reader = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = reader.GetProjectList();

// lees projectinformatie
Console.WriteLine("Print information about projects:");
foreach (var info in list)
{
    Console.WriteLine("Id: " + info.Id);
    Console.WriteLine("Name: " + info.Name);
    Console.WriteLine("Description: " + info.Description);
    Console.WriteLine("Created Date: " + info.CreatedDate);
    Console.WriteLine("Last Saved Date: " + info.LastSavedDate);
    Console.WriteLine("Last Published Date: " + info.LastPublishedDate);
    Console.WriteLine("Is Checked Out: " + info.IsCheckedOut);
}
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


