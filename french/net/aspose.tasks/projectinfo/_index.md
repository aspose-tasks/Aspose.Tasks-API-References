---
title: "Classe ProjectInfo"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.ProjectInfo. Brève information sur le projet publié disponible sur Project Online"
type: docs
weight: 1470
url: /fr/net/aspose.tasks/projectinfo/
---
## ProjectInfo class

Brève information sur le projet publié disponible sur Project Online.

```csharp
public sealed class ProjectInfo
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ProjectInfo](projectinfo/)() | Initialise une nouvelle instance de la classe `ProjectInfo`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CreatedDate](../../aspose.tasks/projectinfo/createddate/) { get; } | Obtient la date et l'heure de création du projet. |
| [Description](../../aspose.tasks/projectinfo/description/) { get; } | Obtient la description du projet. |
| [Id](../../aspose.tasks/projectinfo/id/) { get; } | Obtient l'identifiant unique du projet. |
| [IsCheckedOut](../../aspose.tasks/projectinfo/ischeckedout/) { get; } | Obtient une valeur indiquant si le projet est extrait. |
| [LastPublishedDate](../../aspose.tasks/projectinfo/lastpublisheddate/) { get; } | Obtient la date la plus récente à laquelle le projet a été publié. |
| [LastSavedDate](../../aspose.tasks/projectinfo/lastsaveddate/) { get; } | Obtient la date la plus récente à laquelle le projet a été enregistré. |
| [Name](../../aspose.tasks/projectinfo/name/) { get; } | Obtient le nom du projet. |

## Exemples

Montre comment lire les informations sur les projets depuis Project Online.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

var reader = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = reader.GetProjectList();

// lire les informations du projet
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

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


