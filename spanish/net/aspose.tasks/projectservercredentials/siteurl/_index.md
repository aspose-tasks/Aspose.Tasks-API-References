---
title: "ProjectServerCredentials.SiteUrl"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ProjectServerCredentials. Obtiene la URL de PWA en el sitio de SharePoint o la URL del Project Server local. Por ejemplo https//your_company_name.sharepoint.com/sites/pwa"
type: docs
weight: 30
url: /es/net/aspose.tasks/projectservercredentials/siteurl/
---
## ProjectServerCredentials.SiteUrl property

Obtiene la URL de PWA en el sitio SharePoint o la URL del Project Server local. Por ejemplo, https://your_company_name.sharepoint.com/sites/pwa\";

```csharp
public string SiteUrl { get; }
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


