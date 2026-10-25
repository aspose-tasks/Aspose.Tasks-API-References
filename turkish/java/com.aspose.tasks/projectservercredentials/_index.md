---
title: "ProjectServerCredentials"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Project Online veya yerel Project Server örneğine bağlanmak için kullanılan kimlik bilgileri."
type: docs
weight: 225
url: /tr/java/com.aspose.tasks/projectservercredentials/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerCredentials
```

Project Online veya yerel Project Server örneğine bağlanmak için kullanılan kimlik bilgileri.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ProjectServerCredentials(String siteUrl, String authToken)](#ProjectServerCredentials-java.lang.String-java.lang.String-) | SharePoint sitesinin URL'si ve geçerli SPOIDCRL yetkilendirme belirteci kullanarak SharePoint'ın PWA (Project Web Access) sitesi için [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) sınıfının yeni bir örneğini başlatır. |
| [ProjectServerCredentials(String siteUrl, String userName, String password)](#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-) | SharePoint sitesinin URL'si, kullanıcı adı ve şifre kullanarak [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getAuthToken()](#getAuthToken--) | SharePoint örneği için yetkilendirme belirtecini alır. |
| [getSiteUrl()](#getSiteUrl--) | SharePoint sitesindeki PWA'nın URL'sini veya yerinde (on-premise) Project Server'ın URL'sini alır. |
| [getUserName()](#getUserName--) | SharePoint sitesi için kullanıcı adını alır. |
| [toString()](#toString--) | Bu örneğin dize temsilini döndürür. |
### ProjectServerCredentials(String siteUrl, String authToken) {#ProjectServerCredentials-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String authToken)
```


SharePoint sitesinin URL'si ve geçerli SPOIDCRL yetkilendirme belirteci kullanarak SharePoint'ın PWA (Project Web Access) sitesi için [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| siteUrl | java.lang.String | Project Online'ın PWA (Project Web Access) API'sinin URL'si. |
|  | authToken | java.lang.String | SharePoint'ın PWA (Project Web Access) sitesi için yetkilendirme belirteci (SPOIDCRL). |

--------------------

SharePoint Online siteniz için zaten AuthToken'ınız olduğunda ProjectOnline'a bağlanmak için bu yapıcıyı kullanın. |

### ProjectServerCredentials(String siteUrl, String userName, String password) {#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String userName, String password)
```


SharePoint sitesinin URL'si, kullanıcı adı ve şifre kullanarak [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| siteUrl | java.lang.String | Project Online'ın PWA (Project Web Access) API'sinin URL'si. |
| userName | java.lang.String | SharePoint sitesi için kullanıcı adı. |
|  | password | java.lang.String | SharePoint sitesi için şifre. |

--------------------

ProjectOnline'a bağlanmak için bu yapıcıyı kullanın. Lütfen eski kimlik doğrulamanın Azure portalınızda ve Office 365 Yönetim merkezinde etkinleştirilmesi gerektiğini unutmayın. |

### getAuthToken() {#getAuthToken--}
```
public final String getAuthToken()
```


SharePoint örneği için yetkilendirme belirtecini alır.

**Returns:**
java.lang.String - SharePoint örneği için yetkilendirme belirteci.
### getSiteUrl() {#getSiteUrl--}
```
public final String getSiteUrl()
```


SharePoint sitesindeki PWA'nın URL'sini veya yerinde (on-premise) Project Server'ın URL'sini alır. Örneğin, https://your\_company\_name.sharepoint.com/sites/pwa\";

**Returns:**
java.lang.String - SharePoint sitesindeki PWA'nın URL'si veya yerinde (on-premise) Project Server'ın URL'si.
### getUserName() {#getUserName--}
```
public final String getUserName()
```


SharePoint sitesi için kullanıcı adını alır.

**Returns:**
java.lang.String - SharePoint sitesi için kullanıcı adı.
### toString() {#toString--}
```
public String toString()
```


Bu örneğin dize temsilini döndürür.

**Returns:**
java.lang.String - bu örneğin dize temsili.
