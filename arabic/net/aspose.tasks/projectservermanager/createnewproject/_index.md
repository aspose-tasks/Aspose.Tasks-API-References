---
title: ProjectServerManager.CreateNewProject
second_title: Aspose.Tasks لمرجع .NET API
description: ProjectServerManager طريقة. إنشاء مشروع جديد في مثيل Project Server  Project Online باستخدام خيارات الحفظ الافتراضية.
type: docs
weight: 30
url: /ar/net/aspose.tasks/projectservermanager/createnewproject/
---
## CreateNewProject(Project) {#createnewproject}

إنشاء مشروع جديد في مثيل Project Server \ Project Online باستخدام خيارات الحفظ الافتراضية.

```csharp
public void CreateNewProject(Project project)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| project | Project | المشروع الذي سيتم حفظه في مثيل Project Server \ Project Online. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | في حالة حدوث خطأ في الاتصال أو خطأ تم إرجاعه بواسطة الخادم. |

### أمثلة

في هذا المثال ، يتم تحميل المشروع من ملف .mpp وحفظه في حساب Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com "،" yyyyy@xxxxxxx.onmicrosoft.com "،" password ") ;
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project);
```

### أنظر أيضا

* class [Project](../../project/)
* class [ProjectServerManager](../)
* مساحة الاسم [Aspose.Tasks](../../projectservermanager/)
* المجسم [Aspose.Tasks](../../../)

---

## CreateNewProject(Project, ProjectServerSaveOptions) {#createnewproject_1}

إنشاء مشروع جديد في مثيل Project Server \ Project Online باستخدام خيارات الحفظ المحددة.

```csharp
public void CreateNewProject(Project project, ProjectServerSaveOptions saveOptions)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| project | Project | المشروع الذي سيتم حفظه في مثيل Project Server \ Project Online. |
| saveOptions | ProjectServerSaveOptions | حالة[`ProjectServerSaveOptions`](../../projectserversaveoptions/) فصل. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | في حالة حدوث خطأ في الاتصال أو خطأ تم إرجاعه بواسطة الخادم. |

### أمثلة

في هذا المثال ، يتم تحميل المشروع من ملف .mpp وحفظه في حساب Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com "،" yyyyy@xxxxxxx.onmicrosoft.com "،" password ") ;
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project, new ProjectServerSaveOptions
{
    ProjectName = "My new project"
});
```

### أنظر أيضا

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* مساحة الاسم [Aspose.Tasks](../../projectservermanager/)
* المجسم [Aspose.Tasks](../../../)


