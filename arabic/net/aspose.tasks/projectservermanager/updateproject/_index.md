---
title: "ProjectServerManager.UpdateProject"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ProjectServerManager. تقوم بتحديث المشروع الموجود في مثيل Project ServerProject Online باستخدام خيارات الحفظ الافتراضية. سيتم استبدال المشروع الموجود"
type: docs
weight: 70
url: /ar/net/aspose.tasks/projectservermanager/updateproject/
---
## UpdateProject(Project) {#updateproject}

يحدّث المشروع الموجود في نسخة Project Server\Project Online باستخدام خيارات الحفظ الافتراضية. سيتم استبدال المشروع الموجود.

```csharp
public void UpdateProject(Project project)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| المشروع | Project | المشروع لحفظه إلى مثيل Project Server\Project Online. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | في حالة حدوث خطأ في الاتصال أو خطأ تم إرجاعه من الخادم. |

## ملاحظات

يجب أن تكون خاصية المشروع 'project.Get(Prj.Guid)' معرف GUID صالح لمشروع موجود في حساب Project Server \ Project Online.

## الأمثلة

في هذا المثال يتم تحميل المشروع من حساب Project Online، ثم تعديلها وحفظها مرة أخرى إلى حساب Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project);
```

يوضح كيفية تحديث المشروع على Microsoft Project Online.

```csharp
const string URL = "https://contoso.sharepoint.com/sites/pwa";
const string Domain = "CONTOSO.COM";
const string UserName = "Administrator";
const string Password = "MyPassword";

var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
try
{
    var manager = new ProjectServerManager(projectServerCredentials);

    ProjectInfo projectInfo = null;
    foreach (var info in manager.GetProjectList())
    {
        if (info.Name == "My project")
        {
            projectInfo = info;
        }
    }

    if (projectInfo == null)
    {
        Console.WriteLine("Project 'My project' not found in working store of Project Online account.");
        return;
    }

    var project = manager.GetProject(projectInfo.Id);
    project.Set(Prj.FinishDate, new DateTime(2020, 03, 01));

    var task = project.RootTask.Children.Add("New task");
    task.Set(Tsk.Start, new DateTime(2020, 02, 26));
    task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));

    manager.UpdateProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine("Failed to update the project. Error: " + ex);
}
```

### انظر أيضًا

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## UpdateProject(Project, ProjectServerSaveOptions) {#updateproject_1}

يحدّث المشروع الموجود في نسخة Project Server\Project Online باستخدام خيارات الحفظ المحددة. سيتم استبدال المشروع الموجود.

```csharp
public void UpdateProject(Project project, ProjectServerSaveOptions saveOptions)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| المشروع | Project | المشروع لحفظه إلى مثيل Project Server\Project Online. |
| saveOptions | ProjectServerSaveOptions | مثال على فئة [`ProjectServerSaveOptions`](../../projectserversaveoptions/). |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | في حالة حدوث خطأ في الاتصال أو خطأ تم إرجاعه من الخادم. |

## ملاحظات

يجب تعيين saveOptions.ProjectGuid إلى معرف GUID لمشروع موجود في مثيل Project Server\ Project Online.

## الأمثلة

في هذا المثال يتم تحميل المشروع من حساب Project Online، ثم تعديلها وحفظها مرة أخرى إلى حساب Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
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

يوضح كيفية تحديث المشروع على Microsoft Project Online باستخدام خيارات حفظ Project Server.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

try
{
    var manager = new ProjectServerManager(credentials);

    ProjectInfo projectInfo = null;
    foreach (var info in manager.GetProjectList())
    {
        if (info.Name == "My project")
        {
            projectInfo = info;
        }
    }

    if (projectInfo == null)
    {
        Console.WriteLine("Project 'My project' not found in working store of Project Online account.");
        return;
    }

    var project = manager.GetProject(projectInfo.Id);
    project.Set(Prj.FinishDate, new DateTime(2020, 03, 01));

    var task = project.RootTask.Children.Add("New task");
    task.Set(Tsk.Start, new DateTime(2020, 02, 26));
    task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));

    var options = new ProjectServerSaveOptions { Timeout = TimeSpan.FromMinutes(5) };

    manager.UpdateProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine("Failed to update the project. Error: " + ex);
}
```

### انظر أيضًا

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


