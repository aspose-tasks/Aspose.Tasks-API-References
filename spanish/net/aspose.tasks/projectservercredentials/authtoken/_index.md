---
title: "ProjectServerCredentials.AuthToken"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ProjectServerCredentials. Obtiene el token de autorización para la instancia de SharePoint"
type: docs
weight: 20
url: /es/net/aspose.tasks/projectservercredentials/authtoken/
---
## ProjectServerCredentials.AuthToken property

Obtiene el token de autorización para la instancia de SharePoint.

```csharp
public string AuthToken { get; }
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


