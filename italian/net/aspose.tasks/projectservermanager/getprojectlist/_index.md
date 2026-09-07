---
title: "ProjectServerManager.GetProjectList"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ProjectServerManager. Ottiene l'elenco dei progetti dallo store di lavoro dell'account corrente di Project Online e dell'istanza Project Server"
type: docs
weight: 50
url: /it/net/aspose.tasks/projectservermanager/getprojectlist/
---
## ProjectServerManager.GetProjectList method

Recupera l'elenco dei progetti dal deposito 'Working' dell'account Project Online corrente \ istanza di Project Server.

```csharp
public IEnumerable<ProjectInfo> GetProjectList()
```

### Valore di ritorno

Un'enumerazione dei progetti nell'account corrente di Project Online \ istanza Project Server.

## Esempi

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

* class [ProjectInfo](../../projectinfo/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


