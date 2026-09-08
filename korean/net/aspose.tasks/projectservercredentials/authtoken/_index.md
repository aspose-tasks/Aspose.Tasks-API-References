---
title: "ProjectServerCredentials.AuthToken"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectServerCredentials 속성. SharePoint 인스턴스에 대한 인증 토큰을 가져옵니다"
type: docs
weight: 20
url: /ko/net/aspose.tasks/projectservercredentials/authtoken/
---
## ProjectServerCredentials.AuthToken property

SharePoint 인스턴스에 대한 인증 토큰을 가져옵니다.

```csharp
public string AuthToken { get; }
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


