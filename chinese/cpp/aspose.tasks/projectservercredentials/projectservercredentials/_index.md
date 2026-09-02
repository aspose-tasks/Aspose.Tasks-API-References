---
title: "Aspose::Tasks::ProjectServerCredentials::ProjectServerCredentials 构造函数"
linktitle: "ProjectServerCredentials"
articleTitle: "ProjectServerCredentials"
second_title: "Aspose.Tasks for C++"
description: "使用 SharePoint 站点的 URL 和有效的 SPOIDCRL 授权令牌初始化 ProjectServerCredentials 类的新实例，用于 SharePoint 的 PWA ( Proj"
type: docs
weight: 10
url: /zh/cpp/aspose.tasks/projectservercredentials/projectservercredentials/
---

## ProjectServerCredentials (1 of 3) {#projectservercredentials_1}

使用 SharePoint 站点的 URL 和用于 SharePoint PWA（项目 Web 访问）站点的有效 SPOIDCRL 授权令牌初始化 ProjectServerCredentials 类的新实例。

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & authToken)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| siteUrl | Project Online 的 PWA（Project Web Access）API 的 URL。 |
| authToken | SharePoint 的 PWA（Project Web Access）站点的授权令牌（SPOIDCRL）。 |

---

## ProjectServerCredentials (2 of 3) {#projectservercredentials_2}

使用 SharePoint 站点的 URL、用户名和密码初始化 ProjectServerCredentials 类的新实例。

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & userName, const System::String & password)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| siteUrl | Project Online 的 PWA（Project Web Access）API 的 URL。 |
| userName | SharePoint 站点的用户名。 |
| password | SharePoint 站点的密码。 |

---

## ProjectServerCredentials (3 of 3) {#projectservercredentials_3}

使用 Project Web Access 端点的 URL 和网络凭据初始化 ProjectServerCredentials 类的新实例。

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::SharedPtr< System::Net::NetworkCredential > & credentials)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| siteUrl | Project Web Access 端点的 URL。 |
| credentials | 用于登录 Project Web Access 端点的凭据。 |

