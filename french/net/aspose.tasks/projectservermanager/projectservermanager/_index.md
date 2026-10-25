---
title: "ProjectServerManager.ProjectServerManager"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur ProjectServerManager. Initialise une nouvelle instance de la classe ProjectServerManager."
type: docs
weight: 10
url: /fr/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

Initialise une nouvelle instance de la classe [`ProjectServerManager`](../).

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| identifiants | ProjectServerCredentials | Identifiants utilisés pour se connecter au compte Project Online. |

## Exemples

Cet exemple montre comment créer une instance de ProjectServerManager pour accéder à une instance sur site de Project Server.

```csharp
[C#]
string site = "http://project_server_instance.local/";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

Cet exemple montre comment créer une instance de ProjectServerManager pour accéder à un compte dans le service Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

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

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


