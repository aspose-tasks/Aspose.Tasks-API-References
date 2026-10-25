---
title: "ProjectServerManager.GetProject"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectServerManager-methode. Haalt het project op met de opgegeven guid van de Project Online-account  Project Server-instantie"
type: docs
weight: 40
url: /nl/net/aspose.tasks/projectservermanager/getproject/
---
## ProjectServerManager.GetProject method

Haalt het project met de opgegeven guid op uit het Project Online‑account \ Project Server‑instantie.

```csharp
public Project GetProject(Guid projectGuid)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| projectGuid | Guid | De Guid van het project om te lezen. |

### Retourwaarde

Instantie van de [`Project`](../../project/) klasse die een project representeert dat is gelezen van Project Online \ Project Server.

## Voorbeelden

Toont hoe een project te lezen van Microsoft Project Online.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
var manager = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = manager.GetProjectList();

foreach (var info in list)
{
    var project = manager.GetProject(info.Id);
    Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
    Console.WriteLine("Resources count: {0}", project.Resources.Count);
}
```

### Zie ook

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


