---
title: "ProjectServerCredentials.ProjectServerCredentials"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectServerCredentials 构造函数。使用 SharePoint 站点的 URL 和有效的 SPOIDCRL 授权令牌，初始化 ProjectServerCredentials 类的新实例，以访问 SharePoint 的 PWA 项目 Web 访问站点"
type: docs
weight: 10
url: /zh/net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

初始化一个新的 [`ProjectServerCredentials`](../) 类实例，使用 SharePoint 站点的 URL 和有效的 SPOIDCRL 授权令牌，以访问 SharePoint 的 PWA（Project Web Access）站点。

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| siteUrl | 字符串 | Project Online 的 PWA（Project Web Access）API 的 URL。 |
| authToken | 字符串 | SharePoint 的 PWA（Project Web Access）站点的授权令牌 (SPOIDCRL)。 |

## 备注

当您已经拥有 SharePoint Online 站点的 AuthToken 时，使用此构造函数连接到 ProjectOnline。

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

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

使用 SharePoint 站点的 URL、用户名和密码，初始化 [`ProjectServerCredentials`](../) 类的新实例。

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| siteUrl | 字符串 | Project Online 的 PWA（Project Web Access）API 的 URL。 |
| userName | 字符串 | SharePoint 站点的用户名。 |
| password | 字符串 | SharePoint 站点的密码。 |

## 备注

使用此构造函数连接到 ProjectOnline。请注意，应在您的 Azure 门户和 Office 365 管理中心启用传统身份验证。

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

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

使用 Project Web Access 端点的 URL 和网络凭据，初始化 [`ProjectServerCredentials`](../) 类的新实例。

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| siteUrl | 字符串 | Project Web Access 端点的 URL。 |
| 凭据 | NetworkCredential | 用于登录 Project Web Access 端点的凭据。 |

## 备注

使用此构造函数通过 PWA 连接到本地部署的 Project Server 实例。

## 示例

在此示例中，使用 [`ProjectServerManager`](../../projectservermanager/) 类的实例从位于 http://project_server_instance.local 的 Project Server 实例读取项目列表。

```csharp
string site = "http://project_server_instance.local/sites/pwa";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);

var list = manager.GetProjectList();
foreach (var projectInfo in list)
{
    Console.WriteLine("{0} - {1} - {2}", projectInfo.Id, projectInfo.CreatedDate, projectInfo.Name);
}
```

展示如何使用 Project Server 凭据与网络凭据从本地部署的 Project Server 实例读取项目。

```csharp
try
{
    const string URL = "https://project_server.local/sites/pwa";
    const string Domain = "CONTOSO.COM";
    const string UserName = "Administrator";
    const string Password = "MyPassword";

    var project = new Project(DataDir + @"Project1.mpp");

    var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
    var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
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


