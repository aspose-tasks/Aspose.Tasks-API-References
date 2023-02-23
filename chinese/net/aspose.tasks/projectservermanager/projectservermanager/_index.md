---
title: ProjectServerManager.ProjectServerManager
second_title: Aspose.Tasks for .NET API 参考
description: ProjectServerManager 构造函数. 初始化一个新的实例ProjectServerManager类.
type: docs
weight: 10
url: /zh/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

初始化一个新的实例[`ProjectServerManager`](../)类.

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| credentials | ProjectServerCredentials | 用于连接到 Project Online 帐户的凭据。 |

### 例子

此示例说明如何创建 ProjectServerManager 实例以访问 Project Server 的本地实例。

```csharp
[C#]
string site = "http://project_server_instance.local/";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

此示例说明如何创建 ProjectServerManager 实例以访问 Project Online 服务中的帐户。

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "密码");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

### 也可以看看

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* 命名空间 [Aspose.Tasks](../../projectservermanager/)
* 部件 [Aspose.Tasks](../../../)


