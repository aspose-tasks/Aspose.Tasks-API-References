---
title: "Aspose::Tasks::ProjectServerCredentials::ProjectServerCredentials yapıcı"
linktitle: "ProjectServerCredentials"
articleTitle: "ProjectServerCredentials"
second_title: "C++ için Aspose.Tasks"
description: "ProjectServerCredentials sınıfının yeni bir örneğini SharePoint sitesinin URL'si ve SharePoint'in PWA ( Proj için geçerli SPOIDCRL yetkilendirme belirteci kullanarak başlatır"
type: docs
weight: 10
url: /tr/cpp/aspose.tasks/projectservercredentials/projectservercredentials/
---

## ProjectServerCredentials (1 of 3) {#projectservercredentials_1}

SharePoint sitesinin URL'si ve SharePoint'in PWA (Project Web Access) sitesi için geçerli SPOIDCRL yetkilendirme belirteci kullanarak ProjectServerCredentials sınıfının yeni bir örneğini başlatır.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & authToken)
```

| Parametre | Açıklama |
| --- | --- |
| siteUrl | Project Online'ın PWA ( Project Web Access) API'sinin URL'si. |
| authToken | SharePoint'in PWA ( Project Web Access) sitesi için yetkilendirme belirteci (SPOIDCRL). |

---

## ProjectServerCredentials (2 of 3) {#projectservercredentials_2}

ProjectServerCredentials sınıfının yeni bir örneğini SharePoint sitesinin URL'si, kullanıcı adı ve şifre kullanarak başlatır

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & userName, const System::String & password)
```

| Parametre | Açıklama |
| --- | --- |
| siteUrl | Project Online'ın PWA ( Project Web Access) API'sinin URL'si. |
| userName | SharePoint sitesi için kullanıcı adı. |
| password | SharePoint sitesi için şifre. |

---

## ProjectServerCredentials (3 of 3) {#projectservercredentials_3}

ProjectServerCredentials sınıfının yeni bir örneğini Project Web Access uç noktasının URL'si ve ağ kimlik bilgileri kullanarak başlatır

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::SharedPtr< System::Net::NetworkCredential > & credentials)
```

| Parametre | Açıklama |
| --- | --- |
| siteUrl | Project Web Access uç noktasının URL'si. |
| kimlik bilgileri | Project Web Access uç noktasına giriş için kullanılan kimlik bilgileri. |

