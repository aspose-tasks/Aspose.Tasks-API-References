---
title: "ProjectServerCredentials"
second_title: "Aspose.Tasks for Java API Reference"
description: "Credenziali utilizzate per connettersi a Project Online o all'istanza on-premise di Project Server."
type: docs
weight: 225
url: /it/java/com.aspose.tasks/projectservercredentials/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerCredentials
```

Credenziali utilizzate per connettersi a Project Online o all'istanza on-premise di Project Server.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ProjectServerCredentials(String siteUrl, String authToken)](#ProjectServerCredentials-java.lang.String-java.lang.String-) | Inizializza una nuova istanza della classe [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) utilizzando l'URL del sito SharePoint e un token di autorizzazione SPOIDCRL valido per il sito PWA (Project Web Access) di SharePoint. |
| [ProjectServerCredentials(String siteUrl, String userName, String password)](#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-) | Inizializza una nuova istanza della classe [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) utilizzando l'URL del sito SharePoint, nome utente e password. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getAuthToken()](#getAuthToken--) | Ottiene il token di autorizzazione per l'istanza SharePoint. |
| [getSiteUrl()](#getSiteUrl--) | Ottiene l'URL di PWA sul sito SharePoint o l'URL del Project Server on-premise. |
| [getUserName()](#getUserName--) | Ottiene il nome utente per il sito SharePoint. |
| [toString()](#toString--) | Restituisce una rappresentazione stringa di questa istanza. |
### ProjectServerCredentials(String siteUrl, String authToken) {#ProjectServerCredentials-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String authToken)
```


Inizializza una nuova istanza della classe [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) utilizzando l'URL del sito SharePoint e un token di autorizzazione SPOIDCRL valido per il sito PWA (Project Web Access) di SharePoint.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| siteUrl | java.lang.String | L'URL dell'API PWA (Project Web Access) di Project Online. |
|  | authToken | java.lang.String | Il token di autorizzazione (SPOIDCRL) per il sito PWA (Project Web Access) di SharePoint. |

--------------------

Utilizza questo costruttore per connetterti a ProjectOnline quando disponi già di AuthToken per il tuo sito SharePoint Online. |

### ProjectServerCredentials(String siteUrl, String userName, String password) {#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String userName, String password)
```


Inizializza una nuova istanza della classe [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) utilizzando l'URL del sito SharePoint, nome utente e password.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| siteUrl | java.lang.String | L'URL dell'API PWA (Project Web Access) di Project Online. |
| userName | java.lang.String | Il nome utente per il sito SharePoint. |
|  | password | java.lang.String | La password per il sito SharePoint. |

--------------------

Utilizza questo costruttore per connetterti a ProjectOnline. Nota che l'autenticazione legacy deve essere abilitata nel tuo portale Azure e nel centro amministrativo di Office 365. |

### getAuthToken() {#getAuthToken--}
```
public final String getAuthToken()
```


Ottiene il token di autorizzazione per l'istanza SharePoint.

**Returns:**
java.lang.String - il token di autorizzazione per l'istanza SharePoint.
### getSiteUrl() {#getSiteUrl--}
```
public final String getSiteUrl()
```


Ottiene l'URL di PWA sul sito SharePoint o l'URL del Project Server on-premise. Per esempio, https://your\_company\_name.sharepoint.com/sites/pwa\";

**Returns:**
java.lang.String - l'URL di PWA sul sito SharePoint o l'URL del Project Server on-premise.
### getUserName() {#getUserName--}
```
public final String getUserName()
```


Ottiene il nome utente per il sito SharePoint.

**Returns:**
java.lang.String - il nome utente per il sito SharePoint.
### toString() {#toString--}
```
public String toString()
```


Restituisce una rappresentazione stringa di questa istanza.

**Returns:**
java.lang.String - una rappresentazione stringa di questa istanza.
