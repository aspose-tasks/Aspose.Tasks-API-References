---
title: "ProjectServerManager.GetProject"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "méthode ProjectServerManager. Obtient le projet avec le guid spécifié depuis le compte Project Online de l'instance Project Server"
type: docs
weight: 40
url: /fr/net/aspose.tasks/projectservermanager/getproject/
---
## ProjectServerManager.GetProject method

Récupère le projet avec le guid spécifié depuis le compte Project Online \ instance de Project Server.

```csharp
public Project GetProject(Guid projectGuid)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| projectGuid | Guid | Le guid du projet à lire. |

### Valeur de retour

Instance de la classe [`Project`](../../project/) qui représente le projet lu depuis Project Online \ Project Server.

## Exemples

Montre comment lire un projet depuis Microsoft Project Online.

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

### Voir aussi

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


