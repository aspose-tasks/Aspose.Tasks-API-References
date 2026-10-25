---
title: "الفئة ProjectServerCredentials"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.ProjectServerCredentials. بيانات الاعتماد التي تُستخدم للاتصال بـ Project Online أو نسخة محلية من Project Server"
type: docs
weight: 1490
url: /ar/net/aspose.tasks/projectservercredentials/
---
## ProjectServerCredentials class

بيانات الاعتماد المستخدمة للاتصال بـ Project Online أو مثيل Project Server المحلي.

```csharp
public sealed class ProjectServerCredentials
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ProjectServerCredentials](projectservercredentials/#constructor)(string, NetworkCredential) | ينشئ مثلاً جديداً من الفئة `ProjectServerCredentials` باستخدام عنوان URL لنقطة نهاية Project Web Access وبيانات الاعتماد الشبكية. |
| [ProjectServerCredentials](projectservercredentials/#constructor_1)(string, string) | ينشئ مثلاً جديداً من الفئة `ProjectServerCredentials` باستخدام عنوان URL لموقع SharePoint ورمز تفويض SPOIDCRL صالح لموقع PWA (Project Web Access) الخاص بـ SharePoint. |
| [ProjectServerCredentials](projectservercredentials/#constructor_2)(string, string, string) | ينشئ مثلاً جديداً من الفئة `ProjectServerCredentials` باستخدام عنوان URL لموقع SharePoint، اسم المستخدم وكلمة المرور. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AuthToken](../../aspose.tasks/projectservercredentials/authtoken/) { get; } | يحصل على رمز التفويض لنسخة SharePoint. |
| [SiteUrl](../../aspose.tasks/projectservercredentials/siteurl/) { get; } | يحصل على عنوان URL لـ PWA في موقع SharePoint أو عنوان URL لـ Project Server المحلي. على سبيل المثال، https://your_company_name.sharepoint.com/sites/pwa"; |
| [UserName](../../aspose.tasks/projectservercredentials/username/) { get; } | يحصل على اسم المستخدم لموقع SharePoint. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [ToString](../../aspose.tasks/projectservercredentials/tostring/)() | يعيد تمثيلًا نصيًا لهذا الكائن. |

## الأمثلة

يعرض كيفية استخدام بيانات اعتماد خادم المشروع لاسترجاع قائمة المشاريع من Microsoft Project Online.

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var newProject = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(newProject);

    IEnumerable<ProjectInfo> list = manager.GetProjectList();

    foreach (var info in list)
    {
        var project = manager.GetProject(info.Id);
        Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
        Console.WriteLine("Resources count: {0}", project.Resources.Count);
    }
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


