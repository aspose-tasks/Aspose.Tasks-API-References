---
title: "ProjectServerCredentials.UserName"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "ProjectServerCredentials properti. Mendapatkan nama pengguna untuk situs SharePoint"
type: docs
weight: 40
url: /id/net/aspose.tasks/projectservercredentials/username/
---
## ProjectServerCredentials.UserName property

Mendapatkan nama pengguna untuk situs SharePoint.

```csharp
public string UserName { get; }
```

## Contoh

Menampilkan cara menggunakan kredensial Project Server dengan SharePointOnlineCredentials untuk membuat proyek di Microsoft Project Online.

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

### Lihat Juga

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


