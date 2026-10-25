---
title: "ProjectServerManager.GetProject"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ProjectServerManager. Ottiene il progetto con il guid specificato dall'account Project Online dell'istanza Project Server"
type: docs
weight: 40
url: /it/net/aspose.tasks/projectservermanager/getproject/
---
## ProjectServerManager.GetProject method

Recupera il progetto con il guid specificato dall'account Project Online \ istanza di Project Server.

```csharp
public Project GetProject(Guid projectGuid)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| projectGuid | Guid | Il Guid del progetto da leggere. |

### Valore di ritorno

Istanza della classe [`Project`](../../project/) che rappresenta il progetto letto da Project Online \ Project Server.

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

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


