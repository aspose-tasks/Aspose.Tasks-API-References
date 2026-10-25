---
title: "ProjectServerManager.ProjectServerManager"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor ProjectServerManager. Inicializa una nueva instancia de la clase ProjectServerManager."
type: docs
weight: 10
url: /es/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

Inicializa una nueva instancia de la clase [`ProjectServerManager`](../).

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| credenciales | ProjectServerCredentials | Credenciales utilizadas para conectarse a la cuenta de Project Online. |

## Ejemplos

Este ejemplo muestra cómo crear una instancia de ProjectServerManager para acceder a la instancia local de Project Server.

```csharp
[C#]
string site = "http://project_server_instance.local/";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

Este ejemplo muestra cómo crear una instancia de ProjectServerManager para acceder a una cuenta en el servicio Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

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

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


