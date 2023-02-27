---
title: ProjectServerCredentials.ProjectServerCredentials
second_title: Aspose.Tasks لمرجع .NET API
description: ProjectServerCredentials البناء. يقوم بتهيئة مثيل جديد لملفProjectServerCredentials فئة باستخدام عنوان URL لموقع SharePoint ورمز ترخيص SPOIDCRL صالح لموقع PWA Project Web Access الخاص بـ SharePoint.
type: docs
weight: 10
url: /ar/net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`ProjectServerCredentials`](../) فئة باستخدام عنوان URL لموقع SharePoint ورمز ترخيص SPOIDCRL صالح لموقع PWA (Project Web Access) الخاص بـ SharePoint.

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| siteUrl | String | عنوان URL لـ PWA (Project Web Access) API الخاص بـ Project Online. |
| authToken | String | رمز التفويض المميز (SPOIDCRL) لموقع PWA (Project Web Access) الخاص بـ SharePoint. |

### ملاحظات

استخدم هذا المُنشئ للاتصال بـ ProjectOnline عندما يكون لديك بالفعل AuthToken لموقع SharePoint Online الخاص بك.

### أنظر أيضا

* class [ProjectServerCredentials](../)
* مساحة الاسم [Aspose.Tasks](../../projectservercredentials/)
* المجسم [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

يقوم بتهيئة مثيل جديد لملف[`ProjectServerCredentials`](../) فئة باستخدام URL لموقع SharePoint واسم المستخدم وكلمة المرور.

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| siteUrl | String | عنوان URL لـ PWA (Project Web Access) API الخاص بـ Project Online. |
| userName | String | اسم المستخدم لموقع SharePoint. |
| password | String | كلمة المرور لموقع SharePoint. |

### ملاحظات

استخدم هذا المُنشئ للاتصال بـ ProjectOnline. الرجاء ملاحظة أنه يجب تمكين المصادقة القديمة في مدخل Azure ومركز إدارة Office 365.

### أنظر أيضا

* class [ProjectServerCredentials](../)
* مساحة الاسم [Aspose.Tasks](../../projectservercredentials/)
* المجسم [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

يقوم بتهيئة مثيل جديد لملف[`ProjectServerCredentials`](../) فئة باستخدام URL لنقطة نهاية Project Web Access وبيانات اعتماد الشبكة.

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| siteUrl | String | عنوان URL لنقطة نهاية الوصول إلى الويب الخاصة بالمشروع. |
| credentials | NetworkCredential | بيانات الاعتماد المستخدمة لتسجيل الدخول إلى نقطة نهاية Project Web Access. |

### ملاحظات

استخدم هذا المُنشئ للاتصال بمثيل محلي لـ Project Server عبر PWA.

### أمثلة

في هذا المثال مثيل[`ProjectServerManager`](../../projectservermanager/)تُستخدم الفئة لقراءة قائمة بالمشروع من مثيل Project Server الموجود على http: //project_server_instance.local

```csharp
string site = "http://project_server_instance.local/sites/pwa ";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);

var list = manager.GetProjectList();
foreach (var projectInfo in list)
{
    Console.WriteLine("{0} - {1} - {2}", projectInfo.Id, projectInfo.CreatedDate, projectInfo.Name);
}
```

### أنظر أيضا

* class [ProjectServerCredentials](../)
* مساحة الاسم [Aspose.Tasks](../../projectservercredentials/)
* المجسم [Aspose.Tasks](../../../)


