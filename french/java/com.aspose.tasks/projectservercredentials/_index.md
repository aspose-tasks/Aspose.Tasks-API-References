---
title: "ProjectServerCredentials"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Identifiants utilisés pour se connecter à Project Online ou à une instance sur site de Project Server."
type: docs
weight: 225
url: /fr/java/com.aspose.tasks/projectservercredentials/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerCredentials
```

Identifiants utilisés pour se connecter à Project Online ou à une instance sur site de Project Server.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ProjectServerCredentials(String siteUrl, String authToken)](#ProjectServerCredentials-java.lang.String-java.lang.String-) | Initialise une nouvelle instance de la classe [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) en utilisant l'URL du site SharePoint et un jeton d'autorisation SPOIDCRL valide pour le site PWA (Project Web Access) de SharePoint. |
| [ProjectServerCredentials(String siteUrl, String userName, String password)](#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-) | Initialise une nouvelle instance de la classe [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) en utilisant l'URL du site SharePoint, le nom d'utilisateur et le mot de passe. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getAuthToken()](#getAuthToken--) | Obtient le jeton d'autorisation pour l'instance SharePoint. |
| [getSiteUrl()](#getSiteUrl--) | Obtient l'URL du PWA sur le site SharePoint ou l'URL du serveur Project Server sur site. |
| [getUserName()](#getUserName--) | Obtient le nom d'utilisateur pour le site SharePoint. |
| [toString()](#toString--) | Renvoie une représentation sous forme de chaîne de cette instance. |
### ProjectServerCredentials(String siteUrl, String authToken) {#ProjectServerCredentials-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String authToken)
```


Initialise une nouvelle instance de la classe [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) en utilisant l'URL du site SharePoint et un jeton d'autorisation SPOIDCRL valide pour le site PWA (Project Web Access) de SharePoint.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| siteUrl | java.lang.String | L'URL de l'API PWA (Project Web Access) de Project Online. |
|  | authToken | java.lang.String | Le jeton d'autorisation (SPOIDCRL) pour le site PWA (Project Web Access) de SharePoint. |

--------------------

Utilisez ce constructeur pour vous connecter à ProjectOnline lorsque vous avez déjà un AuthToken pour votre site SharePoint Online. |

### ProjectServerCredentials(String siteUrl, String userName, String password) {#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String userName, String password)
```


Initialise une nouvelle instance de la classe [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) en utilisant l'URL du site SharePoint, le nom d'utilisateur et le mot de passe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| siteUrl | java.lang.String | L'URL de l'API PWA (Project Web Access) de Project Online. |
| userName | java.lang.String | Le nom d'utilisateur pour le site SharePoint. |
|  | password | java.lang.String | Le mot de passe pour le site SharePoint. |

--------------------

Utilisez ce constructeur pour vous connecter à ProjectOnline. Veuillez noter que l'authentification hérité doit être activée dans votre portail Azure et le centre d'administration Office 365. |

### getAuthToken() {#getAuthToken--}
```
public final String getAuthToken()
```


Obtient le jeton d'autorisation pour l'instance SharePoint.

**Returns:**
java.lang.String - le jeton d'autorisation pour l'instance SharePoint.
### getSiteUrl() {#getSiteUrl--}
```
public final String getSiteUrl()
```


Obtient l'URL du PWA sur le site SharePoint ou l'URL du serveur Project Server sur site. Par exemple, https://your\_company\_name.sharepoint.com/sites/pwa";

**Returns:**
java.lang.String - l'URL du PWA sur le site SharePoint ou l'URL du serveur Project Server sur site.
### getUserName() {#getUserName--}
```
public final String getUserName()
```


Obtient le nom d'utilisateur pour le site SharePoint.

**Returns:**
java.lang.String - le nom d'utilisateur pour le site SharePoint.
### toString() {#toString--}
```
public String toString()
```


Renvoie une représentation sous forme de chaîne de cette instance.

**Returns:**
java.lang.String - une représentation sous forme de chaîne de cette instance.
