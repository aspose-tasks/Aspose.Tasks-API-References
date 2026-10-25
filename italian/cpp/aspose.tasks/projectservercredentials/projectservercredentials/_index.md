---
title: "Aspose::Tasks::ProjectServerCredentials::ProjectServerCredentials costruttore"
linktitle: "ProjectServerCredentials"
articleTitle: "ProjectServerCredentials"
second_title: "Aspose.Tasks per C++"
description: "Inizializza una nuova istanza della classe ProjectServerCredentials utilizzando l'URL del sito SharePoint e un token di autorizzazione SPOIDCRL valido per il PWA ( Proj"
type: docs
weight: 10
url: /it/cpp/aspose.tasks/projectservercredentials/projectservercredentials/
---

## ProjectServerCredentials (1 of 3) {#projectservercredentials_1}

Inizializza una nuova istanza della classe ProjectServerCredentials utilizzando l'URL del sito SharePoint e un token di autorizzazione SPOIDCRL valido per il sito PWA (Project Web Access) di SharePoint.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & authToken)
```

| Parametro | Descrizione |
| --- | --- |
| siteUrl | L'URL del PWA ( Project Web Access) API di Project Online. |
| authToken | Il token di autorizzazione (SPOIDCRL) per il PWA ( Project Web Access) del sito SharePoint. |

---

## ProjectServerCredentials (2 of 3) {#projectservercredentials_2}

Inizializza una nuova istanza della classe ProjectServerCredentials utilizzando l'URL del sito SharePoint, il nome utente e la password.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & userName, const System::String & password)
```

| Parametro | Descrizione |
| --- | --- |
| siteUrl | L'URL del PWA ( Project Web Access) API di Project Online. |
| userName | Il nome utente per il sito SharePoint. |
| password | La password per il sito SharePoint. |

---

## ProjectServerCredentials (3 of 3) {#projectservercredentials_3}

Inizializza una nuova istanza della classe ProjectServerCredentials utilizzando l'URL del punto finale Project Web Access e le credenziali di rete.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::SharedPtr< System::Net::NetworkCredential > & credentials)
```

| Parametro | Descrizione |
| --- | --- |
| siteUrl | L'URL del punto finale di project web access. |
| credenziali | Le credenziali utilizzate per accedere al punto finale di Project Web Access. |

