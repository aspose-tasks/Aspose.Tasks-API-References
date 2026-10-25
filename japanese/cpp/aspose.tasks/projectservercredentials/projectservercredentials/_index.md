---
title: "Aspose::Tasks::ProjectServerCredentials::ProjectServerCredentials コンストラクタ"
linktitle: "ProjectServerCredentials"
articleTitle: "ProjectServerCredentials"
second_title: "Aspose.Tasks for C++"
description: "ProjectServerCredentials クラスの新しいインスタンスを、SharePoint サイトの URL と、SharePoint の PWA（Project Web Access）用の有効な SPOIDCRL 認証トークンを使用して初期化します ( Proj"
type: docs
weight: 10
url: /ja/cpp/aspose.tasks/projectservercredentials/projectservercredentials/
---

## ProjectServerCredentials (1 of 3) {#projectservercredentials_1}

SharePoint サイトの URL と、SharePoint の PWA（Project Web Access）サイト用の有効な SPOIDCRL 認証トークンを使用して、ProjectServerCredentials クラスの新しいインスタンスを初期化します。

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & authToken)
```

| パラメーター | 説明 |
| --- | --- |
| siteUrl | Project Online の PWA（Project Web Access）API の URL。 |
| authToken | SharePoint の PWA（Project Web Access）サイト用の認証トークン（SPOIDCRL）。 |

---

## ProjectServerCredentials (2 of 3) {#projectservercredentials_2}

ProjectServerCredentials クラスの新しいインスタンスを、SharePoint サイトの URL、ユーザー名、パスワードを使用して初期化します。

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & userName, const System::String & password)
```

| パラメーター | 説明 |
| --- | --- |
| siteUrl | Project Online の PWA（Project Web Access）API の URL。 |
| userName | SharePoint サイトのユーザー名。 |
| password | SharePoint サイトのパスワード。 |

---

## ProjectServerCredentials (3 of 3) {#projectservercredentials_3}

ProjectServerCredentials クラスの新しいインスタンスを、Project Web Access エンドポイントの URL とネットワーク認証情報を使用して初期化します。

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::SharedPtr< System::Net::NetworkCredential > & credentials)
```

| パラメーター | 説明 |
| --- | --- |
| siteUrl | Project Web Access エンドポイントの URL。 |
| 認証情報 | Project Web Access エンドポイントにログインするために使用される認証情報。 |

