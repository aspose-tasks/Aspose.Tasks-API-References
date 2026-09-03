---
title: "Aspose::Tasks::ProjectServerCredentials::ProjectServerCredentials constructor"
linktitle: "ProjectServerCredentials"
articleTitle: "ProjectServerCredentials"
second_title: "Aspose.Tasks voor C++"
description: "Initialiseert een nieuw exemplaar van de ProjectServerCredentials‑klasse met de URL van de SharePoint‑site en een geldig SPOIDCRL‑autorisatietoken voor de PWA ( Proj"
type: docs
weight: 10
url: /nl/cpp/aspose.tasks/projectservercredentials/projectservercredentials/
---

## ProjectServerCredentials (1 of 3) {#projectservercredentials_1}

Initialiseert een nieuwe instantie van de ProjectServerCredentials‑klasse met de URL van de SharePoint‑site en een geldig SPOIDCRL‑autorisatietoken voor de PWA‑site (Project Web Access) van SharePoint.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & authToken)
```

| Parameter | Beschrijving |
| --- | --- |
| siteUrl | De URL van de PWA ( Project Web Access) API van Project Online. |
| authToken | Het autorisatietoken (SPOIDCRL) voor de PWA ( Project Web Access) site van SharePoint. |

---

## ProjectServerCredentials (2 of 3) {#projectservercredentials_2}

Initialiseert een nieuw exemplaar van de ProjectServerCredentials‑klasse met de URL van de SharePoint‑site, gebruikersnaam en wachtwoord.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & userName, const System::String & password)
```

| Parameter | Beschrijving |
| --- | --- |
| siteUrl | De URL van de PWA ( Project Web Access) API van Project Online. |
| userName | De gebruikersnaam voor de SharePoint‑site. |
| password | Het wachtwoord voor de SharePoint‑site. |

---

## ProjectServerCredentials (3 of 3) {#projectservercredentials_3}

Initialiseert een nieuw exemplaar van de ProjectServerCredentials‑klasse met de URL van het Project Web Access‑eindpunt en netwerkauthenticatie.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::SharedPtr< System::Net::NetworkCredential > & credentials)
```

| Parameter | Beschrijving |
| --- | --- |
| siteUrl | De URL van het project web access‑eindpunt. |
| referenties | De inloggegevens die worden gebruikt om in te loggen op het Project Web Access‑eindpunt. |

