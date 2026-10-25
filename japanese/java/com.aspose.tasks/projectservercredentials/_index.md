---
title: "ProjectServerCredentials"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "Project Online またはオンプレミスの Project Server インスタンスに接続するために使用される認証情報です。"
type: docs
weight: 225
url: /ja/java/com.aspose.tasks/projectservercredentials/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerCredentials
```

Project Online またはオンプレミスの Project Server インスタンスに接続するために使用される認証情報です。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [ProjectServerCredentials(String siteUrl, String authToken)](#ProjectServerCredentials-java.lang.String-java.lang.String-) | SharePoint サイトの URL と、SharePoint の PWA（Project Web Access）サイト用の有効な SPOIDCRL 認証トークンを使用して、[ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) クラスの新しいインスタンスを初期化します。 |
| [ProjectServerCredentials(String siteUrl, String userName, String password)](#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-) | SharePoint サイトの URL、ユーザー名、パスワードを使用して、[ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getAuthToken()](#getAuthToken--) | SharePoint インスタンスの認証トークンを取得します。 |
| [getSiteUrl()](#getSiteUrl--) | SharePoint サイトの PWA の URL またはオンプレミス Project Server の URL を取得します。 |
| [getUserName()](#getUserName--) | SharePoint サイトのユーザー名を取得します。 |
| [toString()](#toString--) | このインスタンスの文字列表現を返します。 |
### ProjectServerCredentials(String siteUrl, String authToken) {#ProjectServerCredentials-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String authToken)
```


SharePoint サイトの URL と、SharePoint の PWA（Project Web Access）サイト用の有効な SPOIDCRL 認証トークンを使用して、[ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| siteUrl | java.lang.String | Project Online の PWA（Project Web Access）API の URL。 |
|  | authToken | java.lang.String | SharePoint の PWA（Project Web Access）サイト用の認証トークン（SPOIDCRL）。 |

--------------------

SharePoint Online サイトの AuthToken を既に持っている場合に、このコンストラクタを使用して ProjectOnline に接続します。 |

### ProjectServerCredentials(String siteUrl, String userName, String password) {#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String userName, String password)
```


SharePoint サイトの URL、ユーザー名、パスワードを使用して、[ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| siteUrl | java.lang.String | Project Online の PWA（Project Web Access）API の URL。 |
| userName | java.lang.String | SharePoint サイトのユーザー名。 |
|  | password | java.lang.String | SharePoint サイトのパスワード。 |

--------------------

このコンストラクタを使用して ProjectOnline に接続します。レガシー認証は Azure ポータルおよび Office 365 管理センターで有効にする必要があることに注意してください。 |

### getAuthToken() {#getAuthToken--}
```
public final String getAuthToken()
```


SharePoint インスタンスの認証トークンを取得します。

**Returns:**
java.lang.String - SharePoint インスタンス用の認証トークン。
### getSiteUrl() {#getSiteUrl--}
```
public final String getSiteUrl()
```


SharePoint サイトの PWA の URL またはオンプレミス Project Server の URL を取得します。例: https://your\_company\_name.sharepoint.com/sites/pwa";

**Returns:**
java.lang.String - SharePoint サイトの PWA の URL またはオンプレミス Project Server の URL。
### getUserName() {#getUserName--}
```
public final String getUserName()
```


SharePoint サイトのユーザー名を取得します。

**Returns:**
java.lang.String - SharePoint サイトのユーザー名。
### toString() {#toString--}
```
public String toString()
```


このインスタンスの文字列表現を返します。

**Returns:**
java.lang.String - このインスタンスの文字列表現です。
