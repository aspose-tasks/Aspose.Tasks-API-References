---
title: "ProjectInfo.CreatedDate"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ProjectInfo. Obtient la date et l'heure de création du projet"
type: docs
weight: 20
url: /fr/net/aspose.tasks/projectinfo/createddate/
---
## ProjectInfo.CreatedDate property

Obtient la date et l'heure de création du projet.

```csharp
public DateTime CreatedDate { get; }
```

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

* class [ProjectInfo](../)
* namespace [Aspose.Tasks](../../projectinfo/)
* assembly [Aspose.Tasks](../../../)


