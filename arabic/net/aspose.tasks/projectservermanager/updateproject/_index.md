---
title: ProjectServerManager.UpdateProject
second_title: Aspose.Tasks لمرجع .NET API
description: ProjectServerManager طريقة. يقوم بتحديث المشروع الموجود في Project Server  Project Online باستخدام خيارات الحفظ الافتراضية. سيتم الكتابة فوق المشروع الحالي.
type: docs
weight: 70
url: /ar/net/aspose.tasks/projectservermanager/updateproject/
---
## UpdateProject(Project) {#updateproject}

يقوم بتحديث المشروع الموجود في Project Server \ Project Online باستخدام خيارات الحفظ الافتراضية. سيتم الكتابة فوق المشروع الحالي.

```csharp
public void UpdateProject(Project project)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| project | Project | المشروع الذي سيتم حفظه في مثيل Project Server \ Project Online. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | في حالة حدوث خطأ في الاتصال أو خطأ تم إرجاعه بواسطة الخادم. |

### ملاحظات

يجب أن تكون خاصية Project.Get (Prj.Guid) الخاصة بالمشروع دليلًا إرشاديًا صالحًا لمشروع موجود في مثيل Project Online / Project Server.

### أمثلة

في هذا المثال ، يتم تحميل المشروع من حساب Project Online ، وتعديله وحفظه مرة أخرى في حساب Project Online .

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com "،" yyyyy@xxxxxxx.onmicrosoft.com "،" password ") ;
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project);
```

### أنظر أيضا

* class [Project](../../project/)
* class [ProjectServerManager](../)
* مساحة الاسم [Aspose.Tasks](../../projectservermanager/)
* المجسم [Aspose.Tasks](../../../)

---

## UpdateProject(Project, ProjectServerSaveOptions) {#updateproject_1}

يقوم بتحديث المشروع الموجود في Project Server \ Project Online باستخدام خيارات الحفظ المحددة. سيتم الكتابة فوق المشروع الحالي.

```csharp
public void UpdateProject(Project project, ProjectServerSaveOptions saveOptions)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| project | Project | المشروع الذي سيتم حفظه في مثيل Project Server \ Project Online. |
| saveOptions | ProjectServerSaveOptions | حالة[`ProjectServerSaveOptions`](../../projectserversaveoptions/) فصل. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | في حالة حدوث خطأ في الاتصال أو خطأ تم إرجاعه بواسطة الخادم. |

### ملاحظات

يجب تعيين saveOptions.ProjectGuid إلى دليل إرشادي لمشروع موجود على مثيل Project Server \ Project Online.

### أمثلة

في هذا المثال ، يتم تحميل المشروع من حساب Project Online ، وتعديله وحفظه مرة أخرى في حساب Project Online .

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com "،" yyyyy@xxxxxxx.onmicrosoft.com "،" password ") ;
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project, new ProjectServerSaveOptions
{
    ProjectGuid = projectGuid
});
```

### أنظر أيضا

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* مساحة الاسم [Aspose.Tasks](../../projectservermanager/)
* المجسم [Aspose.Tasks](../../../)


