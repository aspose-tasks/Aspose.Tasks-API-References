---
title: "ProjectInfo.Id"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectInfo eigenschap. Haalt de unieke identifier van het project op"
type: docs
weight: 40
url: /nl/net/aspose.tasks/projectinfo/id/
---
## ProjectInfo.Id property

Haalt de unieke identifier van het project op.

```csharp
public Guid Id { get; }
```

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

* class [ProjectInfo](../)
* namespace [Aspose.Tasks](../../projectinfo/)
* assembly [Aspose.Tasks](../../../)


