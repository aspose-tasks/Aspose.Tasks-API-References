---
title: ProjectServerManager.ProjectServerManager
second_title: Aspose.Tasks لمرجع .NET API
description: ProjectServerManager البناء. يقوم بتهيئة مثيل جديد لملفProjectServerManager فئة .
type: docs
weight: 10
url: /ar/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

يقوم بتهيئة مثيل جديد لملف[`ProjectServerManager`](../) فئة .

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| credentials | ProjectServerCredentials | بيانات الاعتماد المستخدمة للاتصال بحساب Project Online. |

### أمثلة

يوضح هذا المثال كيفية إنشاء مثيل ProjectServerManager للوصول إلى مثيل Project Server في مقر الشركة.

```csharp
[C#]
string site = "http://project_server_instance.local/ ";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

يوضح هذا المثال كيفية إنشاء مثيل ProjectServerManager للوصول إلى الحساب في خدمة Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com "،" yyyyy@xxxxxxx.onmicrosoft.com "،" password ") ;
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

### أنظر أيضا

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* مساحة الاسم [Aspose.Tasks](../../projectservermanager/)
* المجسم [Aspose.Tasks](../../../)


