---
title: "ProjectServerManager.GetProjectList"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ProjectServerManager. Obtiene la lista de proyectos del almacén de trabajo de la cuenta actual de Project Online / instancia de Project Server."
type: docs
weight: 50
url: /es/net/aspose.tasks/projectservermanager/getprojectlist/
---
## ProjectServerManager.GetProjectList method

Obtiene la lista de proyectos del almacén 'Working' de la cuenta actual de Project Online \\ instancia de Project Server.

```csharp
public IEnumerable<ProjectInfo> GetProjectList()
```

### Valor devuelto

Una enumeración de proyectos en la cuenta actual de Project Online \ instancia de Project Server.

## Ejemplos

Muestra cómo leer un proyecto de Microsoft Project Online.

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

### Ver también

* class [ProjectInfo](../../projectinfo/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


