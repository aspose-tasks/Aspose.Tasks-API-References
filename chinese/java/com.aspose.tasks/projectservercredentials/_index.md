---
title: "ProjectServerCredentials"
second_title: "Aspose.Tasks for Java API 参考"
description: "用于连接到 Project Online 或本地部署的 Project Server 实例的凭据。"
type: docs
weight: 225
url: /zh/java/com.aspose.tasks/projectservercredentials/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerCredentials
```

用于连接到 Project Online 或本地部署的 Project Server 实例的凭据。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ProjectServerCredentials(String siteUrl, String authToken)](#ProjectServerCredentials-java.lang.String-java.lang.String-) | 使用 SharePoint 站点的 URL 和有效的 SPOIDCRL 授权令牌（用于 SharePoint 的 PWA（Project Web Access）站点），初始化 [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) 类的新实例。 |
| [ProjectServerCredentials(String siteUrl, String userName, String password)](#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-) | 使用 SharePoint 站点的 URL、用户名和密码，初始化 [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getAuthToken()](#getAuthToken--) | 获取 SharePoint 实例的授权令牌。 |
| [getSiteUrl()](#getSiteUrl--) | 获取 SharePoint 站点上 PWA 的 URL 或本地部署的 Project Server 的 URL。 |
| [getUserName()](#getUserName--) | 获取 SharePoint 站点的用户名。 |
| [toString()](#toString--) | 返回此实例的字符串表示形式。 |
### ProjectServerCredentials(String siteUrl, String authToken) {#ProjectServerCredentials-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String authToken)
```


使用 SharePoint 站点的 URL 和有效的 SPOIDCRL 授权令牌（用于 SharePoint 的 PWA（Project Web Access）站点），初始化 [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| siteUrl | java.lang.String | Project Online 的 PWA（Project Web Access）API 的 URL。 |
|  | authToken | java.lang.String | SharePoint 的 PWA（Project Web Access）站点的授权令牌 (SPOIDCRL)。 |

--------------------

当您已经拥有 SharePoint Online 站点的 AuthToken 时，使用此构造函数连接到 ProjectOnline。 |

### ProjectServerCredentials(String siteUrl, String userName, String password) {#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String userName, String password)
```


使用 SharePoint 站点的 URL、用户名和密码，初始化 [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| siteUrl | java.lang.String | Project Online 的 PWA（Project Web Access）API 的 URL。 |
| userName | java.lang.String | SharePoint 站点的用户名。 |
|  | password | java.lang.String | SharePoint 站点的密码。 |

--------------------

使用此构造函数连接到 ProjectOnline。请注意，应在您的 Azure 门户和 Office 365 管理中心启用传统身份验证。 |

### getAuthToken() {#getAuthToken--}
```
public final String getAuthToken()
```


获取 SharePoint 实例的授权令牌。

**Returns:**
java.lang.String - SharePoint 实例的授权令牌。
### getSiteUrl() {#getSiteUrl--}
```
public final String getSiteUrl()
```


获取 SharePoint 站点上 PWA 的 URL 或本地部署的 Project Server 的 URL。例如，https://your\_company\_name.sharepoint.com/sites/pwa\";

**Returns:**
java.lang.String - SharePoint 站点上 PWA 的 URL 或本地部署的 Project Server 的 URL。
### getUserName() {#getUserName--}
```
public final String getUserName()
```


获取 SharePoint 站点的用户名。

**Returns:**
java.lang.String - SharePoint 站点的用户名。
### toString() {#toString--}
```
public String toString()
```


返回此实例的字符串表示形式。

**Returns:**
java.lang.String - 此实例的字符串表示形式。
