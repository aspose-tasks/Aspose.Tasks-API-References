---
title: "Aspose::Tasks::ProjectServerCredentials::ProjectServerCredentials constructor"
linktitle: "ProjectServerCredentials"
articleTitle: "ProjectServerCredentials"
second_title: "Aspose.Tasks for C++"
description: "Initializes a new instance of the ProjectServerCredentials class using URL of SharePoint site and valid SPOIDCRL authorization token for SharePoint's PWA ( Proj"
type: docs
weight: 10
url: /cpp/aspose.tasks/projectservercredentials/projectservercredentials/
---

## ProjectServerCredentials (1 of 3) {#projectservercredentials_1}

Initializes a new instance of the ProjectServerCredentials class using URL of SharePoint site and valid SPOIDCRL authorization token for SharePoint's PWA ( Project Web Access) site.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & authToken)
```

| Parameter | Description |
| --- | --- |
| siteUrl | The URL of PWA ( Project Web Access) API of Project Online. |
| authToken | The authorization token (SPOIDCRL) for SharePoint's PWA ( Project Web Access) site. |

---

## ProjectServerCredentials (2 of 3) {#projectservercredentials_2}

Initializes a new instance of the ProjectServerCredentials class using URL of SharePoint site, user name and password.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & userName, const System::String & password)
```

| Parameter | Description |
| --- | --- |
| siteUrl | The URL of PWA ( Project Web Access) API of Project Online. |
| userName | The user name for the SharePoint site. |
| password | The password for the SharePoint site. |

---

## ProjectServerCredentials (3 of 3) {#projectservercredentials_3}

Initializes a new instance of the ProjectServerCredentials class using URL of Project Web Access endpoint and network credentials.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::SharedPtr< System::Net::NetworkCredential > & credentials)
```

| Parameter | Description |
| --- | --- |
| siteUrl | The URL of project web access endpoint. |
| credentials | The credentials used to login to Project Web Access endpoint. |

