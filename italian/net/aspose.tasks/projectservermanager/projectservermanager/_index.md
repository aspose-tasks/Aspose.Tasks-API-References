---
title: "ProjectServerManager.ProjectServerManager"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore ProjectServerManager. Inizializza una nuova istanza della classe ProjectServerManager."
type: docs
weight: 10
url: /it/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

Inizializza una nuova istanza della classe [`ProjectServerManager`](../).

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| credenziali | ProjectServerCredentials | Credenziali utilizzate per connettersi all'account Project Online. |

## Esempi

Questo esempio mostra come creare un'istanza di ProjectServerManager per accedere all'istanza on-premise di Project Server.

```csharp
[C#]
string site = "http://project_server_instance.local/";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

Questo esempio mostra come creare un'istanza di ProjectServerManager per accedere all'account nel servizio Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

Mostra come leggere un progetto da Microsoft Project Online.

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

### Vedi anche

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


