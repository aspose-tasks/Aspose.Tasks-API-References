---
title: "ProjectServerCredentials"
second_title: "Aspose.Tasks for Java API Reference"
description: "Anmeldeinformationen, die zum Verbinden mit Project Online oder einer lokalen Instanz von Project Server verwendet werden."
type: docs
weight: 225
url: /de/java/com.aspose.tasks/projectservercredentials/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerCredentials
```

Anmeldeinformationen, die zum Verbinden mit Project Online oder einer lokalen Instanz von Project Server verwendet werden.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ProjectServerCredentials(String siteUrl, String authToken)](#ProjectServerCredentials-java.lang.String-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) unter Verwendung der URL der SharePoint‑Site und eines gültigen SPOIDCRL‑Autorisierungstokens für die PWA (Project Web Access)-Site von SharePoint. |
| [ProjectServerCredentials(String siteUrl, String userName, String password)](#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) unter Verwendung der URL der SharePoint‑Site, des Benutzernamens und des Passworts. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getAuthToken()](#getAuthToken--) | Ruft das Autorisierungstoken für die SharePoint‑Instanz ab. |
| [getSiteUrl()](#getSiteUrl--) | Ermittelt die URL von PWA an der SharePoint‑Site oder die URL des lokalen Project Server. |
| [getUserName()](#getUserName--) | Ermittelt den Benutzernamen für die SharePoint‑Site. |
| [toString()](#toString--) | Gibt eine Zeichenkettenrepräsentation dieser Instanz zurück. |
### ProjectServerCredentials(String siteUrl, String authToken) {#ProjectServerCredentials-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String authToken)
```


Initialisiert eine neue Instanz der Klasse [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) unter Verwendung der URL der SharePoint‑Site und eines gültigen SPOIDCRL‑Autorisierungstokens für die PWA (Project Web Access)-Site von SharePoint.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| siteUrl | java.lang.String | Die URL der PWA (Project Web Access) API von Project Online. |
|  | authToken | java.lang.String | Das Autorisierungstoken (SPOIDCRL) für die PWA (Project Web Access) Site von SharePoint. |

--------------------

Verwenden Sie diesen Konstruktor, um eine Verbindung zu ProjectOnline herzustellen, wenn Sie bereits ein AuthToken für Ihre SharePoint‑Online‑Site haben. |

### ProjectServerCredentials(String siteUrl, String userName, String password) {#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String userName, String password)
```


Initialisiert eine neue Instanz der Klasse [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) unter Verwendung der URL der SharePoint‑Site, des Benutzernamens und des Passworts.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| siteUrl | java.lang.String | Die URL der PWA (Project Web Access) API von Project Online. |
| userName | java.lang.String | Der Benutzername für die SharePoint‑Site. |
|  | password | java.lang.String | Das Passwort für die SharePoint‑Site. |

--------------------

Verwenden Sie diesen Konstruktor, um eine Verbindung zu ProjectOnline herzustellen. Bitte beachten Sie, dass die Legacy‑Authentifizierung in Ihrem Azure‑Portal und im Office‑365‑Admin‑Center aktiviert sein muss. |

### getAuthToken() {#getAuthToken--}
```
public final String getAuthToken()
```


Ruft das Autorisierungstoken für die SharePoint‑Instanz ab.

**Returns:**
java.lang.String - das Autorisierungstoken für die SharePoint‑Instanz.
### getSiteUrl() {#getSiteUrl--}
```
public final String getSiteUrl()
```


Ermittelt die URL von PWA an der SharePoint‑Site oder die URL des lokalen Project Server. Zum Beispiel, https://your\_company\_name.sharepoint.com/sites/pwa";

**Returns:**
java.lang.String - die URL von PWA an der SharePoint‑Site oder die URL des lokalen Project Server.
### getUserName() {#getUserName--}
```
public final String getUserName()
```


Ermittelt den Benutzernamen für die SharePoint‑Site.

**Returns:**
java.lang.String - der Benutzername für die SharePoint‑Site.
### toString() {#toString--}
```
public String toString()
```


Gibt eine Zeichenkettenrepräsentation dieser Instanz zurück.

**Returns:**
java.lang.String - eine Zeichenkettenrepräsentation dieser Instanz.
