---
title: "ProjectServerManager.ProjectServerManager"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectServerManager 构造函数。初始化 ProjectServerManager 类的新实例。"
type: docs
weight: 10
url: /zh/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

初始化 [`ProjectServerManager`](../) 类的新实例。

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 凭据 | ProjectServerCredentials | 用于连接到 Project Online 帐户的凭据。 |

## 示例

此示例展示了如何创建 ProjectServerManager 实例以访问本地部署的 Project Server 实例。

```csharp
[C#]
string site = "http://project_server_instance.local/";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

此示例展示了如何创建 ProjectServerManager 实例以访问 Project Online 服务中的账户。

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

展示如何从 Microsoft Project Online 读取项目。

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
var manager = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = manager.GetProjectList();

foreach (var info in list)
{
    var project = manager.GetProject(info.Id);
    Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
    Console.WriteLine("Resources count: {0}", project.Resources.Count);
}
```

### 另见

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


