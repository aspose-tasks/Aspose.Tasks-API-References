---
title: "الفئة ProjectServerSaveOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.ProjectServerSaveOptions. يسمح بتحديد خيارات إضافية عند حفظ المشروع إلى Project Server أو Project Online."
type: docs
weight: 1510
url: /ar/net/aspose.tasks/projectserversaveoptions/
---
## ProjectServerSaveOptions class

يسمح بتحديد خيارات إضافية عند حفظ المشروع إلى Project Server أو Project Online.

```csharp
public sealed class ProjectServerSaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ProjectServerSaveOptions](projectserversaveoptions/)() | يقوم بتهيئة نسخة جديدة من الفئة `ProjectServerSaveOptions`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [PollingInterval](../../aspose.tasks/projectserversaveoptions/pollinginterval/) { get; set; } | يحصل أو يضبط الفاصل الزمني بين طلبات حالة وظائف الطابور. القيمة الافتراضية هي 2 ثانية. |
| [ProjectGuid](../../aspose.tasks/projectserversaveoptions/projectguid/) { get; set; } | يحصل أو يضبط المعرف الفريد للمشروع. يجب أن يكون فريدًا داخل مثيل Project Server \ Project Online. |
| [ProjectName](../../aspose.tasks/projectserversaveoptions/projectname/) { get; set; } | يحصل أو يضبط اسم المشروع الذي يُعرض في قائمة مشاريع Project Server \ Project Online. يجب أن يكون فريدًا داخل مثيل Project Server \ Project Online. إذا تم حذف القيمة، سيتم استخدام قيمة الخاصية Prj.Name بدلاً من ذلك. |
| [Timeout](../../aspose.tasks/projectserversaveoptions/timeout/) { get; set; } | يحصل أو يضبط مهلة الانتظار المستخدمة عند انتظار معالجة طلب حفظ المشروع بواسطة خدمة معالجة طابور Project Server. القيمة الافتراضية لهذه الخاصية هي دقيقة واحدة. |

## الأمثلة

يوضح كيفية استخدام خيارات &lt;see cref="Aspose.Tasks.ProjectServerSaveOptions" /&gt; لإنشاء مشروع جديد في مثيل Project Server المحلي.

```csharp
try
{
    const string URL = "https://project_server.local/sites/pwa";
    const string Domain = "CONTOSO.COM";
    const string UserName = "Administrator";
    const string Password = "MyPassword";

    var project = new Project(DataDir + @"Project1.mpp");

    var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
    var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
    var manager = new ProjectServerManager(projectServerCredentials);
    var options = new ProjectServerSaveOptions
                      {
                          ProjectGuid = Guid.NewGuid(),
                          ProjectName = "New project",
                          Timeout = TimeSpan.FromMinutes(5),
                          PollingInterval = TimeSpan.FromSeconds(3)
                      };

    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


