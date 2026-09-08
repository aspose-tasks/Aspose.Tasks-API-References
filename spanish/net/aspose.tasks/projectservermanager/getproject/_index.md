---
title: "ProjectServerManager.GetProject"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ProjectServerManager. Obtiene el proyecto con el guid especificado de la cuenta Project Online instancia de Project Server"
type: docs
weight: 40
url: /es/net/aspose.tasks/projectservermanager/getproject/
---
## ProjectServerManager.GetProject method

Obtiene el proyecto con el GUID especificado de la cuenta de Project Online \\ instancia de Project Server.

```csharp
public Project GetProject(Guid projectGuid)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| projectGuid | Guid | El Guid del proyecto a leer. |

### Valor devuelto

Instancia de la clase [`Project`](../../project/) que representa el proyecto leído de Project Online \\ Project Server.

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

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


