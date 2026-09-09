---
title: "ProjectServerCredentials.UserName"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectServerCredentials özelliği. SharePoint sitesi için kullanıcı adını alır"
type: docs
weight: 40
url: /tr/net/aspose.tasks/projectservercredentials/username/
---
## ProjectServerCredentials.UserName property

SharePoint sitesi için kullanıcı adını alır.

```csharp
public string UserName { get; }
```

## Örnekler

Project Server kimlik bilgilerini SharePointOnlineCredentials ile kullanarak Microsoft Project Online'da proje oluşturmayı gösterir.

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

### Ayrıca Bakınız

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


