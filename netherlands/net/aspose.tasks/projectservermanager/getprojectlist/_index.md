---
title: "ProjectServerManager.GetProjectList"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectServerManager-methode. Haalt de lijst met projecten op uit de werkopslag van het huidige Project Online‑account / Project Server‑instantie."
type: docs
weight: 50
url: /nl/net/aspose.tasks/projectservermanager/getprojectlist/
---
## ProjectServerManager.GetProjectList method

Haalt de lijst met projecten op uit de 'Working'-opslag van het huidige Project Online‑account \ Project Server‑instantie.

```csharp
public IEnumerable<ProjectInfo> GetProjectList()
```

### Retourwaarde

An enumeration of projects in the current Project Online account \\ Project Server instance.

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

* class [ProjectInfo](../../projectinfo/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


