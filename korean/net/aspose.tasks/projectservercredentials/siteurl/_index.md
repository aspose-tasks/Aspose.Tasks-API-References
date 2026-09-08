---
title: "ProjectServerCredentials.SiteUrl"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectServerCredentials 속성. SharePoint 사이트의 PWA URL 또는 온프레미스 Project Server URL을 가져옵니다. 예: https//your_company_name.sharepoint.com/sites/pwa"
type: docs
weight: 30
url: /ko/net/aspose.tasks/projectservercredentials/siteurl/
---
## ProjectServerCredentials.SiteUrl property

SharePoint 사이트의 PWA URL 또는 온프레미스 Project Server URL을 가져옵니다. 예: https://your_company_name.sharepoint.com/sites/pwa\";

```csharp
public string SiteUrl { get; }
```

## 예제

Project Server 자격 증명을 SharePointOnlineCredentials와 함께 사용하여 Microsoft Project Online에서 프로젝트를 만드는 방법을 보여줍니다.

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

### 또 보기

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


