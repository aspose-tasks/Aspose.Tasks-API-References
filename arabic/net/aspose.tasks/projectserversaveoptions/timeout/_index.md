---
title: "ProjectServerSaveOptions.Timeout"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ProjectServerSaveOptions. تحصل أو تعيين مهلة الانتظار المستخدمة عند انتظار معالجة طلب حفظ المشروع بواسطة خدمة معالجة طابور Project Servers. القيمة الافتراضية لهذه الخاصية هي دقيقة واحدة"
type: docs
weight: 50
url: /ar/net/aspose.tasks/projectserversaveoptions/timeout/
---
## ProjectServerSaveOptions.Timeout property

يحصل أو يضبط مهلة الانتظار المستخدمة عند انتظار معالجة طلب حفظ المشروع بواسطة خدمة معالجة طابور Project Server. القيمة الافتراضية لهذه الخاصية هي دقيقة واحدة.

```csharp
public TimeSpan Timeout { get; set; }
```

## ملاحظات

قد يكون وقت المعالجة أطول للمشاريع الكبيرة أو في حالة ان كان مثيل Project Server مشغولاً جداً في الاستجابة للطلبات الأخرى.

## الأمثلة

يوضح كيفية تحديث المشروع على Microsoft Project Online والتحكم في قيمة مهلة الحفظ.

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

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


