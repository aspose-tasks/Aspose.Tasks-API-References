---
title: "ProjectServerCredentials"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Inloggegevens die worden gebruikt om verbinding te maken met Project Online of een on‑premise‑instantie van Project Server."
type: docs
weight: 225
url: /nl/java/com.aspose.tasks/projectservercredentials/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerCredentials
```

Inloggegevens die worden gebruikt om verbinding te maken met Project Online of een on‑premise‑instantie van Project Server.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ProjectServerCredentials(String siteUrl, String authToken)](#ProjectServerCredentials-java.lang.String-java.lang.String-) | Initialiseert een nieuw exemplaar van de [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) klasse met behulp van de URL van de SharePoint‑site en een geldig SPOIDCRL‑autorisatietoken voor de PWA (Project Web Access)‑site van SharePoint. |
| [ProjectServerCredentials(String siteUrl, String userName, String password)](#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-) | Initialiseert een nieuw exemplaar van de [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) klasse met behulp van de URL van de SharePoint‑site, gebruikersnaam en wachtwoord. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getAuthToken()](#getAuthToken--) | Haalt het autorisatietoken op voor de SharePoint‑instantie. |
| [getSiteUrl()](#getSiteUrl--) | Haalt de URL van PWA op bij de SharePoint‑site of de URL van de on‑premise Project Server. |
| [getUserName()](#getUserName--) | Haalt de gebruikersnaam op voor de SharePoint‑site. |
| [toString()](#toString--) | Retourneert een tekenreeksrepresentatie van deze instantie. |
### ProjectServerCredentials(String siteUrl, String authToken) {#ProjectServerCredentials-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String authToken)
```


Initialiseert een nieuw exemplaar van de [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) klasse met behulp van de URL van de SharePoint‑site en een geldig SPOIDCRL‑autorisatietoken voor de PWA (Project Web Access)‑site van SharePoint.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| siteUrl | java.lang.String | De URL van de PWA (Project Web Access) API van Project Online. |
|  | authToken | java.lang.String | Het autorisatietoken (SPOIDCRL) voor de PWA (Project Web Access)‑site van SharePoint. |

--------------------

Gebruik deze constructor om verbinding te maken met ProjectOnline wanneer je al een AuthToken hebt voor je SharePoint Online‑site. |

### ProjectServerCredentials(String siteUrl, String userName, String password) {#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String userName, String password)
```


Initialiseert een nieuw exemplaar van de [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) klasse met behulp van de URL van de SharePoint‑site, gebruikersnaam en wachtwoord.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| siteUrl | java.lang.String | De URL van de PWA (Project Web Access) API van Project Online. |
| userName | java.lang.String | De gebruikersnaam voor de SharePoint‑site. |
|  | password | java.lang.String | Het wachtwoord voor de SharePoint‑site. |

--------------------

Gebruik deze constructor om verbinding te maken met ProjectOnline. Houd er rekening mee dat legacy‑authenticatie moet worden ingeschakeld in je Azure‑portal en Office 365‑admincentrum. |

### getAuthToken() {#getAuthToken--}
```
public final String getAuthToken()
```


Haalt het autorisatietoken op voor de SharePoint‑instantie.

**Returns:**
java.lang.String - het autorisatietoken voor de SharePoint‑instantie.
### getSiteUrl() {#getSiteUrl--}
```
public final String getSiteUrl()
```


Haalt de URL van PWA op bij de SharePoint‑site of de URL van de on‑premise Project Server. Bijvoorbeeld, https://your\_company\_name.sharepoint.com/sites/pwa\";

**Returns:**
java.lang.String - de URL van PWA bij de SharePoint‑site of de URL van de on‑premise Project Server.
### getUserName() {#getUserName--}
```
public final String getUserName()
```


Haalt de gebruikersnaam op voor de SharePoint‑site.

**Returns:**
java.lang.String - de gebruikersnaam voor de SharePoint‑site.
### toString() {#toString--}
```
public String toString()
```


Retourneert een tekenreeksrepresentatie van deze instantie.

**Returns:**
java.lang.String - een tekenreeksrepresentatie van deze instantie.
