---
title: "ProjectServerCredentials"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Credenciales que se utilizan para conectarse a Project Online o a una instancia local de Project Server."
type: docs
weight: 225
url: /es/java/com.aspose.tasks/projectservercredentials/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerCredentials
```

Credenciales que se utilizan para conectarse a Project Online o a una instancia local de Project Server.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ProjectServerCredentials(String siteUrl, String authToken)](#ProjectServerCredentials-java.lang.String-java.lang.String-) | Inicializa una nueva instancia de la clase [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) usando la URL del sitio SharePoint y un token de autorización SPOIDCRL válido para el sitio PWA (Project Web Access) de SharePoint. |
| [ProjectServerCredentials(String siteUrl, String userName, String password)](#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-) | Inicializa una nueva instancia de la clase [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) usando la URL del sitio SharePoint, el nombre de usuario y la contraseña. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getAuthToken()](#getAuthToken--) | Obtiene el token de autorización para la instancia de SharePoint. |
| [getSiteUrl()](#getSiteUrl--) | Obtiene la URL de PWA en el sitio SharePoint o la URL del Project Server local. |
| [getUserName()](#getUserName--) | Obtiene el nombre de usuario para el sitio SharePoint. |
| [toString()](#toString--) | Devuelve una representación en cadena de esta instancia. |
### ProjectServerCredentials(String siteUrl, String authToken) {#ProjectServerCredentials-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String authToken)
```


Inicializa una nueva instancia de la clase [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) usando la URL del sitio SharePoint y un token de autorización SPOIDCRL válido para el sitio PWA (Project Web Access) de SharePoint.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| siteUrl | java.lang.String | La URL de la API PWA (Project Web Access) de Project Online. |
|  | authToken | java.lang.String | El token de autorización (SPOIDCRL) para el sitio PWA (Project Web Access) de SharePoint. |

--------------------

Utilice este constructor para conectarse a ProjectOnline cuando ya tenga AuthToken para su sitio SharePoint Online. |

### ProjectServerCredentials(String siteUrl, String userName, String password) {#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String userName, String password)
```


Inicializa una nueva instancia de la clase [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) usando la URL del sitio SharePoint, el nombre de usuario y la contraseña.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| siteUrl | java.lang.String | La URL de la API PWA (Project Web Access) de Project Online. |
| userName | java.lang.String | El nombre de usuario para el sitio SharePoint. |
|  | password | java.lang.String | La contraseña para el sitio SharePoint. |

--------------------

Utilice este constructor para conectarse a ProjectOnline. Tenga en cuenta que la autenticación heredada debe estar habilitada en su portal de Azure y en el centro de administración de Office 365. |

### getAuthToken() {#getAuthToken--}
```
public final String getAuthToken()
```


Obtiene el token de autorización para la instancia de SharePoint.

**Returns:**
java.lang.String - el token de autorización para la instancia de SharePoint.
### getSiteUrl() {#getSiteUrl--}
```
public final String getSiteUrl()
```


Obtiene la URL de PWA en el sitio SharePoint o la URL del Project Server local. Por ejemplo, https://your\\_company\\_name.sharepoint.com/sites/pwa\";

**Returns:**
java.lang.String - la URL de PWA en el sitio SharePoint o la URL del Project Server local.
### getUserName() {#getUserName--}
```
public final String getUserName()
```


Obtiene el nombre de usuario para el sitio SharePoint.

**Returns:**
java.lang.String - el nombre de usuario para el sitio SharePoint.
### toString() {#toString--}
```
public String toString()
```


Devuelve una representación en cadena de esta instancia.

**Returns:**
java.lang.String - una representación en cadena de esta instancia.
