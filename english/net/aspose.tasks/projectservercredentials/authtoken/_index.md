---
title: ProjectServerCredentials.AuthToken
second_title: Aspose.Tasks for .NET API Reference
description: ProjectServerCredentials property. Gets the authorization token for the SharePoint instance
type: docs
weight: 20
url: /net/aspose.tasks/projectservercredentials/authtoken/
---
## ProjectServerCredentials.AuthToken property

Gets the authorization token for the SharePoint instance.

```csharp
public string AuthToken { get; }
```

## Examples

Shows how to use Project Server credentials with SharePointOnlineCredentials to create project in Microsoft Project Online.

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

### See Also

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


