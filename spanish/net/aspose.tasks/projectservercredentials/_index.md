---
title: "Clase ProjectServerCredentials"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.ProjectServerCredentials. Credenciales que se utilizan para conectarse a Project Online o a una instancia local de Project Server"
type: docs
weight: 1490
url: /es/net/aspose.tasks/projectservercredentials/
---
## ProjectServerCredentials class

Credenciales que se utilizan para conectar a Project Online o a una instancia local de Project Server.

```csharp
public sealed class ProjectServerCredentials
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ProjectServerCredentials](projectservercredentials/#constructor)(string, NetworkCredential) | Inicializa una nueva instancia de la clase `ProjectServerCredentials` usando la URL del punto final de Project Web Access y credenciales de red. |
| [ProjectServerCredentials](projectservercredentials/#constructor_1)(string, string) | Inicializa una nueva instancia de la clase `ProjectServerCredentials` usando la URL del sitio SharePoint y un token de autorización SPOIDCRL válido para el sitio PWA (Project Web Access) de SharePoint. |
| [ProjectServerCredentials](projectservercredentials/#constructor_2)(string, string, string) | Inicializa una nueva instancia de la clase `ProjectServerCredentials` usando la URL del sitio SharePoint, nombre de usuario y contraseña. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AuthToken](../../aspose.tasks/projectservercredentials/authtoken/) { get; } | Obtiene el token de autorización para la instancia de SharePoint. |
| [SiteUrl](../../aspose.tasks/projectservercredentials/siteurl/) { get; } | Obtiene la URL de PWA en el sitio SharePoint o la URL del Project Server local. Por ejemplo, https://your_company_name.sharepoint.com/sites/pwa\"; |
| [UserName](../../aspose.tasks/projectservercredentials/username/) { get; } | Obtiene el nombre de usuario para el sitio SharePoint. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [ToString](../../aspose.tasks/projectservercredentials/tostring/)() | Devuelve una representación en cadena de esta instancia. |

## Ejemplos

Muestra cómo usar credenciales de Project Server para obtener la lista de proyectos de Microsoft Project Online.

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var newProject = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(newProject);

    IEnumerable<ProjectInfo> list = manager.GetProjectList();

    foreach (var info in list)
    {
        var project = manager.GetProject(info.Id);
        Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
        Console.WriteLine("Resources count: {0}", project.Resources.Count);
    }
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


