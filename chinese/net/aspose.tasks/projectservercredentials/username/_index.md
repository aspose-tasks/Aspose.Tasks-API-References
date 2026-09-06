---
title: "ProjectServerCredentials.UserName"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectServerCredentials 属性。获取 SharePoint 站点的用户名"
type: docs
weight: 40
url: /zh/net/aspose.tasks/projectservercredentials/username/
---
## ProjectServerCredentials.UserName property

获取 SharePoint 站点的用户名。

```csharp
public string UserName { get; }
```

## 示例

展示如何使用 Project Server 凭据与 SharePointOnlineCredentials 在 Microsoft Project Online 中创建项目。

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

### 另见

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


