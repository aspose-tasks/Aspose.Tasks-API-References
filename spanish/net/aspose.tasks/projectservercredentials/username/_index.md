---
title: "ProjectServerCredentials.UserName"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ProjectServerCredentials. Obtiene el nombre de usuario para el sitio de SharePoint"
type: docs
weight: 40
url: /es/net/aspose.tasks/projectservercredentials/username/
---
## ProjectServerCredentials.UserName property

Obtiene el nombre de usuario para el sitio SharePoint.

```csharp
public string UserName { get; }
```

## Ejemplos

Muestra cómo usar credenciales de Project Server con SharePointOnlineCredentials para crear un proyecto en Microsoft Project Online.

```csharp
try
{
    const string Username = "admin@contoso.onmicrosoft.com";
    const string SecuredPassword = "MyPassword";
    var url = new Uri("https://contoso.sharepoint.com/sites/pwa");
    var project = new Project(DataDir + "Project1.mpp");
    var password = new SecureString();
    foreach (var c in SecuredPassword)
    {
        password.AppendChar(c);
    }

    var onlineCredentials = new SharePointOnlineCredentials(Username, password);
    var projectServerCredentials = new ProjectServerCredentials(url.ToString(), onlineCredentials.GetAuthenticationCookie(url, true));

    Console.WriteLine("Project Server Auth Token: " + projectServerCredentials.AuthToken);
    Console.WriteLine("Project Server Site Url: " + projectServerCredentials.SiteUrl);
    Console.WriteLine("Project Server User Name: " + projectServerCredentials.UserName);

    var manager = new ProjectServerManager(projectServerCredentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Ver también

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


