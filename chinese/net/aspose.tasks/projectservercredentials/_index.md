---
title: Class ProjectServerCredentials
second_title: Aspose.Tasks for .NET API 参考
description: Aspose.Tasks.ProjectServerCredentials 班级. 用于连接到 Project Online 或 Project Server 的本地实例的凭据
type: docs
weight: 1240
url: /zh/net/aspose.tasks/projectservercredentials/
---
## ProjectServerCredentials class

用于连接到 Project Online 或 Project Server 的本地实例的凭据。

```csharp
public sealed class ProjectServerCredentials
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [ProjectServerCredentials](projectservercredentials/#constructor)(string, NetworkCredential) | 初始化一个新的实例`ProjectServerCredentials`使用 Project Web Access 终结点的 URL 和网络凭据的类。 |
| [ProjectServerCredentials](projectservercredentials/#constructor_1)(string, string) | 初始化一个新的实例`ProjectServerCredentials`使用 SharePoint 站点的 URL 和 SharePoint 的 PWA（项目 Web 访问）站点的有效 SPOIDCRL 授权令牌的类。 |
| [ProjectServerCredentials](projectservercredentials/#constructor_2)(string, string, string) | 初始化一个新的实例`ProjectServerCredentials`使用 SharePoint 站点的 URL、用户名和密码的类。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [AuthToken](../../aspose.tasks/projectservercredentials/authtoken/) { get; } | 获取 SharePoint 实例的授权令牌。 |
| [SiteUrl](../../aspose.tasks/projectservercredentials/siteurl/) { get; } | 获取 SharePoint 网站上 PWA 的 URL 或本地项目服务器的 URL。 例如，https://your_company_name.sharepoint.com/sites/pwa"; |
| [UserName](../../aspose.tasks/projectservercredentials/username/) { get; } | 获取 SharePoint 站点的用户名。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| override [ToString](../../aspose.tasks/projectservercredentials/tostring/)() | 返回此实例的字符串表示。 |

### 也可以看看

* 命名空间 [Aspose.Tasks](../../aspose.tasks/)
* 部件 [Aspose.Tasks](../../)


