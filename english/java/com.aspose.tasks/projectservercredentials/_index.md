---
title: ProjectServerCredentials
second_title: Aspose.Tasks for Java API Reference
description: Credentials which are used to connect to Project Online or on-premise instance of Project Server.
type: docs
weight: 224
url: /java/com.aspose.tasks/projectservercredentials/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerCredentials
```

Credentials which are used to connect to Project Online or on-premise instance of Project Server.
## Constructors

| Constructor | Description |
| --- | --- |
| [ProjectServerCredentials(String siteUrl, String authToken)](#ProjectServerCredentials-java.lang.String-java.lang.String-) | Initializes a new instance of the [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) class using URL of SharePoint site and valid SPOIDCRL authorization token for SharePoint's PWA (Project Web Access) site. |
| [ProjectServerCredentials(String siteUrl, String userName, String password)](#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-) | Initializes a new instance of the [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) class using URL of SharePoint site, user name and password. |
## Methods

| Method | Description |
| --- | --- |
| [getAuthToken()](#getAuthToken--) | Gets the authorization token for the SharePoint instance. |
| [getSiteUrl()](#getSiteUrl--) | Gets the URL of PWA at SharePoint site or URL of on-premise Project Server. |
| [getUserName()](#getUserName--) | Gets the user name for SharePoint site. |
| [toString()](#toString--) | Returns a string representation of this instance. |
### ProjectServerCredentials(String siteUrl, String authToken) {#ProjectServerCredentials-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String authToken)
```


Initializes a new instance of the [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) class using URL of SharePoint site and valid SPOIDCRL authorization token for SharePoint's PWA (Project Web Access) site.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| siteUrl | java.lang.String | The URL of PWA (Project Web Access) API of Project Online. |
| authToken | java.lang.String | The authorization token (SPOIDCRL) for SharePoint's PWA (Project Web Access) site.

--------------------

Use this constructor to connect to ProjectOnline when you already have AuthToken for your SharePoint Online site. |

### ProjectServerCredentials(String siteUrl, String userName, String password) {#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String userName, String password)
```


Initializes a new instance of the [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) class using URL of SharePoint site, user name and password.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| siteUrl | java.lang.String | The URL of PWA (Project Web Access) API of Project Online. |
| userName | java.lang.String | The user name for the SharePoint site. |
| password | java.lang.String | The password for the SharePoint site.

--------------------

Use this constructor to connect to ProjectOnline. Please note that legacy authentication should be enabled in your Azure portal and Office 365 Admin center. |

### getAuthToken() {#getAuthToken--}
```
public final String getAuthToken()
```


Gets the authorization token for the SharePoint instance.

**Returns:**
java.lang.String - the authorization token for the SharePoint instance.
### getSiteUrl() {#getSiteUrl--}
```
public final String getSiteUrl()
```


Gets the URL of PWA at SharePoint site or URL of on-premise Project Server. For example, https://your\_company\_name.sharepoint.com/sites/pwa";

**Returns:**
java.lang.String - the URL of PWA at SharePoint site or URL of on-premise Project Server.
### getUserName() {#getUserName--}
```
public final String getUserName()
```


Gets the user name for SharePoint site.

**Returns:**
java.lang.String - the user name for SharePoint site.
### toString() {#toString--}
```
public String toString()
```


Returns a string representation of this instance.

**Returns:**
java.lang.String - a string representation of this instance.
