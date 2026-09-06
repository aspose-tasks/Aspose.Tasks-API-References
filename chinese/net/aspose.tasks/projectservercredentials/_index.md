---
title: "类 ProjectServerCredentials"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ProjectServerCredentials 类。用于连接 Project Online 或本地 Project Server 实例的凭据"
type: docs
weight: 1490
url: /zh/net/aspose.tasks/projectservercredentials/
---
## ProjectServerCredentials class

用于连接到 Project Online 或本地部署的 Project Server 实例的凭据。

```csharp
public sealed class ProjectServerCredentials
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [ProjectServerCredentials](projectservercredentials/#constructor)(string, NetworkCredential) | 使用 Project Web Access 端点的 URL 和网络凭据初始化 `ProjectServerCredentials` 类的新实例。 |
| [ProjectServerCredentials](projectservercredentials/#constructor_1)(string, string) | 使用 SharePoint 站点的 URL 和有效的 SPOIDCRL 授权令牌（用于 SharePoint 的 PWA（Project Web Access）站点）初始化 `ProjectServerCredentials` 类的新实例。 |
| [ProjectServerCredentials](projectservercredentials/#constructor_2)(string, string, string) | 使用 SharePoint 站点的 URL、用户名和密码初始化 `ProjectServerCredentials` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AuthToken](../../aspose.tasks/projectservercredentials/authtoken/) { get; } | 获取 SharePoint 实例的授权令牌。 |
| [SiteUrl](../../aspose.tasks/projectservercredentials/siteurl/) { get; } | 获取 SharePoint 站点上 PWA 的 URL 或本地 Project Server 的 URL。例如，https://your_company_name.sharepoint.com/sites/pwa\"; |
| [UserName](../../aspose.tasks/projectservercredentials/username/) { get; } | 获取 SharePoint 站点的用户名。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [ToString](../../aspose.tasks/projectservercredentials/tostring/)() | 返回此实例的字符串表示。 |

## 示例

展示如何使用项目服务器凭据从 Microsoft Project Online 检索项目列表。

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var newProject = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(newProject);

    IEnumerable<ProjectInfo> list = manager.GetProjectList();

    foreach (var info in list)
    {
        var project = manager.GetProject(info.Id);
        Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
        Console.WriteLine("Resources count: {0}", project.Resources.Count);
    }
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


