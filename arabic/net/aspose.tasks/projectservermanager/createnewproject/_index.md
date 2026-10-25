---
title: "ProjectServerManager.CreateNewProject"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ProjectServerManager. تُنشئ مشروعًا جديدًا في نسخة Project ServerProject Online باستخدام خيارات الحفظ الافتراضية."
type: docs
weight: 30
url: /ar/net/aspose.tasks/projectservermanager/createnewproject/
---
## CreateNewProject(Project) {#createnewproject}

ينشئ مشروعًا جديدًا في مثيل Project Server\\Project Online باستخدام خيارات الحفظ الافتراضية.

```csharp
public void CreateNewProject(Project project)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| المشروع | Project | المشروع لحفظه إلى مثيل Project Server\Project Online. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | في حالة حدوث خطأ في الاتصال أو خطأ تم إرجاعه من الخادم. |

## الأمثلة

في هذا المثال يتم تحميل المشروع من ملف .mpp وحفظه إلى حساب Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project);
```

يوضح كيفية استخدام ProjectServerManager لإنشاء مشروع جديد على Microsoft Project Online.

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### انظر أيضًا

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## CreateNewProject(Project, ProjectServerSaveOptions) {#createnewproject_1}

ينشئ مشروعًا جديدًا في نسخة Project Server\Project Online باستخدام خيارات الحفظ المحددة.

```csharp
public void CreateNewProject(Project project, ProjectServerSaveOptions saveOptions)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| المشروع | Project | المشروع لحفظه إلى مثيل Project Server\Project Online. |
| saveOptions | ProjectServerSaveOptions | مثال على فئة [`ProjectServerSaveOptions`](../../projectserversaveoptions/). |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | في حالة حدوث خطأ في الاتصال أو خطأ تم إرجاعه من الخادم. |

## الأمثلة

في هذا المثال يتم تحميل المشروع من ملف .mpp وحفظه إلى حساب Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project, new ProjectServerSaveOptions
{
    ProjectName = "My new project"
});
```

يوضح كيفية استخدام مدير Project Server لإنشاء مشروع جديد مع خيارات حفظ مسبقة التعريف على Microsoft Project Online.

```csharp
try
{
    const string sharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(sharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    var options = new ProjectServerSaveOptions
    {
        Timeout = TimeSpan.FromSeconds(10)
    };
    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### انظر أيضًا

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


