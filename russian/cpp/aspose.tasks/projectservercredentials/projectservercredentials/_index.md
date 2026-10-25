---
title: "Aspose::Tasks::ProjectServerCredentials::ProjectServerCredentials конструктор"
linktitle: "ProjectServerCredentials"
articleTitle: "ProjectServerCredentials"
second_title: "Aspose.Tasks для C++"
description: "Инициализирует новый экземпляр класса ProjectServerCredentials, используя URL сайта SharePoint и действительный токен авторизации SPOIDCRL для PWA (Project"
type: docs
weight: 10
url: /ru/cpp/aspose.tasks/projectservercredentials/projectservercredentials/
---

## ProjectServerCredentials (1 of 3) {#projectservercredentials_1}

Инициализирует новый экземпляр класса ProjectServerCredentials, используя URL сайта SharePoint и действительный токен авторизации SPOIDCRL для сайта PWA (Project Web Access) SharePoint.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & authToken)
```

| Параметр | Описание |
| --- | --- |
| siteUrl | URL PWA (Project Web Access) API сервиса Project Online. |
| authToken | Токен авторизации (SPOIDCRL) для сайта PWA (Project Web Access) SharePoint. |

---

## ProjectServerCredentials (2 of 3) {#projectservercredentials_2}

Инициализирует новый экземпляр класса ProjectServerCredentials, используя URL сайта SharePoint, имя пользователя и пароль.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & userName, const System::String & password)
```

| Параметр | Описание |
| --- | --- |
| siteUrl | URL PWA (Project Web Access) API сервиса Project Online. |
| userName | Имя пользователя для сайта SharePoint. |
| password | Пароль для сайта SharePoint. |

---

## ProjectServerCredentials (3 of 3) {#projectservercredentials_3}

Инициализирует новый экземпляр класса ProjectServerCredentials, используя URL конечной точки Project Web Access и сетевые учетные данные.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::SharedPtr< System::Net::NetworkCredential > & credentials)
```

| Параметр | Описание |
| --- | --- |
| siteUrl | URL конечной точки Project Web Access. |
| учётные данные | Учетные данные, используемые для входа в конечную точку Project Web Access. |

