---
title: "ProjectServerCredentials.AuthToken"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "ProjectServerCredentials propriété. Obtient le jeton d'autorisation pour l'instance SharePoint"
type: docs
weight: 20
url: /fr/net/aspose.tasks/projectservercredentials/authtoken/
---
## ProjectServerCredentials.AuthToken property

Obtient le jeton d'autorisation pour l'instance SharePoint.

```csharp
public string AuthToken { get; }
```

## Exemples

Montre comment utiliser les informations d'identification de Project Server avec SharePointOnlineCredentials pour créer un projet dans Microsoft Project Online.

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

### Voir aussi

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


