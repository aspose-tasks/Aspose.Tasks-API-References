---
title: "ProjectServerCredentials.SiteUrl"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "ProjectServerCredentials property. Ottiene l'URL di PWA nel sito SharePoint o l'URL del Project Server on-premise. Per esempio https//your_company_name.sharepoint.com/sites/pwa"
type: docs
weight: 30
url: /it/net/aspose.tasks/projectservercredentials/siteurl/
---
## ProjectServerCredentials.SiteUrl property

Ottiene l'URL di PWA nel sito SharePoint o l'URL di Project Server on‑premise. Per esempio, https://your_company_name.sharepoint.com/sites/pwa\";

```csharp
public string SiteUrl { get; }
```

## Esempi

Mostra come utilizzare le credenziali di Project Server con SharePointOnlineCredentials per creare un progetto in Microsoft Project Online.

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

### Vedi anche

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


