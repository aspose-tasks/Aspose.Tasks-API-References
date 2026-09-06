---
title: "ProjectServerCredentials"
second_title: "Aspose.Tasks for Java API-referens"
description: "Referenser som används för att ansluta till Project Online eller en lokal instans av Project Server."
type: docs
weight: 225
url: /sv/java/com.aspose.tasks/projectservercredentials/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerCredentials
```

Referenser som används för att ansluta till Project Online eller en lokal instans av Project Server.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ProjectServerCredentials(String siteUrl, String authToken)](#ProjectServerCredentials-java.lang.String-java.lang.String-) | Initierar en ny instans av klassen [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) med URL för SharePoint-webbplatsen och en giltig SPOIDCRL-auktoriseringstoken för SharePoints PWA (Project Web Access)-site. |
| [ProjectServerCredentials(String siteUrl, String userName, String password)](#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-) | Initierar en ny instans av klassen [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) med URL för SharePoint-webbplatsen, användarnamn och lösenord. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getAuthToken()](#getAuthToken--) | Hämtar auktoriseringstoken för SharePoint-instansen. |
| [getSiteUrl()](#getSiteUrl--) | Hämtar URL för PWA på SharePoint-webbplatsen eller URL för lokal Project Server. |
| [getUserName()](#getUserName--) | Hämtar användarnamnet för SharePoint-webbplatsen. |
| [toString()](#toString--) | Returnerar en strängrepresentation av denna instans. |
### ProjectServerCredentials(String siteUrl, String authToken) {#ProjectServerCredentials-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String authToken)
```


Initierar en ny instans av klassen [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) med URL för SharePoint-webbplatsen och en giltig SPOIDCRL-auktoriseringstoken för SharePoints PWA (Project Web Access)-site.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| siteUrl | java.lang.String | URL:en för PWA (Project Web Access)-API:n för Project Online. |
|  | authToken | java.lang.String | Auktoriseringstoken (SPOIDCRL) för SharePoints PWA (Project Web Access)-site. |

--------------------

Använd den här konstruktorn för att ansluta till ProjectOnline när du redan har AuthToken för din SharePoint Online-webbplats. |

### ProjectServerCredentials(String siteUrl, String userName, String password) {#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String userName, String password)
```


Initierar en ny instans av klassen [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) med URL för SharePoint-webbplatsen, användarnamn och lösenord.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| siteUrl | java.lang.String | URL:en för PWA (Project Web Access)-API:n för Project Online. |
| userName | java.lang.String | Användarnamnet för SharePoint‑webbplatsen. |
|  | lösenord | java.lang.String | Lösenordet för SharePoint‑webbplatsen. |

--------------------

Använd den här konstruktorn för att ansluta till ProjectOnline. Observera att äldre autentisering bör vara aktiverad i din Azure‑portal och i Office 365‑admincenter. |

### getAuthToken() {#getAuthToken--}
```
public final String getAuthToken()
```


Hämtar auktoriseringstoken för SharePoint-instansen.

**Returns:**
java.lang.String – auktoriseringstoken för SharePoint‑instansen.
### getSiteUrl() {#getSiteUrl--}
```
public final String getSiteUrl()
```


Hämtar URL:en för PWA på SharePoint‑webbplatsen eller URL:en för en lokal Project Server. Till exempel https://your\_company\_name.sharepoint.com/sites/pwa\";

**Returns:**
java.lang.String – URL:en för PWA på SharePoint‑webbplatsen eller URL:en för en lokal Project Server.
### getUserName() {#getUserName--}
```
public final String getUserName()
```


Hämtar användarnamnet för SharePoint-webbplatsen.

**Returns:**
java.lang.String – användarnamnet för SharePoint‑webbplatsen.
### toString() {#toString--}
```
public String toString()
```


Returnerar en strängrepresentation av denna instans.

**Returns:**
java.lang.String - en strängrepresentation av denna instans.
