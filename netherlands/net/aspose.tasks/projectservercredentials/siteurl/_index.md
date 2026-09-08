---
title: "ProjectServerCredentials.SiteUrl"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectServerCredentials eigenschap. Haalt de URL van PWA op op de SharePoint‑site of de URL van een on‑premise Project Server. Bijvoorbeeld https//your_company_name.sharepoint.com/sites/pwa"
type: docs
weight: 30
url: /nl/net/aspose.tasks/projectservercredentials/siteurl/
---
## ProjectServerCredentials.SiteUrl property

Haalt de URL van PWA op bij de SharePoint-site of de URL van een on-premise Project Server op. Bijvoorbeeld, https://your_company_name.sharepoint.com/sites/pwa\";

```csharp
public string SiteUrl { get; }
```

## Voorbeelden

Toont hoe u Project Server‑referenties met SharePointOnlineCredentials gebruikt om een project te maken in Microsoft Project Online.

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

### Zie ook

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


