---
title: "Aspose::Tasks::ProjectServerCredentials::ProjectServerCredentials constructeur"
linktitle: "ProjectServerCredentials"
articleTitle: "ProjectServerCredentials"
second_title: "Aspose.Tasks pour C++"
description: "Initialise une nouvelle instance de la classe ProjectServerCredentials en utilisant l'URL du site SharePoint et un jeton d'autorisation SPOIDCRL valide pour le PWA ( Project"
type: docs
weight: 10
url: /fr/cpp/aspose.tasks/projectservercredentials/projectservercredentials/
---

## ProjectServerCredentials (1 of 3) {#projectservercredentials_1}

Initialise une nouvelle instance de la classe ProjectServerCredentials en utilisant l'URL du site SharePoint et un jeton d'autorisation SPOIDCRL valide pour le site PWA (Project Web Access) de SharePoint.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & authToken)
```

| Paramètre | Description |
| --- | --- |
| siteUrl | L'URL du PWA ( Project Web Access) API de Project Online. |
| authToken | Le jeton d'autorisation (SPOIDCRL) pour le PWA ( Project Web Access) du site SharePoint. |

---

## ProjectServerCredentials (2 of 3) {#projectservercredentials_2}

Initialise une nouvelle instance de la classe ProjectServerCredentials en utilisant l'URL du site SharePoint, le nom d'utilisateur et le mot de passe.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & userName, const System::String & password)
```

| Paramètre | Description |
| --- | --- |
| siteUrl | L'URL du PWA ( Project Web Access) API de Project Online. |
| userName | Le nom d'utilisateur pour le site SharePoint. |
| password | Le mot de passe pour le site SharePoint. |

---

## ProjectServerCredentials (3 of 3) {#projectservercredentials_3}

Initialise une nouvelle instance de la classe ProjectServerCredentials en utilisant l'URL du point de terminaison Project Web Access et les informations d'identification réseau.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::SharedPtr< System::Net::NetworkCredential > & credentials)
```

| Paramètre | Description |
| --- | --- |
| siteUrl | L'URL du point de terminaison Project Web Access. |
| identifiants | Les informations d'identification utilisées pour se connecter au point de terminaison Project Web Access. |

