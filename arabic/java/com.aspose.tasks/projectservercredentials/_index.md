---
title: "ProjectServerCredentials"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "بيانات الاعتماد المستخدمة للاتصال بـ Project Online أو مثيل Project Server المحلي."
type: docs
weight: 225
url: /ar/java/com.aspose.tasks/projectservercredentials/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerCredentials
```

بيانات الاعتماد المستخدمة للاتصال بـ Project Online أو مثيل Project Server المحلي.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ProjectServerCredentials(String siteUrl, String authToken)](#ProjectServerCredentials-java.lang.String-java.lang.String-) | يُنشئ مثيلًا جديدًا من الفئة [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) باستخدام URL لموقع SharePoint ورمز التفويض SPOIDCRL الصالح لموقع PWA (Project Web Access) الخاص بـ SharePoint. |
| [ProjectServerCredentials(String siteUrl, String userName, String password)](#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-) | يُنشئ مثيلًا جديدًا من الفئة [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) باستخدام URL لموقع SharePoint، اسم المستخدم وكلمة المرور. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getAuthToken()](#getAuthToken--) | يحصل على رمز التفويض لمثيل SharePoint. |
| [getSiteUrl()](#getSiteUrl--) | يحصل على URL الخاص بـ PWA في موقع SharePoint أو URL لخادم Project Server المحلي. |
| [getUserName()](#getUserName--) | يحصل على اسم المستخدم لموقع SharePoint. |
| [toString()](#toString--) | يعيد تمثيلًا نصيًا لهذه النسخة. |
### ProjectServerCredentials(String siteUrl, String authToken) {#ProjectServerCredentials-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String authToken)
```


يُنشئ مثيلًا جديدًا من الفئة [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) باستخدام URL لموقع SharePoint ورمز التفويض SPOIDCRL الصالح لموقع PWA (Project Web Access) الخاص بـ SharePoint.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| siteUrl | java.lang.String | URL الخاص بواجهة برمجة تطبيقات PWA (Project Web Access) لـ Project Online. |
|  | authToken | java.lang.String | رمز التفويض (SPOIDCRL) لموقع PWA (Project Web Access) الخاص بـ SharePoint. |

--------------------

استخدم هذا المُنشئ للاتصال بـ ProjectOnline عندما يكون لديك بالفعل AuthToken لموقع SharePoint Online الخاص بك. |

### ProjectServerCredentials(String siteUrl, String userName, String password) {#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String userName, String password)
```


يُنشئ مثيلًا جديدًا من الفئة [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) باستخدام URL لموقع SharePoint، اسم المستخدم وكلمة المرور.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| siteUrl | java.lang.String | URL الخاص بواجهة برمجة تطبيقات PWA (Project Web Access) لـ Project Online. |
| userName | java.lang.String | اسم المستخدم لموقع SharePoint. |
|  | password | java.lang.String | كلمة المرور لموقع SharePoint. |

--------------------

استخدم هذا المُنشئ للاتصال بـ ProjectOnline. يرجى ملاحظة أنه يجب تمكين المصادقة القديمة في بوابة Azure ومركز إدارة Office 365. |

### getAuthToken() {#getAuthToken--}
```
public final String getAuthToken()
```


يحصل على رمز التفويض لمثيل SharePoint.

**Returns:**
java.lang.String - رمز التفويض لمثيل SharePoint.
### getSiteUrl() {#getSiteUrl--}
```
public final String getSiteUrl()
```


يحصل على URL الخاص بـ PWA في موقع SharePoint أو URL لخادم Project Server المحلي. على سبيل المثال، https://your\_company\_name.sharepoint.com/sites/pwa";

**Returns:**
java.lang.String - URL الخاص بـ PWA في موقع SharePoint أو URL لخادم Project Server المحلي.
### getUserName() {#getUserName--}
```
public final String getUserName()
```


يحصل على اسم المستخدم لموقع SharePoint.

**Returns:**
java.lang.String - اسم المستخدم لموقع SharePoint.
### toString() {#toString--}
```
public String toString()
```


يعيد تمثيلًا نصيًا لهذه النسخة.

**Returns:**
java.lang.String - تمثيل نصي لهذا الكائن.
