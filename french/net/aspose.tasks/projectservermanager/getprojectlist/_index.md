---
title: "ProjectServerManager.GetProjectList"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ProjectServerManager. Obtient la liste des projets du magasin de travail du compte Project Online actuel / instance Project Server"
type: docs
weight: 50
url: /fr/net/aspose.tasks/projectservermanager/getprojectlist/
---
## ProjectServerManager.GetProjectList method

Récupère la liste des projets du magasin 'Working' du compte Project Online actuel \ instance de Project Server.

```csharp
public IEnumerable<ProjectInfo> GetProjectList()
```

### Valeur de retour

Une énumération des projets dans le compte Project Online actuel \ instance Project Server.

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

* class [ProjectInfo](../../projectinfo/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


