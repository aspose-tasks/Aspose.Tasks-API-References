---
title: ProjectServerCredentials.ProjectServerCredentials
second_title: Aspose.Tasks for .NET API 参考
description: ProjectServerCredentials 构造函数. 初始化一个新的实例ProjectServerCredentials使用 SharePoint 站点的 URL 和 SharePoint 的 PWA项目 Web 访问站点的有效 SPOIDCRL 授权令牌的类
type: docs
weight: 10
url: /zh/net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

初始化一个新的实例[`ProjectServerCredentials`](../)使用 SharePoint 站点的 URL 和 SharePoint 的 PWA（项目 Web 访问）站点的有效 SPOIDCRL 授权令牌的类。

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| siteUrl | String | Project Online 的 PWA（Project Web Access）API 的 URL。 |
| authToken | String | SharePoint 的 PWA (Project Web Access) 站点的授权令牌 (SPOIDCRL)。 |

### 评论

当您的 SharePoint Online 网站已有 AuthToken 时，使用此构造函数连接到 ProjectOnline。

### 也可以看看

* class [ProjectServerCredentials](../)
* 命名空间 [Aspose.Tasks](../../projectservercredentials/)
* 部件 [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

初始化一个新的实例[`ProjectServerCredentials`](../)使用 SharePoint 站点的 URL、用户名和密码的类。

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| siteUrl | String | Project Online 的 PWA（Project Web Access）API 的 URL。 |
| userName | String | SharePoint 站点的用户名。 |
| password | String | SharePoint 站点的密码。 |

### 评论

使用此构造函数连接到 ProjectOnline。请注意，应在您的 Azure 门户和 Office 365 管理中心启用旧版身份验证。

### 也可以看看

* class [ProjectServerCredentials](../)
* 命名空间 [Aspose.Tasks](../../projectservercredentials/)
* 部件 [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

初始化一个新的实例[`ProjectServerCredentials`](../)使用 Project Web Access 终结点的 URL 和网络凭据的类。

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| siteUrl | String | 项目 Web 访问端点的 URL。 |
| credentials | NetworkCredential | 用于登录到 Project Web Access 终结点的凭据。 |

### 评论

使用此构造函数通过 PWA 连接到 Project Server 的本地实例。

### 例子

在这个例子中的实例[`ProjectServerManager`](../../projectservermanager/)类用于从位于 http://project_server_instance.local 的 Project Server 实例中读取项目列表

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

### 也可以看看

* class [ProjectServerCredentials](../)
* 命名空间 [Aspose.Tasks](../../projectservercredentials/)
* 部件 [Aspose.Tasks](../../../)


