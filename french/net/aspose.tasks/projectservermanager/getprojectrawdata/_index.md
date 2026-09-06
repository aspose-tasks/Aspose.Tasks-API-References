---
title: "ProjectServerManager.GetProjectRawData"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ProjectServerManager. Récupère les données binaires du projet à des fins de dépannage."
type: docs
weight: 60
url: /fr/net/aspose.tasks/projectservermanager/getprojectrawdata/
---
## ProjectServerManager.GetProjectRawData method

Récupère les données binaires du projet à des fins de dépannage.

```csharp
public Stream GetProjectRawData(Guid projectGuid)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| projectGuid | Guid | Le guid du projet à lire. |

### Valeur de retour

Flux contenant les données brutes du projet.

## Exemples

```csharp
In this example the debug info for the specific project is retrieved. You can pass the resulting "debug.zip" to the support team for troubleshooting purposes.
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// Guid du projet que vous essayez d'obtenir.
var projectGuid = new Guid("e0294bfb-5657-45c8-9cc5-82169fb95d69");
ProjectServerManager manager = new ProjectServerManager(credentials);
using (var fileStream = File.OpenWrite(@"c:\debug.zip"))
{
    using (var stream = manager.GetProjectRawData(projectGuid))
    {
        stream.CopyTo(fileStream);
    }
}
```

Montre comment récupérer les données brutes d'un projet depuis Microsoft Project Online à des fins de dépannage.

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

    // L'utilisateur peut lire le projet sous forme de flux de données brutes à des fins de dépannage.
    using (FileStream fs = File.Create(OutDir + "projectRawData.zip"))
    {
        using (var stream = manager.GetProjectRawData(info.Id))
        {
            stream.CopyTo(fs);
        }
    }

    // vous pouvez transmettre le fichier résultant au support.
}
```

### Voir aussi

* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


