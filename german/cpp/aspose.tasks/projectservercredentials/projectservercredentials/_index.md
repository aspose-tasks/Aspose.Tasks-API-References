---
title: "Aspose::Tasks::ProjectServerCredentials::ProjectServerCredentials Konstruktor"
linktitle: "ProjectServerCredentials"
articleTitle: "ProjectServerCredentials"
second_title: "Aspose.Tasks für C++"
description: "Initialisiert eine neue Instanz der ProjectServerCredentials-Klasse mithilfe der URL der SharePoint-Website und eines gültigen SPOIDCRL-Autorisierungstokens für die PWA ( Proj"
type: docs
weight: 10
url: /de/cpp/aspose.tasks/projectservercredentials/projectservercredentials/
---

## ProjectServerCredentials (1 of 3) {#projectservercredentials_1}

Initialisiert eine neue Instanz der Klasse ProjectServerCredentials unter Verwendung der URL der SharePoint‑Site und eines gültigen SPOIDCRL‑Autorisierungstokens für die PWA‑Site (Project Web Access) von SharePoint.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & authToken)
```

| Parameter | Beschreibung |
| --- | --- |
| siteUrl | Die URL der PWA (Project Web Access)-API von Project Online. |
| authToken | Das Autorisierungstoken (SPOIDCRL) für die PWA (Project Web Access)-Website von SharePoint. |

---

## ProjectServerCredentials (2 of 3) {#projectservercredentials_2}

Initialisiert eine neue Instanz der ProjectServerCredentials-Klasse mithilfe der URL der SharePoint-Website, des Benutzernamens und des Passworts.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & userName, const System::String & password)
```

| Parameter | Beschreibung |
| --- | --- |
| siteUrl | Die URL der PWA (Project Web Access)-API von Project Online. |
| userName | Der Benutzername für die SharePoint-Website. |
| password | Das Passwort für die SharePoint-Website. |

---

## ProjectServerCredentials (3 of 3) {#projectservercredentials_3}

Initialisiert eine neue Instanz der ProjectServerCredentials-Klasse mithilfe der URL des Project Web Access-Endpunkts und Netzwerk-Anmeldeinformationen.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::SharedPtr< System::Net::NetworkCredential > & credentials)
```

| Parameter | Beschreibung |
| --- | --- |
| siteUrl | Die URL des Project Web Access-Endpunkts. |
| credentials | Die Anmeldeinformationen, die zum Anmelden beim Project Web Access-Endpunkt verwendet werden. |

